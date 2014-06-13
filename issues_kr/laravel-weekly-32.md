http://us7.campaign-archive2.com/?u=60fa14809d4de70a885daf382&id=d1535be76f

*이글은 [laravel weekly #32](http://us7.campaign-archive2.com/?u=60fa14809d4de70a885daf382&id=d1535be76f) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*

# Laravel Weekly #32

추수감사절을 맞이 하여 Black Friday와 Cyber Monday를 즐겁게 보냈기를 바랍니다!

Laravel 4.1 버전이 이제 릴리즈를 바로 앞두고 있습니다. 오늘 Symfony 2.4버전이 릴리즈 되었고 Laravel 4.1이 이제  막바지 작업만이 남았습니다. 조금만 더 기다려 주세요!

(역자주 : laravel 4.1 버전에서는 Symfony 2.4 버전을 기반으로 하는데 Symfony 2.4 버전이 정식릴리즈되어 이제 곧 laravel 4.1이 출시될 예정이라는 뜻입니다. )

즐거운 한주 되세요!


## 뉴스(News)

### PHP Town Hall Episode #16

[지난 PHP Townhall 에피스드에서](http://phptownhall.com/blog/2013/12/02/episode-16-taylor-otwell-laravel41/), [Phill Sturgeon](https://twitter.com/philsturgeon) 이 [Taylor Otwell](https://twitter.com/taylorotwell) 과 [Zack Kitzmiller](https://twitter.com/zackkitzmiller)을 초대하여 이야기를 진행했습니다. 주요 주제는 Laravel 4.1과 Go 그리고 Vagrant에 대한 내용이었습니다.

(역자주 : PHP Town Hall 은 Phill Sturgeon이 진행하는 팟캐스트 입니다.)

### Fortrabbit Adds Deployment Files

Fortrabbit에서 배포파일을 통해서 어플리케이션을 배포하는 방법을 새롭게 추가하였습니다. 자세한 내용은 [튜토리얼 문서](http://fortrabbit.com/docs/in-depth/deployment-file)를 참고해주세요. 또는 Laracast의 [스크린캐스트](https://laracasts.com/lessons/fortrabbit-deploment-files)를 확인하실 수도 있습니다..

(역자주 : fortrabbit는 PHP 호스팅 플랫폼 서비스를 제공하는 업체입니다.)

### 새로운 PSR 표준(A New PSR Standard)

[새로운 PSR-4 표준](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-4-autoloader.md) 제정 투표 결과 해당 표준이 통과되어 이제 곧 여러분의 프로젝트에서 사용할 수 있을것 같습니다. PSR-4는 주로 개발자가 자신의 코드를 구성하는 데 있어서 손쉬운 구조를 택할 수 있도록 autoloader와 관련된 내용을 포함하도록 설계되었습니다.

### Taylor를 위한 크리스마스 이벤트(Christmas for Taylor)

크리스 마스를 맞이 하여 Taylor가 그동안 우리에게 놀라운 프레임워크를 선물해준 것에 대한 보답을 하려고 합니다. 바로 크리스마스 이벤트말이죠 ! Dayle이 Taylor의 크리스마스 선물을 마련하기 위해서 기부를 할 수 있는 페이지를 만들었습니다. [도네이션에 참가하세요!](http://daylerees.com/christmas-for-taylor) :)

### Laravel Tricks

이번에 [Maksim Surguy](https://twitter.com/msurguy)가 [Stidges](http://www.stidges.com/)와 함께 새로운 웹사이트를 개설했습니다. [Laravel Tricks](http://www.laravel-tricks.com/tricks/dynamic-view-assignments)입니다. 이 사이트는 Laravel 을 사용하는 방법들을 공개하며 사용자들이 손쉽게 서로의 자료를 공유할 수 있도록 합니다.


## 간단한 팁(Quick Tip)

[Pavel Polyakov](https://github.com/PavelPolyakov) 가 알려준 팁입니다. [Route::controller()를 사용한 라우팅 룰에 이름을 지정하는 방법입니다.](https://gist.github.com/PavelPolyakov/7688524).


## 참고 자료들(Resources)

### 블로그 자료들(Articles)

[Laravel Queues With Beanstalkd](http://glenntaylor.co.uk/blog/read/laravel-queues-with-beanstalkd)  
[Working with jQuery Ajax Uploader and Laravel PHP](http://ryantablada.com/post/working-with-jquery-ajax-uploader-and-laravel-php)  
[Decoupling the Framework](http://kristopherwilson.com/2013/11/27/decoupling-the-framework)   

### 어플리케이션 & 패키지(Applications and Packages)

[Fakefactory](https://github.com/skovachev/fakefactory)  
[Laravel Multi Auth](https://github.com/ollieread/multiauth)  

### Laracasts

[Laravel From Scratch - Record Creation](https://laracasts.com/series/laravel-from-scratch/episodes/11)  
[Laravel From Scratch - Validation](https://laracasts.com/series/laravel-from-scratch/episodes/12)  
[Laravel From Scratch - Refactoring](https://laracasts.com/series/laravel-from-scratch/episodes/13)  
[Fortrabbit Configuration](https://laracasts.com/lessons/fortrabbit-deploment-files)  
[Tinkering With Boris](https://laracasts.com/lessons/tinkering-with-boris)  
[Migrations Decoded](https://laracasts.com/lessons/migrations-decoded)  
[Seeds and Fakes](https://laracasts.com/lessons/seeds-and-fakes)  

### 프리젠테이션 자료(Slides)

[Introduction to Laravel - You have arrived.](https://speakerdeck.com/francisconeves/introduction-to-laravel-you-have-arrived)  

### 기타링크(Other Links)

[The Fall of PEAR and the Rise of Composer](http://benramsey.com/blog/2013/11/the-fall-of-pear-and-the-rise-of-composer/)  
[Becoming a PHP Professional: The Importance of Others](http://www.sitepoint.com/becoming-php-professional-importance-others/)  


## 이벤트(Events)

**December 4, 2013 - Toronto**  
[Community Intro and Show/Tell](http://www.meetup.com/Laravel-Toronto/events/147045302/)

**December 10, 2013 - Brussels, Belgium**  
[December Laravel Meetup](http://www.meetup.com/Laravel-Brussels/events/148643492/)