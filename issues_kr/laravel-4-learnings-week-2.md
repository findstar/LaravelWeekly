#Laravel 4 Learnings: week2

*이글은 [weekly-laravel-weekly-2](http://driesvints.com/blog/laravel-4-learnings-week-2/) 의 글을 번역한것입니다.원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*
 

지난한주는 Laravel4 에 있어서 대단한 한주였습니다. 많은 기능들과 여러 유용한 팁,그리고 자료들이 추가되었습니다. 

##Laravel4 베타4 버전이 이전주 목요일에 릴리즈 될 예정입니다. 

Laravel4 의 4번째 베타버전이 메뉴얼과 함께 이번주 목요일에 릴리즈 될 예정입니다.새롭게 추가된 멋진 기능들을 확인 해 볼 수 있을 것입니다! :)

##Laracon 스크린캐스트(영상 자료들)

아직 Laracon 스크린캐스트를 보지 못했다면 [all the Laracon screencasts](http://www.youtube.com/user/LaravelScreencasts) 사이트에서 확인하실 수 있습니다. 수고해준 [Chris Borgia](https://twitter.com/cborgia) 에게 고마움을 표시합니다.

## 만약 Helpers functions 을 어디에 추가해야될지 모르겠다면 composer를 확인해 보십시오.

이번주 초반에 [Laravel IRC](http://laravel.com/irc) 에서 이 질문을 해봤습니다.(헬퍼 함수들을 어디에 추가하는게 좋을지) 많은 사람들이 `app/start/global.php` 에 추가해야된다고 하더군요. 나는 전에는 라우터 필터 전에 파일을 위치하는 것이 맞다고 생각되어 helpers function 을 추가 하고자 할 때 `app/filters.php` 안에 넣고는 했었습니다. 만약 당신이 `global.php` 파일을 열어본다면 당신은 `filters.php` 파일이 제일 마지막에서 호출되는 것을 볼 수 있습니다. 그리고 여러가지들을 여기에 넣는 것이 더 좋습니다. 왜냐하면 이 지점이 어플리케이션의 시작점이 되기 때문입니다. 기본적으로 프로그램이 동작하기 전에 필요로하는 모든 추가 함수들을 의미한다고 할 수 있습니다.

또한 다른 방법으로 분리된 `custom.php` 파일을 'app/start'에 만들 수도 있습니다. 그리고 그것을 `global.php` 에서 `filters.php` 파일을 호출하기 전에 포함 시킬 수도 있습니다. 이러한 방법은 `global.php` 파일의 기본 코드와 당신의 코드를 분리하는 좋은 방법이기도 합니다.


```
require __DIR__.'/custom.php';
require __DIR__.'/../filters.php';

```
이방법을 통해서 여러분이 작성한 함수들을 파일로 분리할 수 있습니다.

이렇게 추가한 함수들을 어디에 위치시키는가 하는 정해진 방법은 없습니다. 예를 들어 Laravel4의 view composers 에 대한 매뉴얼을 보자면 다음과 같습니다.:

> 컴포저 클래스들을 어느곳에 둘것인가 하는 정해진 컨벤션은 없습니다. composer.json 파일이 오토로딩을 할 수 있는 어느곳이라도 자유롭게 파일을 둘 수 있습니다.

이렇게 이야기 하고 있습니다. 따라서 오토로딩을 할 수 있는 위치라면 어느 곳이라도 마음대로 파일 위치를 정할 수 있습니다.

##모델에서의 네임스페이스Namespacing your models

나는 모델의 첫부분에 네임스페이스를 추가하는 것이 어플리케이션 개발에 도움이 된다는 것을 깨달았습니다. 왜냐하면 당신이 어플리케이션을 개발함에 있어서 언젠가는 동일한 이름이 이미 laravel 어플리케이션 안에 존재할 수 있다는 것을 깨달을 것이기 때문입니다. `File`이라는 이름을 가지는 모델을 생각해 봅시다. 라라벨에서는 이미 파일시스템상에서 파일들을 다루는 파사드의 이름으로 `File`이라는 명칭을 사용하고 있습니다. 이러한 이유로 `File` 이라는 동일한 이름을 사용하는 것은 간섭을 일으킬 수 있습니다. 여기서 필요한 것이 바로 네임스페이스 입니다.

```
<?php namespace Models;

class File extends Eloquent {

    protected $table = 'files';

}
```

이제 모델에 네임스페이스를 선언하였습니다. 그리고 더이상 어플리케이션 내의 동일한 이름에 대한 간섭을 걱정할 필요가 없습니다. 그리고 그 다음으로 이제 모델 내에서 `$table` 프로퍼티를 설정해야될 필요가 있습니다 . 그렇지 않으면 라라벨은 모델 파일명을 가지고 데이타베이스 테이블을 호출할 것이기 때문입니다. (번역주: $table 프로퍼티를 설정함으로써 모델델이 호출하는 테이블명을 지정할 수 있습니다. )

이제 네임스페이스를 지정한 모델을 컨트롤러, 라우터 등에서 간섭에 대한 걱정 없이 사용할 수 있습니다.

```
Models\File::find(1);
```

 다른 예로 지정한 모델을 사용하면서 글로벌 네임스페이스로 부터 File 별칭을 사용할 수도 있습니다.

```
<?php

use Models\File;

class UserController extends BaseController {

    public function index()
    {
        // File 모델 사용
        $file = File::find(1);

        // File 별칭을 통한 모델 사용 (글로벌 네임스페이스)
        return \File::get($file->filepath);
    }

}
```

만약 당신이 처음부터 모델에 네임스페이스를 지정했다면 나중에 다른곳에서 동일한 이름때문에 문제가 발생할 여지를 줄여줄 것입니다.

##모델 쿼리 스코프 Model query scopes

몇일 전에 라라벨4 베타 버전에 모델 쿼리 스코프 기능이 추가되었습니다!

https://twitter.com/laravelphp/status/314568892376829952


##데이타베이스 합계 함수 Database aggregate functions

이건 라라벨4에서 추가된 기능으로 정말 유용합니다. 수학적인 함수들을 사용해서 데이타베이스로 부터 즉시 값을 얻을 수 있습니다.

Source: [링크](http://laravel.com/docs/queries#aggregates)


##폼 안에서의 플래쉬 데이타 값에 대해서 걱정하지 마십시오.

Jeffry way 가 다음 트윗에서 이것을 알려주었습니다. 뷰안의 폼에 값을 넣어야 될 일이 있을 때 라라벨이 자동으로 값들을 채워줍니다. 완전 좋아요! :)

https://twitter.com/jeffrey_way/status/315128216148922368

https://twitter.com/jeffrey_way/status/315128395346362370

##Laravel Testing Decoded

Jeffrey Way가 집필한 라라벨 테스팅에 대한 멋진 책이 나왔습니다. [a cool eBook](https://leanpub.com/laravel-testing-decoded)


##참고

이번 weekly 를 준비하는데 참고한 내용들입니다.
 - [Error After A Composer Update Of The Laravel 4 Beta](http://jasonlewis.me/article/error-afer-a-composer-update-of-the-laravel-4-beta) by [Jason Lewis](https://twitter.com/jasonclewis)
 - [Snappy](http://besnappy.com/): Helpdesk service by [Userscape](http://www.userscape.com/) which is actually build by Taylor amongst others. You can bet Laravel is powering it ;)
 - A bunch of new videos are up at Nettuts: https://tutsplus.com/course/whats-new-in-laravel-4/
 - [PHPunit wrappers for Laravel 4](https://github.com/JeffreyWay/PHPUnit-Wrappers) by [Jeffrey Way](http://twitter.com/jeffreyway)
 - [Eloquent relationship tip](http://net.tutsplus.com/tutorials/tools-and-tips/pro-workflow-in-laravel-and-sublime-text/) by [Phil Sturgeon](http://twitter.com/philsturgeon)
 - [Pro workflow in Sublime Text 2 and Laravel](http://net.tutsplus.com/tutorials/tools-and-tips/pro-workflow-in-laravel-and-sublime-text/) by Nettuts
 - [Laravel wallpapers!](https://github.com/msurguy/Laravel-wallpapers) by [Maksim Surguy](https://twitter.com/msurguy)
 - [Installing and updating Laravel 4](http://niallobrien.me/2013/03/installing-and-updating-laravel-4/) by [Niall O'Brien](https://twitter.com/niall_obrien)
 - [Authentication & Authorisation](http://niallobrien.me/2013/03/authentication-authorisation/) by [Niall O'Brien](https://twitter.com/niall_obrien)
 - - -
*원 글은 다음 링크에서 확인하실 수 있습니다. [Original Link](http://driesvints.com/blog/laravel-4-learnings-week-2/)*


*오역이나, 기타 문법, 문맥적으로 매끄럽지 못한 부분에 대한 사항은 [@findstar](https://twitter.com/findstar) 이나 뎃글 주시면 수정하겠습니다.*


*원글에 대한 저작권한은 [@driesvints](https://twitter.com/driesvints) 에게 있습니다.*