http://us7.campaign-archive1.com/?u=60fa14809d4de70a885daf382&id=7d3830b80c

*이글은 [laravel weekly #23](http://us7.campaign-archive1.com/?u=60fa14809d4de70a885daf382&id=7d3830b80c) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*


# Laravel Weekly #23

Laracon EU가 끝난지도 벌써 일주일이 훌쩍 지났습니다. 컨퍼런스를 통해서 많은 사람들을 직접 만날 수 있어서 즐거웠습니다. 참석하신 모든분들께 감사의 인사를 드립니다! 내년까지 어떻게 기다리나요.

Laracon EU가 끝나고 2주동안 많은 일들이 있었습니다. Chris의 책 , Implementing Laravel가 오늘 출간되었고 Laracasts 사이트가 정식 오픈하였습니다. 그리고 사람들은 멋진 블로그와 자료들을 다시 작성하고 있습니다.

벌써 뉴스레터 구독자가 406명을 넘어섰습니다. 여러분들께 감사드립니다.

이번주 뉴스레터를 즐겨주시고, 다음주에 뵈어요!

## 뉴스(News)

### Laracon EU 요약(Laracon EU Recap)

 즐거웠던 Laracon EU가 끝난지도 벌써 2주가 지났습니다! 다시금 잊을 수 없는 이벤트를 만드는데 수고해주신 발표자들과 스폰서들, 참석해주신 모든 분들, 그리고 컨퍼런스가 진행되었던 빔 하우스의 스태프들, 자원봉사자분들 끝으로 컨퍼런스와 관련된 모든 분들께 다시한번 감사드립니다. 특히나 행사를 진행하는데 노력해준 Jeroen 과 Shawn에게도 감사의 말을 전합니다. 덕분에 행사가 순조롭게 진행되었습니다. 발표는 훌륭했고, 음식은 맛 있었습니다 ^^ 빔 하우스에서의 뷰가 참 멋졌습니다. 여러분이 컨퍼런스를 즐겼기를 바라면서 내년에 다시 뵐 수 있기를 기대하겠습니다.

 사전 비디오를 신청하신분들은 영상파일과 발표자료를 확인할 수 있는 링크를 받으셨을 겁니다. 신청자들중 아직 링크를 받지 못하신 분은  [contact@laracon.eu](mailto:contact@laracon.eu)으로 연락 주세요. 확인후 링크를 다시 보내드리겠습니다. 컨퍼런스 전체 영상자료는 정리 작업이 끝나면 공개될 예정입니다.

 그동안 Laravel 커뮤니티에서는 Laracon EU 컨퍼런스의 모습들과 블로그 게시물들 그리고 트위터에 대한 내용으로 분주했습니다. 이에 대해서 한번 모아봤습니다.

**블로그 자료들(Articles)**

[Laracon EU (I)](http://blog.marcomonteiro.net/post/laracon-eu-1)
[Laracon EU (II)](http://blog.marcomonteiro.net/post/laracon-eu-(2))
[Laracon EU (III)](http://blog.marcomonteiro.net/post/laracon-eu-3)
[Laracon EU (IV)](http://blog.marcomonteiro.net/post/laracon-eu-(iv))
[Laracon EU (V)](http://blog.marcomonteiro.net/post/laracon-(v))  
[Laracon Observations](http://blog.fortrabbit.com/laracon-observations/)

**사진(Photos)**

[Dave Shoreman](http://www.flickr.com/photos/101291236@N07/sets/72157635387934720/)
[Jordi Boggiano](http://www.flickr.com/photos/seldaek/sets/72157635332125877/)  
[Raymond Idema](http://www.flickr.com/photos/101145465@N04/sets/72157635338163150/)
[Benedikt Niessen](http://www.flickr.com/photos/benediktniessen/sets/72157635330442674/)
[Stefan Neubig](http://www.flickr.com/photos/emotional-stuntman/sets/72157635322750005/)

또한 지난 토요일 밤에는  #laravel IRC 채널이 한바탕 떠들썩 했습니다. 여기 지난 IRC 에서 있었던 재미난 일들에 대한 내용입니다. [동료개발자 낚기](http://d.pr/i/x68C) ;-)

### 책 출간 소식 - Implementing Laravel Released

[Chris](https://twitter.com/fideloper)' 의 책, [Implementing Laravel 이 출간되었습니다](https://leanpub.com/implementinglaravel). 이 책에서 Chris는 Laravel 코드의 구조, Ioc 컨테이너의 사용법, 서비스 프로바이더를 활용하는 방법과 테스트 가능한 구조 및 유지보수 가능한 코드를 작성하는 방법에 대해서 이야기 합니다.

### Apprentice To Artisan의 새로운 챕터

Taylor Otwell이 그의 책 [Laravel: From Apprentice To Artisan](https://leanpub.com/laravel)에 새로운 챕터를 추가하였습니다. 이 챕터는 디커플링 핸들러에 대한 내용입니다. 앞으로도 몇몇 챕터가 더 추가될 수 있습니다.

### Laravel 4 ACL

[Christopher Pitt](https://twitter.com/followchrisp)가 깊이 있는 튜토리얼의 하나로 [Laravel 4에서의 인증](https://medium.com/on-coding/e8d93c9ce0e2)에 대해서 포스팅을 했습니다. 얼마전에는 [사용자 그룹 관리](https://medium.com/on-coding/a7f2fa1f9791)에 대한 글도 포스팅 해썼습니다. 그의 블로그에는 심도 깊은 팁들과 다양한 사용사례가 많이 있습니다 참고하시면 도움이 될것 같습니다.

### Laracasts Forum

[Laracasts](http://laracasts.com/) 사이트 런칭과 함께 [포럼 사이트](http://laracasts.com/forum/)가 준비 되었습니다. 포럼에서 회원들은 스크린캐스트에 대한 의견이나, PHP 와 Laravel 에 대한 다양한 의견들을 토론할 수 있습니다.

### Laravel 스키마 디자이너(Laravel Schema Designer)

이건 정말 멋진 사이트입니다. [Thomas](https://twitter.com/Okyn01)가  [Laravel 4 스키마 디자이너](http://www.laravelsd.com/) 사이트를 만들었습니다. 스키마 디자이너를 이용하면 기본적인 전체 데이터베이스를 정형화 할 수 있고,  마이그레이션을 내보낼 수 있습니다. 아주 편리합니다!

## 짧은 팁(Quick Tip)

몇주전에 알려드린 폼빌더를 통해서 일정한 범위안의 년도나 개월과 같은 필드의 숫자를 채우는 데 사용할 수 있습니다. [이곳에서 사용법을 확인 할 수 있습니다.](https://gist.github.com/driesvints/6543470#file-laravel-weekly-23-quick-tip-php)

## 참고자료들(Resources)

### 기사자료들(Articles)

[Pivot Tables vs Pivot Models](http://ryantablada.com/post/pivot-tables-vs-pivot-models)
[Assertions on method calls using Mockery](http://lutro.priv.no/posts/assertions-on-method-calls-using-mockery)
[Optimizing for production with Laravel 4](http://lutro.priv.no/posts/optimizing-for-production-with-laravel-4)
[Testable, simple L4 code without repository patterns](http://lutro.priv.no/posts/testable-simple-l4-code-without-repository-patterns)
[Integrating Stripe into Laravel 4 application](http://maxoffsky.com/code-blog/integrating-stripe-into-laravel-4-application/)
[Simple Twitter Feed with Caching Using Laravel and Twitter API](http://www.mackhankins.com/blog/laravel/simple-twitter-feed-with-caching-using-laravel-and-twitter-api)
[How to get Laravel set up in a VM using PuPHPet](http://www.reddit.com/r/PHP/comments/1m7r74/how_to_get_laravel_set_up_in_a_vm_using_puphpet/)
[Is There Merit to Unit Testing Controllers](http://laracasts.com/forum/11-is-there-merit-to-unit-testing-controllers)
[Laravel Quick Tip: Global Route Constraints](http://kuzemchak.net/blog/entry/laravel-quick-tip-global-route-constraints)

### 유용한 어플리케이션 & 패키지(Applications & Packages)

[skorry](https://github.com/flaviozantut/skorry)
[Jl4 Newsletter Application](https://github.com/kJamesy/Laravel4-Newsletter-Application)

### 기타 링크(Other Links)

[Behat for the Rest of Us](https://tutsplus.com/tutorial/behat-for-the-rest-of-us/)
[DesignPatternsPHP](https://github.com/domnikl/DesignPatternsPHP)

## 이벤트 Events

**September 12, 2013 - Fishers, IN**
[Discuss Modern Web & Mobile Development, & Laravel 4's Progress](http://www.meetup.com/Laravel-Modern-Web-Apps-in-Carmel-Fishers-Indianapolis/events/135898802/)

**October 1, 2013 - London, UK**
[First London Laravel Meetup](http://www.meetup.com/London-Laravel/events/139606362/)

**October 3, 2013 - Groningen, Netherlands**
[October meetup: Laravel 4](http://www.meetup.com/GroningenPHP/events/139600382/)

**November 9 or 10, 2013 - Los Angeles, CA**
[Introduction to Laravel PHP framework](http://www.socalcodecamp.com/socalcodecamp/session.aspx?sid=819cd36a-f492-483b-802d-6a770b4f1dcf)