http://laravel.io/topic/29/laravel-weekly-11

*이글은 [laravel weekly #11](http://laravel.io/topic/29/laravel-weekly-11) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*


# Laravel Weekly #11

 새로운 라라벨 위클리에 오신것을 환영합니다. Laravel 4가 릴리즈 된지 이제막 일주일이 되었는데요, 벌써 엄청난 양의 글들이 올라오고 있습니다. 나는 모든 최신 정보들를 제공하기 위해서 노력할 것입니다.

 첫번째로 Laravel IRC 채널이 [laravel.io](http://laravel.io) 로 이동되었습니다. 다음 주소에서 확인할 수 있습니다. [laravel.io/irc](http://laravel.io/irc). Laravel에 관한 질문이 있거나 Laravel 개발자들과 채팅 하기를 원한다면 IRC에 참여하세요!

[.net 어워드 결과가 발표되었습니다.](http://www.thenetawards.com/) 그리고 안타깝게도 Laravel 은 "올해의 오픈소스 프로젝트"에 들지 못했습니다. 하지만 [Bootstrap](http://twitter.github.io/bootstrap/) 과 경쟁해서 뒤진것이 그다지 창피한일은 아닙니다. 2014년을 기대해 봅시다!

몇몇 분들이 Laravel 4 T 셔츠를 [받기 시작했습니다](https://twitter.com/jonathanmarvens/status/341195091270041600). 벌써 받으셨나요? 셔츠를 받으신분들은 코멘트를 달아주세요! 만약 신청을 하지 못했었다면 두번째 캠페인이 진행중입니다.  [클릭](http://teespring.com/laravel-redux).

읽어주셔서 감사합니다. 다음주에 뵈요!

Dries  
[@driesvints](https://twitter.com/driesvints)  
[driesvints.com](http://driesvints.com)

## 뉴스(News)

### Laravel 3 Documentation

Laravel 3 문서가 사라져서 당황한 Laravel 3 개발자를 보았습니다. 걱정하지 마세요. 이곳에서 Laravel 3 문서를 확인할 수 있습니다. [three.laravel.com/docs](http://three.laravel.com/docs).

*출처: [https://twitter.com/laravelphp/status/340202010957721600](https://twitter.com/laravelphp/status/340202010957721600)*

### Laracon EU: 첫번째 발표자가 공개되었습니다(First Speakers Announced)

[Laracon EU](http://laracon.eu/2013/)의 첫번째 발표자가 공개되었습니다. 그리고 곧 다음 발표자가 공개될것입니다ㅏ. 발표자들의 놀라운 모습들을 직접 볼 수 있는 기회를 놓치지 마세요. 25%의 티켓이 판매되었고 아직 나머지는 판매중입니다.

*출처: [https://twitter.com/laraconeu/status/340123245036593152](https://twitter.com/laraconeu/status/340123245036593152)* 

### 손쉬운 설치법(Easier Laravel 4 Installation)

*A quick tip by [Laravel](https://twitter.com/laravelphp)*

컴포저에는 [packagist](https://packagist.org/)에서 패키지를 다운받고 동시에 바로 설치 명령을 실행할 수 있는 편리한 기능이 있습니다. Laravel 4를 쉽게 설치 하는 방법은 다음 명령어를 수행하면 됩니다.

	composer create-project laravel/laravel

*출처: [https://twitter.com/laravelphp/status/340461054263955457](https://twitter.com/laravelphp/status/340461054263955457)*

### From Apprentice To Artisan

[Taylor](https://twitter.com/taylorotwell)가 새로운 서적을 집필하고 있습니다. 아직 내용이 확정되지 않았지만 공개되는 즉시 자세한 사항들을 알려드리겠습니다. 

*출처: [https://twitter.com/taylorotwell/status/340197912476794880](https://twitter.com/taylorotwell/status/340197912476794880)*

### Laravel 4 Release

*An article by [Maksim Surguy](https://twitter.com/msurguy)*

Maksim이 Laravel 4에서의 새로운 점, Laravel 3 와 4의 비교 그리고 Laravel 4 릴리즈 스케줄뿐만 아니라, Laravel 4를 시작하는데 유용한 참고 자료들에 대한 포스팅을 작성했습니다.

*출처: [http://maxoffsky.com/code-blog/laravel-4-is-released/](http://maxoffsky.com/code-blog/laravel-4-is-released/)*

### Laravel 4 Primer

*An article by [The Nerdary](http://www.thenerdary.net/)*

[Kenny Meyers](http://kennymeyers.com/)가 Laravel 4에 대한 간단한 리뷰와 흥미로은 참고자료 목록들을 블로그에 올렸습니다. 

*출처: [http://www.thenerdary.net/post/52067531360/laravel-4-primer](http://www.thenerdary.net/post/52067531360/laravel-4-primer)*

### 언어파일(Laravel 4 Language Files)

*A Github repository by [Caouecs](https://twitter.com/caouecs)*

Laravel 4 어플리케이션에서 사용할 수 있는 언어 파일들을 모아놓은 멋진 github 프로젝트 입니다.

*출처: [https://github.com/caouecs/Laravel4-lang](https://github.com/caouecs/Laravel4-lang)*

## 참고자료들 

### 기사글

[Laravel 4 on Google AppEngine for PHP](http://blog.neoxia.com/laravel-4-on-google-appengine-for-php/) by [Gilles Mergoil](https://twitter.com/gmergoil)  
[Simple Website with Orchestra Platform 2 (Part 1)](http://orchestraplatform.com/blogs/2013/06/01/simple-website-1/) by [Mior Muhammad Zaki](http://crynobone.com/)  
[Simple Website with Orchestra Platform 2 (Part 2)](http://orchestraplatform.com/blogs/2013/06/01/simple-website-2/) by [Mior Muhammad Zaki](http://crynobone.com/)  
[Simple Website with Orchestra Platform 2 (Part 3)](http://orchestraplatform.com/blogs/2013/06/01/simple-website-3/) by [Mior Muhammad Zaki](http://crynobone.com/)  
[Simple Website with Orchestra Platform 2 (Part 4)](http://orchestraplatform.com/blogs/2013/06/02/simple-website-4/) by [Mior Muhammad Zaki](http://crynobone.com/)  
[Laravel 4 Gems: Query results caching](http://www.develophp.org/2013/05/laravel-4-query-results-caching/) by [Franz Liedke](http://www.develophp.org/)  
[Laravel 4 Gems: Model query scopes](http://www.develophp.org/2013/05/laravel-4-model-query-scopes/) by [Franz Liedke](http://www.develophp.org/)  
[Laravel 4 Gems: Maintenance mode](http://www.develophp.org/2013/05/laravel-4-maintenance-mode/) by [Franz Liedke](http://www.develophp.org/)  
[Modules in Laravel 4](http://creolab.hr/2013/05/modules-in-laravel-4/) by [Boris Strahija](https://twitter.com/strija)

### 유용한 패키지들(Packages)

[Mongovel](https://github.com/julien-c/mongovel) by [Julien Chaumond](https://twitter.com/julien_c)

### 스크린캐스트(Screencasts)

[Quick Introduction To Basset's Application Collection](http://vimeo.com/67466414) by [Jason Lewis](http://jasonlewis.me/)

### 기타 링크(Other links)

[Laravel Austin meetup group](http://www.meetup.com/Laravel-Austin/)

## 이벤트(Events)

04/06 - Meetup - Fullerton - [Laravel 4 Release party!](http://www.meetup.com/Laravel-Framework-Fullerton-Meetup-Group/events/117567592/)  
27/06 - Talk - Chicago - [Laravel For The CodeIgniter Developer by Taylor Otwell](http://peersconf.com/2013/sessions#25)  
01/07 - Meetup - New York - [Community intro/show and tell](http://www.meetup.com/New-York-Laravel/events/122708162/)    
30/08 - 31/08 - Conference - Amsterdam - [Laracon EU 2013](http://laracon.eu/2013/)  
