http://us7.campaign-archive2.com/?u=60fa14809d4de70a885daf382&id=19dd711e7a

*이글은 [laravel weekly #25](http://us7.campaign-archive2.com/?u=60fa14809d4de70a885daf382&id=19dd711e7a) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*

# Laravel Weekly #25

[Laracasts](https://laracasts.com) 사이트가 정식으로 오픈했습니다. 그동안 Larave 4가 릴리즈된 이후에 이와 관련된 정보를 제대로 알려줄 수 있는 공간이 필요했습니다. Laracasts 는 다양한 분야 - 아키텍쳐, 레파지토리, 테스팅, 배포등과 관련된 다양한 주제에 대한 학습용 스크린 캐스트를 제공하는 훌륭한 대안이 될것입니다. 만약 여러분이 어떤 주제에 대해서 더 많은 스크린캐스트를 보고싶다면 포럼을 통해서 Jeffrey에게 요청할 수 있습니다. [포럼 사이트](http://laracasts.com/forum/).

지난주에 Laravel 4.1 부터 Artisan 커맨드에 추가된 기능들이 있습니다. 정식 릴리즈가 되기 전에 새로운 원격 구성 요소들과 라이브 디버거를 사용해보도록 하겠습니다.

이번주도 읽어주셔서 감사합니다. 다음주에 봐요!

## 뉴스(News)

### phpstorm 에서 artisan 커맨드를 지원합니다.(Native Artisan Support in PhpStorm)

 JetBrains 사의 phpstorm IDE 에서 Laravel Artisan 커맨드를 지원하기 시작했습니다. [phpstom 블로그 소식을 확인해 보세요](http://blog.jetbrains.com/phpstorm/2013/09/command-line-tools-based-on-symfony-console-doctrine-laravel-in-phpstorm/).

### Laravel 4.1 Artisna 커맨드의 새로운 기능(New Laravel 4.1 Artisan Features)

Laravel 4.1 에 추가 기능들이 마무리 되면서 이제 릴리즈가 가까워져 오고 있습니다. 4.1 버전에서는 Artisan 커맨드에 "tinker" 명령어가 추가되었습니다. 함께 [Boris REPL 이 합류하였습니다.](https://twitter.com/laravelphp/status/380883629292806144) .

그리고 "debug" 커맨드는 라이브 디버깅을 위해서 추가된 기능입니다. Taylor가 이에 대해서 Laracon EU 컨퍼런스에서 이야기를 진행했었습니다.

또한 "env" Artisan 커맨드가 추가되었습니다. 이 기능은 어플리케이션이 구동하는 환경을 체크하는데 사용됩니다. 4.0에서도 사용이 가능합니다. 

마지막으로 "view:publish" 커맨드도 추가되었는데요. 이 기능은 패키지 작성자들이 view를 퍼블리싱 하는데 사용됩니다.

### Leanpub 팟캐스트 인터뷰 #13: Taylor Otwell

Leanpub 팟캐스트에 Taylor Otwell이 출연했습니다. [블로그 기사 보기](http://blog.leanpub.com/2013/09/taylor-otwell.html).

### Laracasts 런칭(Laracasts Soft Launch)

[Laracasts](http://laracasts.com/)가 첫번째 비디오 시리즈를 런칭했습니다. 회원가입후 한달에 $9의 가격으로 모든 스크린 캐스트 자료에 엑세스 할 수 있습니다. Laracasts를 통해서 Laravel 커뮤니티 내에서 가장 유명한 컨트리뷰터 중에 한명인 [Jeffrey Way](https://twitter.com/jeffrey_way)의 노하우를 배울 수 있습니다.

## 간단한 팁(Quick Tip)

Laravel에는 표준 파일 함수들 이외에 Filebuilder 클래스기반의 꽤 강력한 파일 핸들러가 있습니다. [자세히 보기](https://gist.github.com/driesvints/6784886)

## 참고 자료들(Resources)

### 블로그 자료들(Articles)

[Creating a Subscription-Based Website with Laravel and Recurly, Part 1](http://www.sitepoint.com/creating-subscription-based-website-laravel-recurly-1/)  
[Creating a Subscription-Based Website with Laravel and Recurly, Part 2](http://www.sitepoint.com/creating-subscription-based-website-laravel-recurly-2/)  
[The Less Code to Write, the Better, Right? Then Use Laravel.](http://www.myjive.com/code-write-better-right-laravel)  
[Codesleeve Laravel 4 Asset Pipeline (inspired by rails/sprockets)](http://www.keltdockins.com/2/post/2013/09/codesleeve-laravel-4-asset-pipeline-inspired-by-railssprockets.html)  
[Caching routes using filters in Laravel 4](http://markvaneijk.com/caching-routes-using-filters-in-laravel-4)  
[An Eloquent Notification Strategy](http://ryantablada.com/post/an-eloquent-notification-strategy)  
[Getting Started with Laravel 4 and PostgreSQL](http://www.codedungeon.org/2013/09/10/getting-started-with-laravel-and-postgresql/)  

### 어플리케이션 & 패키지(Applications & Packages)

[Acclimate](https://github.com/jeremeamia/acclimate)  
[XStatic](https://github.com/jeremeamia/xstatic)  

### 기타 링크(Other Links)

[Clockwork](https://github.com/itsgoingd/clockwork)  
[Deploying Snappy](http://blog.userscape.com/post/deploying-snappy)  

## 이벤트(Events)

**October 3, 2013 - Southlake, TX**  
[Database Bliss: Tips, Tricks, & Pitfalls of Database Design](http://www.meetup.com/laravel-dallas-fort-worth/events/138790412/)

**October 3, 2013 - Groningen, Netherlands**  
[October meetup: Laravel 4](http://www.meetup.com/GroningenPHP/events/139600382/)

**October 10, 2013 - Fishers, IN**  
[Build Systems, Unit Testing, Vagrant, Authentication, Service Providers/IoC, etc](http://www.meetup.com/Laravel-Modern-Web-Apps-in-Carmel-Fishers-Indianapolis/events/141852692/)

**November 9 or 10, 2013 - Los Angeles, CA**  
[Introduction to Laravel PHP framework](http://www.socalcodecamp.com/socalcodecamp/session.aspx?sid=819cd36a-f492-483b-802d-6a770b4f1dcf)

**November 15, 2013 - Location TBD**  
[Laravel Seattle / Vancouver UG Meeting](http://www.meetup.com/Laravel-Seattle-Vancouver/events/142345922/)

## 참여를 기다립니다(We want you...)!

 알고 계시는 자료들, 패키지, 모임소식, 스크린캐스트등 다음주 weekly에 추가될만한 그 어떤 것이라도 이메일로 보내주세요. [hello@laravelweekly.com](mailto:hello@laravelweekly.com)