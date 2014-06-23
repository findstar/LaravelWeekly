http://us7.campaign-archive1.com/?u=60fa14809d4de70a885daf382&id=309f8659d6

*이글은 [laravel weekly #42](http://us7.campaign-archive1.com/?u=60fa14809d4de70a885daf382&id=309f8659d6) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*


#Laravel Weekly #42

몇주간 자리를 비웠었습니다. 잘 지내셨나요? Laracon US 티켓의 매진이 임박했습니다. 참가를 계획하셨던 분들은 서두르셔야 겠습니다. Laracon EU도 8월 28, 29, 30일에 있을 예정입니다. 잊지 마세요!

조만간 Laravel weekly에 변화를 계획하고 있습니다. 두어달 안에 보여드릴 수 있을것 같네요.

언제나 그렇듯이 읽어주셔서 감사합니다!

\- Dries
## 뉴스(News)

### Laracon EU 행사 일자가 발표되었습니다.(Laracon EU Dates Announced!)

다음 [Laracon EU](http://laracon.eu/2014/) 컨퍼런스 행사 일자가 확정되었습니다. 8월 28, 29, 30일에 걸쳐 진행될 예정입니다. 일정이외에 다른 내용은 전해진바가 없습니다만, 더 자세한 소식이 알려지는 대로 여러분께 전해드리겠습니다.

### Laracon US 티켓은 매진이 임박했습니다.(Laracon US Almost Sold Out)

Laracon US 티켓 판매가 거의 완료되어 갑니다. 이제 15장의 티켓만이 남아 있다고 하는데요. 참가를 계획하셨던 분들은 [서둘러서 구매해주세요](https://conference.laravel.com/)!

### Laravel Cashier

Laravel 4.2 버전 릴리즈가 다가오고 있습니다. Taylor는 최근 Laravel과 Cashier라는 통합되는 독립적인 실행형 패키지를 선보였습니다. [Cashier](https://github.com/laravel/cashier)는 여러분의 어플리케이션에 [Stripe](https://stripe.com/) 결제 서비스를 연결할 수 있는 손쉬운 방법을 제공합니다.

### PHPWomen 에서 Laracon 티켓을 증정합니다.(PHPWomen Laracon Ticket Giveaway)

[PHPWomen](http://phpwomen.org/)을 통해서 두장의 Laracon US 티켓을 구할 수 있습니다! 자세한 사항은 [이곳](https://docs.google.com/forms/d/1fvoAoJra55tLsPpRKyGZG0G6nmCJXImvE4wdBqgQ4y4/viewform)을 참고해주세요.

### Laravel 브라질(Laravel Brazil)

지난번 소식을 통해서 헝가리 Laravel 커뮤니티에 대해서 전해드렸었는데요. 이번주에는 브라질 Laravel 커뮤니티 소식을 전해드리게 되었습니다. [Laravel 브라질 커뮤니티](http://www.laravel.com.br/)는 놀라울 정도로 빠르게 성장하고 있다고 합니다. Laravel 브라질 커뮤니티에서는 정기적으로 관련 포스팅과 튜토리얼을 제공하고 있습니다. 또한 브라질 언어를 사용하는 사람들 사이에 여러 자료와 지원을 받을 수 있는 [포럼](http://forum.laravel.com.br/)도 운영하고 있습니다.

또한 [Brayan Rastelli](https://twitter.com/heybrayan)이 제공하는 브라질 언어로 된 [강좌](http://www.edukee.com/pt/curso/curso-imersao-laravel-4/sala-unica/1699276709)들을 확인해 보실 수 있습니다.

### Clivern의 Laravel 자료들(Laravel Articles by Clivern)

리소스 섹션을 통해서 많은 블로그 포스팅 자료들을 소개해 드렸었는데요. 이번에 소개하는 Clivern가 운영하는 [웹사이트](http://clivern.com/category/laravel/)는 꼭 확인해 보셔야 할것 같습니다. [ORM](http://clivern.com/laravel-orm-part1/)이나 [마이그레이션](http://clivern.com/laravel-migrations-part1/)과 같은 다양한 주제에 대한 블로그 포스팅 자료들이 많이 있습니다.

### InvoiceNinja

InvoiceNinja는 인보이스(청구서)를 발행하는데 사용할 수 있는 무료 서비스 입니다. 웹사이트는 Laravel을 기반으로 제작되었으며 사이트를 만드는데 사용한 소스코드를 [GitHub에서 내려받을 수 있습니다](https://github.com/hillelcoren/invoice-ninja/blob/master/LICENSE).

## 간단한 팁(Quick Tip)

이번주 팁은 [Laravel News](http://laravel-news.com/)에서 [firstOrFail 메소드 사용법](http://laravel-news.com/post/80173955034/laravel-firstorfail-forthewin)을 제공해 주었습니다.

## 참고자료(Resources)

### 블로그 자료들(Articles)

[Integrating Two-Factor Authentication with Clef](http://blog.enge.me/post/integrating-two-factor-authentication-with-clef)
[Integrating Remote Logout with Clef](http://blog.enge.me/post/integrating-remote-logout-with-clef)
[Revisionable now supports being used as a trait](http://www.chrisduell.com/blog/development/revisionable-now-supports-being-used-as-a-trait/)
[What To Return From Repositories](http://programmingarehard.com/2014/03/12/what-to-return-from-repositories.html)
[Decoupling your code in Laravel using Repositiories and Services](http://dfg.gd/blog/decoupling-your-code-in-laravel-using-repositiories-and-services)
[Extending The Connection Class In Laravel](http://blog.stidges.com/post/extending-the-connection-class-in-laravel)
[Getting Started With Laravel 4](https://medium.com/tech-reviews/f8881d2014c7)
[Implementing A Page View Counter In Laravel](http://blog.stidges.com/post/implementing-a-page-view-counter-in-laravel)
[Laravel Application Logs and Logrotate](http://thereluctantdeveloper.com/2014/03/laravel-application-logs-logrotate/)
[Proxies, Service Locators, Alias, Facades, and War](http://ryantablada.com/post/proxies-service-locators-alias-facades-and-war)

### 어플리케이션 & 패키지(Applications and Packages)

[Cruddy](https://github.com/lazychaser/cruddy)
[Firewall](https://github.com/antonioribeiro/firewall)
[Steroids](https://github.com/antonioribeiro/steroids)
[Rulez - Validation for Laravel](https://github.com/keevitaja/rulez-laravel)
[Laravel Automigrate](https://github.com/marlek/laravel-automigrate)
[Laravel DB Normalizer](https://github.com/stidges/laravel-db-normalizer)
[Laravel Validation Loader](https://github.com/fortrabbit/validator-loader)

### Laracasts

[Get Off MAMP...Now](https://laracasts.com/lessons/get-off-mamp-now)
[Fast Workflow With Generators](https://laracasts.com/lessons/fast-workflow-with-generators)
[Continuous Integration With Travis](https://laracasts.com/lessons/continuous-integration-with-travis)
[Subscriptions With Laravel and Stripe](https://laracasts.com/lessons/painless-subscriptions-with-laravel-and-stripe)
[Cache Tags and Memcached](https://laracasts.com/lessons/cache-tags-and-memcached)
[Laravel, PHPSpec, and Refactoring](https://laracasts.com/lessons/phpspec-laravel-and-refactoring)
[Package Dev Best Practices](https://laracasts.com/lessons/composer-package-development-best-practices)
[Bulk Email Notifications: Part 1](https://laracasts.com/lessons/bulk-email-notifications-part-1)
[Bulk Email Notifications: Part 2](https://laracasts.com/lessons/bulk-email-notifications-part-2)
[Efficient SQL Queries](https://laracasts.com/lessons/efficient-sql-queries)

### 기타 링크(Other Links)

[Hack](http://hacklang.org/)
[HHVM vs Zephir vs PHP: The showdown](http://simonholywell.com/post/2014/02/hhvm-vs-zephir-vs-php-the-showdown.html)
[Using Composer Without GitIgnoring Vendor/](http://www.lornajane.net/posts/2014/using-composer-without-gitignoring)

## 이벤트(Events)

**March 22, 2014 - Algarve, Portugal**
[Geek Sessions Lab: Laravel PHP Framework](https://www.facebook.com/events/221772971354788)

**May 15 & 16, 2014 - New York**
[Laracon US](https://conference.laravel.com/)

**August 28, 29 & 30, 2014 - Amsterdam, The Netherlands**
[Laracon EU](http://laracon.eu/2014/)