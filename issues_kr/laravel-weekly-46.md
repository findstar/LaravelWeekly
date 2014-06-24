http://us7.campaign-archive2.com/?u=60fa14809d4de70a885daf382&id=70d54eea13

*이글은 [laravel weekly #46](http://us7.campaign-archive2.com/?u=60fa14809d4de70a885daf382&id=70d54eea13) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*

# Laravel Weekly #46

뉴스레터 #46에 오신것을 환영합니다! 지난주 Laracon은 어떠셨나요? 여러분들께서 컨퍼런스를 즐겁게 보내셨기를 바랍니다! 컨퍼런스는 매주 멋지게 마무리 되었습니다. 다행히 저는 내년에도 참석해서 여러분들을 만날수 있을것 같습니다.

대부분의 사람들이 뉴스를 확인하기 위해서 다양한 미디어 채널을 선호하고 있기 때문에 우리는 뉴스레터 뿐만 아니라 [페이스북 페이지와](https://www.facebook.com/laravelweekly) [구글+](https://plus.google.com/114030303943229111045) 페이지도 만들기로 하였습니다. 관련 페이지를 확인하시고 소셜 미디어 플랫폼을 통해서도 Laravel weekly를 즐겨주세요!

## 뉴스(News)

### Laracon

Laracon은 올해도 성공적으로 개최되었고 계속 성장하고 있습니다. 비록 제가 거기에 참석하지는 못했지만, 트위터를 통해서 본 모습들만 봐도 컨퍼런스가 성공적이었다는 것을 느낄 수 있었습니다. 각각의 세션은 성공적이었고, 많은 사람들이 서로 만나고 [셀카를 찍어 올리는 모습을](https://twitter.com/search?q=%23laraconselfie) 볼 수 있었습니다. 그리고 Taylor가 [Laravel Homestead](http://laravel.com/docs/homestead)와 [Laravel Forge](https://forge.laravel.com/)라는 멋진 기능들에 대한 발표가 있었습니다. 이렇게 즐겁고 성공적이며 매년 성장하는 컨퍼런스를 보고 있으니, 내년에는 저도 무조건 참석해야겠네요.

행사 이후 컨퍼런스에 참석한 사람들이 포스팅한 블로그들이 있습니다. 컨퍼런스 전경들을 확인해 보실 수 있구요, 참석하신 분들은 각각 발표자들의 세션을 투표하는 것을 잊지 말아주세요. 다음은 [Andrew Del Prete](https://github.com/Pathsofdesign)가 작성한 [Laracon에 대한 요약정리 gist](https://gist.github.com/Pathsofdesign/61cc8521231f652c9a67)입니다. 

다음은 Laracon EU입니다. 여전히 3개월 이상 남아있습니다만 시간이 모자랄지도 모릅니다. [여러분 서둘러 등록해 주세요](http://laracon.eu/2014/) :)

### Laravel Forge

지난주 Laracon 에서 공개한 가장 큰 화제는 의심할 여지없이 [Laravel Forge](https://forge.laravel.com/)였습니다. Laravel Forge를 사용하면 Digital Ocean, 아마존 AWS, Rackspace 그리고 Linode와 같은 Iaas 호스팅상에서 응용프로그램을 셋팅하는 수고를 덜어버릴 수 있습니다. 이보다 더 쉬울수는 없을것 같네요. 여러분의 코드를 Github에 올려놓는다면 자동으로 서버에 배포를 수행할 수 있습니다. Laravel Forge가 발표된 후 관련 기사를 제법 많이 모아두었습니다. 앞으로 계속 뉴스레터에 관련 소식을 실을 예정이니 뉴스레터 확인하는것을 잊지 말아주세요!

또한 관련하여 [David Hemphill](https://twitter.com/davidhemphill) 와 [Tanner Hearne](https://twitter.com/tannerhearne)가 만든 [ForgeRecipes](http://forgerecipes.com/) 사이트를 확인해 주세요.

Laracast에서도 관련 강좌를 시작했습니다. [이곳](https://laracasts.com/series/server-management-with-forge)에서 확인해 보세요.

### Laravel Homestead

Laracon을 통해서 릴리즈된 laravel 의 새로운 내용은 [Laravel Homestead입니다](http://laravel.com/docs/homestead?version=4.2). Homestead는 각각의 개인 프로젝트를 위한 vagrant 의 사전 패키지 입니다. 하나의 Vagrant 머신만 있으면 Laravel Homestead를 활용해 프로젝트가 동작 가능한 Vagrant를 손쉽게 구성할 수 있습니다. 

자세한 도움을 위해 이미 [Laracasts에](https://laracasts.com/lessons/introducing-laravel-homestead) 영상이 준비되어 있습니다.

### Laravel 4.1.29

Laravel 4.1.29 버전이 대량 할당으로부터(Mass assignments) 응용 프로그램을 보호 할 수 있도록 하는 인용 열(quoting column)에 대한 몇 가지 개선과 함께 릴리즈 되었습니다. [업그레이드 가이드를](http://laravel.com/docs/upgrade?version=4.1#upgrade-4.1.29) 통해서 상세한 내용을 확인할 수 있습니다.

### OctoberCMS 런칭

[OctoberCMS가](http://octobercms.com/) 드디어 공개되었습니다. OctoberCMS는 Laravel 기반으로 작성된 CMS 플랫폼입니다. 오픈소스로 공개되어 있으며 [Github에서](https://github.com/octobercms/october) 확인하실 수 있습니다. 

### Laravel 스톡홀름(Laravel Stockholm)

[Laravel Stockholm은](http://www.meetup.com/Laravel-Stockholm/) 새롭게 개설된 스웨덴 스톡홀름의 laravel 사용자 모임입니다. 이제 막 시작했지만 벌써 60명의 사람들이 가입을 했습니다. 스톡홀름에 거주하신다면 가입해보세요!

## 참고자료(Resources)

### 블로그 자료들(Articles)

[Getting your first site up and running in Laravel Forge](http://mattstauffer.co/blog/getting-your-first-site-up-and-running-in-laravel-forge)  
[Laravel Forge - Logging With Papertrail](http://mattstauffer.co/blog/laravel-forge-logging-with-papertrail)  
[Laravel Forge - Using Environment Variables for Environment Detection](http://mattstauffer.co/blog/laravel-forge-using-environment-variables-for-environment-detection)  
[IronMQ and Laravel: Setup](http://www.sitepoint.com/ironmq-laravel-setup/)  
[Breaking the Mold](http://daylerees.com/breaking-the-mold)  
[Setting the Environment Name in Laravel](http://www.slashnode.com/setting-environment-name-laravel/)  
[Impressions from the Laracon 2014](http://www.devfactory.ch/fr/node/111)  
[Protect or disable laravel artisan commands in production](http://www.chrisduell.com/blog/development/laravel/protecting-laravel-artisan-commands-production/)  
[Laracon – impressions, memories, takeaways](http://maxoffsky.com/maxoffsky-blog/laracon-impressions-memories-takeaways/)  
[Laracon 2014 – All Pros and No Cons](http://soapboxhq.com/blog/laracon-2014-all-pros-no-cons/)  
[Community - Just a longer “C” word](https://medium.com/laravel-stuff/8bab8b719d63)  
[Laracon NYC 2014 photos by Eric Barnes](https://www.facebook.com/media/set/?set=a.234788050053803.1073741828.214020072130601&type=3)  
[My Laracon Recap](http://laravel-news.com/2014/05/my-laracon-recap)  
[Self-Updating Composer in Production using Laravel Envoy](http://garrettstjohn.com/entry/self-updating-composer-using-laravel-envoy/)  

### 어플리케이션 & 패키지(Applications and Package)

[Storage Package for Laravel 4](https://github.com/dmyers/laravel-storage)  
[Laravel Offline Documentation](https://chrome.google.com/webstore/detail/laravel-offline-documenca/mhndfmojlokbeijmdjbclinoaefcnkpb)  
[Webhooks](https://github.com/florianbeer/webhooks)  
[Sanitizer Package](https://github.com/daylerees/sanitizer)  
[Laravel Excel](https://github.com/Maatwebsite/Laravel-Excel)  
[Intervention Image v2](http://image.intervention.io/)  
[Laravel the very basic auth filter](https://gist.github.com/PavelPolyakov/1084bd3e635a5ee146a7)  
[Snappy Concierge](http://besnappy.com/concierge)  
[Funny Face App](https://github.com/jeremeamia/FunnyFacesL4ExampleApp)  

### Laracasts

[Introducing Laravel Homestead](https://laracasts.com/lessons/introducing-laravel-homestead)  
[Special Edition: Laracasts Live](https://laracasts.com/lessons/laracasts-live)  
[Server Management With Forge](https://laracasts.com/series/server-management-with-forge)  

## 이벤트(Events)

**May 27, 2014 - San Francisco, CA**
[Inaugural Laravel SF Meetup!](http://www.meetup.com/LaravelSF/events/171330572/)

**June 5, 2014 - Fishers, IN**
[Laravel 4.2 Recap, Performance Tuning, Libraries](http://www.meetup.com/Laravel-Modern-Web-Apps-in-Carmel-Fishers-Indianapolis/events/181268002/)

**June 9, 2014 - Winnipeg, MB**
[Laravel 201 - Masters of the Laraverse](http://www.meetup.com/Winnipeg-PHP/events/183045462/)

**June 10, 2014 - Austin, TX**
[Laravel Austin - Meetup](http://www.meetup.com/Laravel-Austin/events/184373342/)

**June 10, 2014 - Berlin, Germany**
[Laravel Berlin Usergroup Meeting](http://www.meetup.com/laravel-berlin/events/183011902/)

**August 28, 29 & 30, 2014- Amsterdam, The Netherlands**
[Laracon EU](http://laracon.eu/2014/)