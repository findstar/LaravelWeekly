http://us7.campaign-archive2.com/?u=60fa14809d4de70a885daf382&id=c4862519b5

*이글은 [laravel weekly #21](http://us7.campaign-archive2.com/?u=60fa14809d4de70a885daf382&id=c4862519b5) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*

# Laravel Weekly #21

드디어 첫번째 Laravel weekly 뉴스레터입니다! 이제부터 매주 Laravel 뉴스를 메일로 받아 볼 수 있습니다! 이미 뉴스 레터의 구독을 신청해주신 분들께 감사합니다. 벌써 195명 이상이 Laravel 뉴스를 구독신청하였습니다.

누구나 이 뉴스레터를 구독할 수 있습니다. 만약 여러분이 뉴스레터를 통해서 공유하고자 하는 것이 있다면 언제든지 알려주세요! 여러분이 알고 있는 유용한 패키지들, 기사글들, 튜토리얼들 그리고 스크린캐스트 자료들을 링크와 함께 [hello@laravelweekly.com](mailto:hello@laravelweekly.com)로 보내주세요. 그러면 그 다음주차에 내용을 실을 수 있도록 하겠습니다.

 뉴스레터에서 뭔가 잘못된 것들을 발견하게 된다면 우리에게 알려주세요. 버그 리포트들은  [hello@laravelweekly.com](mailto:hello@laravelweekly.com)로 보내 주시면 됩니다.

아직 구독 신청을 하지 않으셨다면 [이곳](http://eepurl.com/DGabL)을 통해서 진행할 수 있습니다.

다음주에 만나요!

## 뉴스(News)

### Laracon EU가 다음주로 다가왔습니다.(Laracon EU is next week!)

[Laracon EU](http://laracon.eu/2013/)가 이제 일주일 밖게 남지 않았습니다!
행사가 열리는 한주 동안 200명 이상의 Laravel 개발자들이 암스테르담에 모이고 그중에서 가장 유명한 사람들의 세션들을 들을 수 있습니다. 정말 신납니다!

 지금까지도 티켓을 구매하지 않았다면 아직 약간의 시간이 남아 있습니다! 아직 당신이 망설이고 있다면 좋은 소식 하나를 알려드리겠습니다. [Cartalyst (http://www.cartalyst.com/) 에서 남아 있는 Laracon EU 티켓 30장을 구매하면 자신들의 서비스를 60% 할인된 금액에 제공해주겠다고 공지하였습니다.(http://www.cartalyst.com/pricing). 저렴한 가격으로 프리미엄 컴포넌트를 얻을 수 있는 기회입니다. 
 (번역주 : cartalyst 는 프리미엄 laravel 컴포넌트를 서비스 하는 업체 입니다. 이 서비스는 분기별(3개월) 별로 갱신하는 형태로 되어 있는데 남은 30장의 티켓 구매자에게는 이 3개월 서비스를 60%할인된 금액에 제공해 주겠다는 이야기 입니다.))
 
 그리고 한가지 더 Laracon EU에 참석한 사람들에게는 [Taylor의 최근 서적](https://twitter.com/laravelphp/status/367498147884318720), "From Apprentice to Artisan"의 무료 카피본을 나눠준다고 합니다. 
 (번역주 : From Apprentice to Artisan은 ebook로 출간하였습니다.)

### 세번째 팟캐스트 - 패키지(Podcast #3 - Packages!)

놓치신 분들을 위해 알려드립니다. 지난주 [laravel.io](http://laravel.io/) 에 [세번째 Laravel 팟캐스트](http://laravel.io/topic/44/podcast-3-packages)가 업로드 되었습니다. 이번 에피소드에서는, [Taylor Otwell](https://twitter.com/taylorotwell)과 그의 동료 backbone-ninja [Eric Barnes](https://twitter.com/ericlbarnes), 그리고 Laravel 커뮤니티의 컨트리뷰터인 [Ryan Tablada](https://twitter.com/RyanTablada)이 출연하여 패키지에 대해서 이야기를 진행하였습니다.

### Laravel 4 인증(Laravel 4 Authentication)

[Christopher Pitt](https://twitter.com/followchrisp) 가 [Laravel 4에서의 인증](https://medium.com/on-coding/e8d93c9ce0e2)에 대해서 심도 있는 튜토리얼을 작성했습니다. 이 튜토리얼을 읽어 보시면 사용자 인증, 암호 재설정 및 오류 처리와 같은 인증과 관련된 모든 일을 구현하는 프로그램을 설정하는 데 도움이 될 것입니다.

### Implementing Laravel

Laravel 커뮤니티에 주요 멤버인 [Chris Fidao](https://twitter.com/fideloper)가 최근 Laravel로 어플리케이션을 구현하는 방법에 대한 [새로운 Laravel 서적](https://leanpub.com/implementinglaravel)을 작업중에 있습니다. 저는 아주 많이 기대하고 있습니다!

### Cartalyst 팀 계정 기능 런칭

프리미엄 Laravel 4 패키지와 어플리케이션을 제공하는 [Cartalyst](http://www.cartalyst.com/)에서 새롭게 [팀 계정 기능](http://blog.cartalyst.com/post/58245326721/team-accounts-pricing)도 제공하기로 했습니다.

## 간단한 팁(Quick Tip)

인스턴스화된 컬렉션의 값들을 "implode" 메소드를 통해서 이어 붙일 수 있다는 걸 알고 계신가요? 또는 여러 아이템들 중에 원하는 첫번째 또는 마지막 x 번째의 값을 "take" 메소드를 통해서 확인할 수 있다는 걸 알고 계신가요? [여기](http://paste.laravel.com/Li1) 예제 샘플을 확인할 수 있습니다.

## 참고자료들(Resources)

### 기사글모음(Articles)

[Laravel 4 and Facebook PHP SDK](http://ifonlyiknewthat.com/facebook/laravel-4-and-facebook-php-sdk/)  
[Permissions, Virtual Hosts, and Laravel](http://jasonlewis.me/article/permissions-virtual-hosts-and-laravel)  
[Platform 2 Extensions - Quick Start guide](https://gist.github.com/drsii/6295234)  
[Cool Stuff I Learned About Laravel 4](http://antjanus.com/blog/web-development-tutorials/cool-stuff-i-learned-about-laravel-4/)  
[Snippetize All The Things](http://laracasts.com/blog/snippetize-all-the-things)  
[Alternative Environment Detection for Laravel 4](http://crynobone.com/posts/5/alternative-environment-detection-for-laravel-4)  
[Integrating Facebook Login into Laravel application](http://maxoffsky.com/code-blog/integrating-facebook-login-into-laravel-application/)  
[Eloquent Connections - Making the World Go Round](http://ryantablada.com/post/eloquent-connections-making-the-world-go-round)  
[Ember JS and Laravel](http://ryantablada.com/post/ember-js-and-laravel)  
[What and Why - Query Builders and Eloquent](http://ryantablada.com/post/what-and-why-query-builders-and-eloquent)  
[Laravel 4 in Shared Hosting](http://crynobone.com/posts/3/laravel-4-in-shared-hosting)  

### 유용한 패키지(Packages)

[Stapler - Easy file attachment management using Eloquent in Laravel 4](https://github.com/CodeSleeve/stapler)  
[Aidkit - The "Admin Interface Development Kit" for Laravel](http://codebryo.github.io/aidkit/)  
[Asset Pipeline](https://github.com/CodeSleeve/asset-pipeline)  
[Laravel Berkshelf Bootstrap](https://github.com/In-Touch/laravel-berkshelf)  

### 스크린캐스트(Screencasts)

[Laravel Tutorial 2 - Controller, View and Pass Data](http://www.youtube.com/watch?v=U_0gNBN7Q7I)  
[Building Laracasts Teaser](http://laracasts.com/blog/building-laracasts-teaser-1)  
[Migrations and Icon fonts](http://social-sharing.s3.amazonaws.com/20-Storing-Thumbnail-References-Within-The-Database.mp4)  
[Helper Functions](http://social-sharing.s3.amazonaws.com/14-Helper-Functions.mp4)  

### 발표자료(Talks)

[Laravel 4 소개 - Intro to Laravel 4](http://www.slideshare.net/kareerme/laravel-sdphp)

### 기타 링크(Other Links)

[Vim Adventures](http://vim-adventures.com/)

### 이벤트(Events)

30/08 - 31/08 - Conference - Amsterdam - [Laracon EU 2013](http://laracon.eu)  
12/09 - Meeting - Fishers, IN - [Discuss Modern Web & Mobile Development, & Laravel 4's Progress](http://www.meetup.com/Laravel-Modern-Web-Apps-in-Carmel-Fishers-Indianapolis/events/135898802/)

## 참여를 기다립니다(We want you...)!

 알고 계시는 자료들, 패키지, 모임소식, 스크린캐스트등 다음주 weekly에 추가될만한 그 어떤 것이라도 이메일로 보내주세요. [hello@laravelweekly.com](mailto:hello@laravelweekly.com)