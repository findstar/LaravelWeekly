http://driesvints.com/blog/weekly-laravel-4-learnings-week-1/

이글은 [weekly-laravel-weekly-1](http://driesvints.com/blog/weekly-laravel-4-learnings-week-1/) 의 글을 번역한것입니다.

원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.

#Laravel 4 Learnings: week1


저는 Laravel4 를 배우는 모든 과정을 기록하기로 마음먹고, 그 과정들을 매주 이 블로그에 포스팅하기로 결정했습니다. 앞으로 기록하게 되는 이 내용들이 Laravel4를 배우고자 하는 다른 사람들에게 도움이 되길 바랍니다. 매주 가능한 많은 팁들을 기록하고자 합니다. 이 포스팅이 그 시작인 첫번째 포스팅입니다.


자 그럼 시작하겠습니다!



##헬퍼 메소드(Helper methods)

: Lravel을 아는 사람들이 어떻게 알고 있는지는 모르겠지만, Laravel4 에는 코드를 이해하는데 드는 시간을 절약하고 많은 도움을 줄 수 있는 helper methods 가 존재합니다. 이러한 helper methods 는 `Illuminate\Support\helpers.php`(번역주 : vender/laravel/framework/src/Illuminate/Support/helpers.php 파일입니다. ) 에서 찾을 수 있습니다. 그 중에 하나를 소개하자면 다음과 같습니다.

 

##이름이 지정된 리소스풀 라우트(Named resourceful routes)

('<route name>@method') 와 같은 형식의  named resourceful routes 를 추가하는것이 가능한지에 대해서 Laravel4의 메뉴얼 에서도도,  github을 통해서  질문해 보았었지만 [link](https://github.com/laravel/framework/issues/550) 찾을 수가 없었습니다. 하지만 Taylor 가 알려주길 이미 이러한 route 를 추가하는것이 가능하다고 알려주었습니다.

(번역주 : 여기서 이야기하는 Named resourful routes 라는 것은 route.php 에서  resource 에 대한 route 를 정하는데 있어 이름을 지정하는 것을 의미합니다. Route::resource('....','...') 형식임을 생각하시면 됩니다. [한국어메뉴얼#컨트롤러](http://laravel-korea.org/docs/controllers)를 참고하시면 좀 더 이해하는데 도움이 됩니다.)


모든 resourceful route 는 자동으로 그 자신을 라우팅 할 수 있는 고유 이름을 가지게 됩니다. 이 이름은 실제로 지정된 route의 형식이 아니고, 단지 resourceful route 을 가리킬뿐입니다. 기본적으로 resourceful 컨트롤러의 메소드와 연결되는 링크를 구성하기를 원한다면 다음과 같이 할 수 있습니다.

	// route 는 resourceful controller 에 해당하는 링크를 생성합니다.

	//route() 메소드는 helper function. 에서 찾을 수 있습니다.
	route('users.edit',1);  // 이렇게 수행하는 것은

	// 다음과 같은 결과를 생성합니다. 

http://example.com/users/1/edit
route 메소드를 사용한 이러한 형식은 복잡한 네임스페이스 컨트롤러 구성에서 아주 편하게 사용 될 수 있습니다.  이러한 방식은 모든 컨트롤러의 액션(메소드)를 수행하기 위한 모든 네임스페이스 형식을 타이핑하는 수고를 덜어줄 수 있습니다. (- 한마디로 컨트롤러와 메소드로 구성된 긴 형식의 이름을 간소화 시킬 수 있다는 것을 의미합니다. )

리소스 집합이나, prefixed 된 reoute 의 경우에도 마찬가지로 가능한데, admin prefix 하위의 user controller 를 구성할때, 간단하게 다음과 같이 표현할 수 있습니다.

	route('admin.users.edit', 1);
이런식으로 타이핑을 하는데 시간과 수고로움을 절약할 수 있습니다.

	(번역주 : route 라는 helper 메소드는 resourceful route 를 가리키는 url을 리턴받을 수 있습니다.  helper.php 에서 653 라인 부근의  소스를 살펴보면 reoute 와 함께 parameter와 absolute 를 매개변수로 넘기게 되어 있는데, reoute 메소드 에서 컨트롤러로 지정된 reoute 에 대한 메소드 호출에 대한 경로도 reoute 라는 helper 메소드를 통해서 얻을 수 있다라는 것을 의미합니다.  - reouseful route 를 지칭하는 간단한 이름을 통해서 링크를 리턴받는 기능을 수행한다. )

 

##제너레이터 (Generators)

제너레이터는 정말 좋은 기능입니다. Nettuts 의 에디터 Jeffery Way는 Artisan CLI 의 custom generator 를 통해서 확장이 가능하도록  Laravel 4 의 패키지를 개발하였습니다. 제너레이터는 여러분들이 주로 코딩하는 Laravel 4 의 다양한 부분을 쉽게 생성 할 수 있도록 해줍니다. 이것이 의미하는 것은 매번 번거롭게 추가해야되는 코딩을 줄여줄 수 있다는 것을 이야기 하는 것입니다. Jeffrey 가 포스팅한 비디오에서 좀 더 자세히 확인 할 수  있습니다. [https://tutsplus.com/lesson/custom-generators/](https://tutsplus.com/lesson/custom-generators/)
 

	(번역주 : 실제로 resource controller 를 추가하는 데는 수동으로 컨트롤러 파일을 생성 할경우 신경 써주어야 되는 부분들을 Laravel 에서 사용하는 Artisan 이라는 command line interface 기반의 명령어를 통해서 손쉽게 진행 할 수 있습니다. controller 를 추가하거나 DB 테이블을 생성하는데에도 손쉽게 사용 할 수 있다는 것을 의미합니다. 동영상을 보시는 것이 좀 더 이해하는 데 도움이 됩니다.  )



##리소스 네이밍 컨벤션(Resource naming conventions)

코딩 컨벤션과 같이 리소스 네임을 지정하는 주제에 대해서 역자가 IRC 채널에서 질문을 해보았습니다. (번역주 : 이글이 쓰여질 당시 2013년 5월 17일) 특별히 리소스 네이밍 컨벤션이 문서에 기록되어 있다고 생각하지는 않지만, 모두가 컨트롤러는 복수형태로 네이밍을 정하는데 동의하는 것으로 보여집니다. 이 말은 예를 들어 컨트롤러의 이름을 정하는데 있어 `UserController` 대신에 `UsersController`를 사용한다는 것을 의미합니다. (단수 말고 복수로 사용하는 형태)  Route 에 이어 view 에서도 동일하게 구성하는데  (`users.show.blade.php` )와 같이 사용됩니다. 다만, 다른 것과는 다르게 예외로 모델의 경우에는 단수형태로 네이밍을 지정합니다. 예)  User. 모델.



##Model::lists() - 메소드.

우리 회사의 [@jannemoonvx](https://twitter.com/jannemoonvx) 가 발견한 매우 깔끔하고 작은 기능이 하나 있습니다. 하나의 model 구조를 나타내는 Key/value 형태의 배열을 얻고자 한다면, lists() 함수를 사용하면 됩니다. 배열의 key / value 를 구성하는데 있어서 lists 함수의 첫번째 파라미터는 배열의 값을 나타내는 Model 컬럼을 쓰고, 두번째 파라미터는  key로 사용되는 Model 컬럼을 씁니다. 다음 예를 보면 두번째 파라미터인 id 컬럼을 사용하여 key로 지정하고 first_name 값을 배열의 값으로 할당한 결과를 가져옵니다. 이렇게 하면 User 모델에서 id 값을 key 로 하고, first_name 을 값으로 하는 배열을 반환 받을 수 있습니다.

	$keyValueArray = User::lists('first_name', 'id');


##결론 Conclusion

지금 작성한 Tip이 그 누구에게라도 도움이 되길 바랍니다. 다음 주에는 좀더 많은것을 공유할 수 있도록 노력 하겠습니다. Laravel4를 시작한 이례로 매주 알게 되는 사항들이 PHP를 배우는데 있어서 많은 도움이 되고 있으며, 뿐만 아니라 진행하는 작업들의 생산성과 속도를 높이데 많은 도움을 주고 있습니다.

질문이 있다면 트위터를 통해서 편하게 질문해 주세요: [@driesvints](http://twitter.com/driesvints)



 - - -
원 글은 다음 링크에서 확인하실 수 있습니다. [Original Link](http://driesvints.com/blog/weekly-laravel-4-learnings-week-1/)**


번역주 : weekly #1 의 내용은 helper method 가 유용하게 쓰일 수 있다는 것을 이야기 하고 있고, 몇몇 메소드에 대해서 설명하고 있습니다. 번역을 진행하고 나니, helper method를 좀 더 자세히 살펴볼 필요가 있겠다는 생각이 드네요. 한글 메뉴얼도 있으니 참고하시면 좋을것 같습니다. [link](http://laravel-korea.org/docs/helpers)**

 
오역이나, 기타 문법, 문맥적으로 매끄럽지 못한 부분에 대한 사항은 [@findstar](https://twitter.com/findstar) 이나 뎃글 주시면 수정하겠습니다.**


원글에 대한 저작권한은 [@driesvints](https://twitter.com/driesvints) 에게 있습니다.**