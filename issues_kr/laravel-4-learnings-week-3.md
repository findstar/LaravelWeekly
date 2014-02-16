http://driesvints.com/blog/laravel-4-learnings-week-3

#Laravel 4 Learnings: week3

*이글은 [weekly-laravel-weekly-3](http://driesvints.com/blog/laravel-4-learnings-week-3) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*

이번주는 라라벨4 베타4 버전이 발표된 대단한 한주였습니다. 프레임워크에는 많은 새로운 기능들이 추가되었습니다. 나는 새로운 기능들 뿐만 아니라 팁, 트위터 및 다음 링크에 게시된 내용들에 대해서 살펴볼 것입니다.
https://twitter.com/laravelphp/status/317671374762156032

#.Net 어워드에서 라라벨에 투표 하세요!

 .Net 어워드 2013년 에서 `2013년 올해의 오픈소스 프로젝트` 카테고리에 라라벨이 목록에 오르게 되었습니다. [라라벨에 투표하세요!](http://www.thenetawards.com/) 투표하는데 어떤 구독권유나, 개인정보를 요청하지 않습니다.

#Cartalyst가 그들의 수익의 1%를 라라벨에 기부하기로 했습니다.

 Cartalyst는 라라벨을 통해서 서비스를 만들 수 있게 된데에 대해서 라라벨과 테일러에게 감사를 표시하기로 했습니다. Cartalyst는 수익의 1%를 라라벨에 기부하기로 하였습니다. Cartalyst의 멋진 결정입니다. 이 결정은 라라벨과 테일러가 프레임워크를 개발하고 라라벨 커뮤니티가 유지되는데 많은 도움이 될 것입니다.

https://twitter.com/Cartalyst/status/316940582356402176

 원하신다면 당신도 기부를 할 수 있습니다. 약간 이라도 라라벨에 도움을 줄 수 있습니다. 그리고 이런 노력들이 당신의 프로젝트에게 다시 도움이 될 것입니다. [이곳](http://laravel.com/about#donations) 에서 진행할 수 있습니다. :)

#라라벨 스택익스체인지 Q&A 사이트

 우리는 스택익스체인지 내부에서 라라벨 Q&A 부분을 분리시킬 수 있도록 노력하고 있습니다. 관심이 있다면 [이곳](http://area51.stackexchange.com/proposals/46607/laravel?referrer=AgG4EvnCx9m753uZWv1VMg2#.UVMgw5DgLGQ.twitter)에서 도움을 줄 수 있습니다.

https://twitter.com/niall_obrien/status/316952716591108096

#라라벨 스크린케스트

 Maksim Surguy 가 라라벨 스크린캐스트들을 볼 수 있는 사이트를 만들었습니다. 라라벨에 대해서 더 배우기를 원하신다면 웹사이트에서 멋진 동영상을 확인하실 수 있습니다. [이곳](http://laracasts.com/)에서 확인하실 수 있습니다.

https://twitter.com/msurguy/status/318130652220375040

##모델 이벤트(Model Events)

 베타4에 추가된 기능인 모델 이벤트 기능은 예를 들어 모델을 데이타베이스에 추가하거나,삭제하는 빈번히 발생하는 동작들을 후킹 할 수 있는 간편한 기능을 제공합니다. 그것은 예를들어 다른 모델에서 참조하고 있는 모델을 삭제하려고 한다거나, 멤버 프로퍼티가 값이 없거나 유효하지 않는 상태에서 모델을 생성하려고 하는 것을 방지하는 방법을 제공합니다. 단순히 2가지의 경우 뿐만 아니라 더 많은 경우에 모델 이벤트 기능을 사용 할 수 있습니다.

 라라벨 메뉴얼에서 전체 이벤트 목록을 확인할 수 있습니다. 이에 대해서 따로 블로깅을 준비하고 있으니 다음 weekly 에서 그에 대해서 이야기 해볼 수 있을 것입니다. :)

##아티잔 라우트 명령어(Artisan Routes Command)

Jeffrey Way 가 제안한 "routes" 명령어가 라라벨 4 코어에 추가되었습니다. 이 명령어는 당신의 어플리케이션의 라우트 룰과 연결된 행동들을 확인하는 간편한 방법입니다.

https://twitter.com/laravelphp/status/316574137676070913


##아티잔 dump-autoload 명령어(Artisan dump-autoload Command)

 어떤 사람들은 `composer dump-autoload` 명령어를 이미 알고 있을 수도 있습니다. 라라벨에서는 artisan 에 이와 동일한 명령어를 추가하였습니다. 이 명령어가 당신의 어플리케이션를 최적화 하는데 도움이 될 것이며 특히 패키지를 개발하고 있다면 도움이 될것 입니다.

다음과 같이 실행합니다. :

```
$ php artisan dump-autoload
```

##상위 모델의 타임스탬프 갱신Touching Parent Timestamps

 엘로퀀트 모델에서의 유용한 기능중에 하나는 상위 모델의 타임스탬프를 갱신 할 수 있다는 것입니다. 하나의 모델은  belongTo()라는 관계를 표현하는 메소드를 가지고있습니다. 만약 상위 모델 이름을 값으로 가지는 배열로된 $touches 라는 멤버변수를 포함하고 있다면 하위 모델이 수정될 때 상위 모델의 updated_at 컬럼이 함께 갱신됩니다. 더 자세한 내용은 [이 문서](http://four.laravel.com/docs/eloquent#touching-parent-timestamps)를 참고하세요.

##와일드 카드 Urls(Wildcard Urls)

 라라벨 베타4의 고유기능이 아니라 이전 버전부터 지원했던 부분이지만, 라라벨4에서 문법이 조금 바뀌었습니다. 예를 들어 CMS를 만들고 있다면 이 기능을 사용할 수 있습니다.
데이타베이스의 고유한 인덱스값을 나타내는 URL이 있고, 이에 대응하는 post 라는 모델을 가지고 있다고 생각해 봅시다. 그리고 URL 값에 따라서 Post 내용을 보여주려 합니다. 그렇다면 다음과 같이 route 를 설정할 수 있습니다 :

```
Route::get('{param}', function($param)
{
    // url 을 통해서 Post 모델 검색
    if  ($post = Post::where('url', $param)->first())
    {
        // view 생성
        return View::make('post', compact('post'));
    }

    // 모델을 찾지 못한 경우에 404 에러.
    App::abort(404).
});
```

 특정 url 을 입력하게 되면 route 클로저는 url 에 해당하는 post 모델을 검색하게 됩니다. 해당되는 모델을 찾았다면 view 생성됩니다. 당신이 생각해야 할것은 이 와일드카드 형식의 라우트 룰은 라우트 파일 마지막에 위치해야한다는 것입니다. 그렇지 않으면 다른 라우트 룰이 실행되기 전에 이 와일드카드 형식의 라우트 룰이 실행되어 다른것이 수행되지 않습니다. 먼저 "고정" 경로 및 경로 그룹을 등록하고 마지막 단계에서 와일드 카드 경로를 배치합니다.

 그건 그렇고, 위의 코드에서 [compact](http://php.net/manual/en/function.compact.php) 함수를 모르신다면 이 함수의 기능은 단지 배열의 키와 자신의 이름으로 된 변수와 배열을 만드는 역활을 한다는 것을 이해하시면 됩니다.

 또한 다음과 같이 여러개의 와일드카드 파라미터를 설정할 수도 있습니다.

```
Route::get('{param}/{param2?}', function($param, $param2 = null)
{
    // 첫번째 또는 두번째 둘다의 파리미터에 대응
});
```

 위의 코드는 첫번째 파라미터를 찾고 선택적으로 두번째 파라미터를 찾습니다. 두번째 파라미터 마지막의 '?' 문자는 이 파라미터가 선택적 - 옵션임을 의미합니다. 이러한 방법은 중첩된 페이지 모델을 처리할 수 있는 좋은 방법입니다.

##헬퍼 메소드(with Helper Method)

 이제 보여드릴 것은 깔끔하고 편리한 헬퍼 메소드 중에 하나입니다. :)

 제 생각에 많은 개발자들이 정적함수가 아닌 특정 함수를 호출하기 전에 먼저 새로운 클래스 인스턴스를 생성해야 된다는 것이 때때로 귀찮고 짜증나는 일이라는 것을 알고 있습니다. 아마 예전에 이런식으로 작업을 하고 있었을 것입니다. :

```
// 새로운 오브젝트를 인스턴스화 함.
$post = new Post;
// 스태틱이 아는 함수를 호출.
$postTypes = $post->getPostTypes();
```

with() 헬퍼 메소드를 사용하면 이러한 작업들이 쉬워집니다.

```
$postTypes = with(new Post)->getPostTypes();
```

 기본적으로 with 메소드는 함께 전달되는 것 객체를 반환합니다. 이것은 당신이 객체의 새 변수를 만들 필요가 없다는 것을 의미합니다. 그래서 당신은 새로운 객체를 위한 변수를 생성할 필요가 없다는 것을 의미합니다.

##더 읽어볼만한 자료들

- [Howto : AJAX multiple file upload in Laravel](http://maxoffsky.com/code-blog/howto-ajax-multiple-file-upload-in-laravel/) by [Maksim Surguy](https://twitter.com/msurguy)
- [Incredible large PHP resources list](https://gist.github.com/ziadoz/1677679) by [Jamie York](https://twitter.com/jamieyork)
- [Sending mail with Postmark](https://tutsplus.com/lesson/sending-mail-with-postmark/) by [Jeffrey Way](https://twitter.com/jeffrey_way)
- [Install Laravel with symlink through terminal shell function/command mamp](http://davidheward.com/2013/03/install-laravel-with-symlink-through-terminal-shell-functioncommand-mamp/) by [David Heward](https://twitter.com/daveheward)
- [I didn’t want to be the ideas person any more](http://insanemission.com/post/46285751294/i-didnt-want-to-be-the-ideas-person-any-more) by [Adam Smith](https://twitter.com/adamontherun)
- [Creating a Custom Laravel 4 Auth Driver](http://toddish.co.uk/blog/creating-a-custom-laravel-4-auth-driver/) by [Todd Francis](https://twitter.com/Toddish)
- [Vagrant development machine provisioned and configured for PHP and Laravel](https://github.com/Aboalarm/devbox) by [Stefan Neubig](https://twitter.com/stefanneubig)
- [ETags and Concurrency Control in Laravel 4](http://fideloper.com/laravel4-etag-concurrency-control) by [Chris Fidao](https://twitter.com/fideloper)
- [An interview with Taylor Otwell](http://webuildatnight.com/features/Laravel) by [We Build At Night](http://webuildatnight.com/)


##유용한 패키지

- [API package for Cartalyst](http://forums.laravel.io/viewtopic.php?pid=32702#p32702)
- [Laravel 4 Auth package](http://docs.toddish.co.uk/verify-l4/) by [Todd Francis](https://twitter.com/Toddish)
- [Keeping revisions of your laravel model data](http://www.chrisduell.com/blog/development/keeping-revisions-of-your-laravel-model-data/) by [Chris Duell](https://twitter.com/duellsy)


##감사합니다!

 다시한번 읽어주셔서 감사합니다. 라라벨 4에 대해서 어떤 좋은 블로그 글이나 패키지 또는 다른 어떤 것이라도 알려주신다면 다음주 포스트에 포함하도록 하겠습니다. :)


*원 글은 다음 링크에서 확인하실 수 있습니다. [Original Link](http://driesvints.com/blog/laravel-4-learnings-week-3)*


*오역이나, 기타 문법, 문맥적으로 매끄럽지 못한 부분에 대한 사항은 [@findstar](https://twitter.com/findstar) 이나 뎃글 주시면 수정하겠습니다.*


*원글에 대한 저작권한은 [@driesvints](https://twitter.com/driesvints) 에게 있습니다.*