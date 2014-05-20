http://laravel.io/topic/38/laravel-weekly-17

*이글은 [laravel weekly #17](http://laravel.io/topic/38/laravel-weekly-17) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*

# Laravel Weekly #17

이번주에는 많은 일들이 있었습니다. 코드이그나이터는 새로운 관리자를 찾고 있고, Taylor는 그의 책을 출간하였습니다, 그리고 Laracon EU의 마지막 발표자가 공개되는 등 기타 여러 일들이 있었습니다.

지난 2주 동안 진행한 설문조사를 완료하였습니다. 요청된 내용들을 바탕으로 더 많은 노력들을 하겠습니다. 감사합니다.

다음주에 만나요!

## 뉴스(News)

### Laracon EU의 마지막 발표자가 공개되었습니다(Final Laracon EU Speakers Announced)

Laracon EU가 가까워져 오면서 마지막 발표자들이 공개되었습니다. Laravel 프레임워크의 창시자인 [Taylor Otwell](https://twitter.com/taylorotwell)뿐만 아니라 Symfony framework의 창시자인 [Fabien Potencier](https://twitter.com/fabpot)도 포함되었습니다. 
마지막으로 [Ross Tuck](https://twitter.com/rosstuck)는 HTTP 프로토콜에 대해서 이야기 할 예정입니다.

*출처: [http://laracon.eu/2013/](http://laracon.eu/2013/)*

### Laravel: From Apprentice To Artisan 출간

Taylor가 그의 집필을 완료하였습니다. ["Laravel: From Apprentice To Artisan"](https://leanpub.com/laravel)는 dependency injection, interfaces, service providers, SOLID 디자인과 같은 고급 주제들에한 내용을 담고 있습니다. leanpub을 통해서 구매를 하시면 책이 업데이트 되더라도 무료로 확인할 수 있습니다.

*출처: [https://leanpub.com/laravel](https://leanpub.com/laravel)*

### Laravel Weekly 설문조사 결과

2주동안 정확히 244명이 설문조사에 답변해주었습니다. 많은 분들이 참가해주신데에 대해서 감사드립니다! 결과는 다음과 같습니다. 

Would you be interested in a Newsletter?  
뉴스레터에 관심이 있으신가요?

그렇다: 215 (88%)  
아니다: 29 (12%)  

How regurarly do you read Laravel Weekly?  
얼마나 정기적으로 Laravel weekly를 읽고계신가요?

매주: 195 (80%)  
2주간격: 31 (13%)  
매달: 10 (4%)  
기타 (3%)  

On a scale of 1-5,how would you rate the content quality for Laravel Weekly?  
Laravel weekly의 내용에 대해서 1-5점으로 나누어 평점을 매긴다면?

5점: 49 (20%)  
4점: 147 (60%)  
3점: 46 (19%)  
2점: 2 (1%)  

What do you consider more important for Laravel Weekly?  
Laravel Weekly에서 어떤 부분이 더 중요하다고 생각하시나요?

뉴스자료의 양 Amount of news items: 13 (5%)  
참고자료들의 양 Amount of resources: 79 (32%)  
내용의 퀄리티 Content Quality: 144 (59%)  
더 많은 인터뷰 More interviews: 8 (3%)  

Most notable other requests:
기타 요청들 중에 주목할만한 부분들 

- More content 더 많은 내용
- More tutorials 더 많은 튜토리얼
- Quick code tips 코드에 대한 간단한 팁들

많은 사람들이 우리가 하는 일들에 대해서 많은 관심을 가져주었고, 그들의 긍정적인 반응에 감사를 표하지 않을 수 없습니다. 설문조사를 통해서 받은 피드백들을 가지고 여러분들의 요청사항들을 적용하기 위해서 많은 노력과 시도를 하겠습니다. 우선 88% 사람들이 원하고 있는 뉴스레터 부터 시작하도록 하겠습니다.

(*번역주 처음에는 dries vints의 개인 블로그 글로 부터 시작하여 이제는 뉴스레터 형식을 갖추게 되었습니다.)

### 기회를 잡으세요(Win Stuff)!

 [Snappy](http://www.besnappy.com/)팀들은 Laracon EU 에 참석할 수 있는 3장의 티켓과 Taylor의 새로운 책을 제공하기로 하였습니다. [이곳](http://www.besnappy.com/laraconeu)에서 자세한 내용을 확인할 수 있습니다. 

*출처: [http://www.besnappy.com/laraconeu](http://www.besnappy.com/laraconeu)*

### 더 많은 기회를 잡으세요(Win Even More Stuff)!

 그것으로 충분하지 않다면 [Sanisoft](http://www.sanisoft.com/)에서 Laracon EU 2013 티켓을 경품추첨하고 있습니다. 제한없이 모든 사람들이 참가할 수 있습니다!

*출처: [http://laracon.eu/2013/raffle.html](http://laracon.eu/2013/raffle.html)*

### EllisLab Seeking New Owner for CodeIgniter

많은 사람들이 예상했던 일이 일어났습니다. 코드이그나이터를 지원했던 [ElissLab](http://ellislab.com/)이 이제 프레임 워크에 대한 새로운 관리자를 찾고 있습니다. 
그들의 우선순위가 더이상 코드이그나이터가 더 가치있을 수 있게 하는데 시간을 쏟을 수 없기 때문입니다. 코드이그나이터는 지난 몇년간 계속 고군분투 하였지만, Laravel 과 같은 모던한 프레임워크와 같이 새롭워지지 못했습니다. 

*출처: [http://ellislab.com/blog/entry/ellislab-seeking-new-owner-for-codeigniter](http://ellislab.com/blog/entry/ellislab-seeking-new-owner-for-codeigniter)*

### Laravel 4: Diving Into The Source

Jason Lewis가 Laravel core와 각각의 동작에 관한 방법들에 대해서 멋진 글을 작성했습니다.

*출처: [http://jasonlewis.me/article/laravel-4-diving-into-the-source](http://jasonlewis.me/article/laravel-4-diving-into-the-source)*

### 새로운 Wardrobe CMS 기능(New Wardrobe CMS features)

[Wardrobe](http://wardrobecms.com/) CMS 는 최근 새롭게 추가된 기능들에 대한 내용을 작성했습니다.

*출처: [http://wardrobecms.com/post/new-features-galore](http://wardrobecms.com/post/new-features-galore)*

## 참고자료들(Resources)

### 기사자료들(Articles)

[How to Install Laravel 4 on a CentOS 6 VPS](https://www.digitalocean.com/community/articles/how-to-install-laravel-4-on-a-centos-6-vps) by [DigitalOcean](https://www.digitalocean.com)  
[Laravel Sentry 2 with multiple user types](https://gist.github.com/leabdalla/5999421) by [Leandro Abdalla](https://gist.github.com/leabdalla)  
[Why Laravel’s Seeds and Migrations Are Damn Powerful Tools](http://antjanus.com/blog/web-development-tutorials/back-end-development/why-laravels-seeds-and-migration-are-a-damn-powerful-tool/) by [Antonin Januska](http://antjanus.com/)  
[Production-Ready Beanstalkd with Laravel 4 Queues](http://fideloper.com/ubuntu-beanstalkd-and-laravel4) by [Chris Fidao](http://fideloper.com/)  
[Laravel 4: Sending Emails](http://www.masnun.com/2013/07/13/laravel-4-sending-emails.html) by [Abu Ashraf Masnun](http://www.masnun.com/)  
[Simple and easy Laravel login authentication](http://scotch.io/bar-talk/x/simple-and-easy-laravel-authentication) by [Chris Sevilleja](http://www.sevilayha.com/)  
[Creating a Laravel App on AppFog](http://bwsewell.com/2013/07/11/creating_a_laravel_app_on_appfog.html) by [Brian Sewell](http://bwsewell.com/)  
[Image manipulation in Laravel 4 with Imagine](http://creolab.hr/2013/07/image-manipulation-in-laravel-4-with-imagine/) by [Boris Strahija](http://creolab.hr/)

### 유용한 패키지들(Packages)

[Arcadia CMS](https://github.com/ludo237/Arcadia-CMS) by [Claudio Ludovico](https://github.com/ludo237)  
[wkhtml2pdf](https://github.com/NitMedia/wkhtml2pdf) by [NitMedia](https://github.com/NitMedia)  
[Presenter](https://github.com/robclancy/presenter) by [Robert Clancy](https://github.com/robclancy)  
[Camelot-Auth](https://github.com/taftse/camelot-auth/) by [Timothy](https://github.com/taftse)  

### 기타링크(Other Links)

[Building a Decent API](http://philsturgeon.co.uk/blog/2013/07/building-a-decent-api) by [Phil Sturgeon](http://philsturgeon.co.uk/)  

## 이벤트(Events)

18/07 - Meeting - Austin, TX - [Welcome to Laravel Austin!](http://www.meetup.com/Laravel-Austin/)  
18/07 - Meeting - Washington, DC - [Meeting up for the first time](http://www.meetup.com/Capital-Laravel-Group/events/127827542/)  
25/07 - Meeting - Vienna - [Laravel Frameworkers Vienna](http://www.meetup.com/Laravel-Frameworkers-Vienna/)  
08/08 - Meeting - Fishers, IN - [Hang Out With Other PHP, Laravel, & Mobile App Devs](http://www.meetup.com/Laravel-Modern-Web-Apps-in-Carmel-Fishers-Indianapolis/events/128471462/)  
17/08 - Talk - Boston, MA - [Introduction to Laravel](http://www.northeastphp.org/talks/view/10/Introduction-to-Laravel)  
30/08 - 31/08 - Conference - Amsterdam - [Laracon EU 2013](http://laracon.eu/2013/)  