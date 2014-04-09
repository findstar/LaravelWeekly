http://driesvints.com/blog/laravel-weekly-8

*이글은 [laravel weekly 8](http://driesvints.com/blog/laravel-weekly-8) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*

# Laravel Weekly #8

 weekly 의 이름을 다시 한번 변경했습니다. 이번이 마지막이 될 수 있을까요? 아마 그렇지는 않을것 같네요.

 이제부터는 이 포스트를 트위터에 #laravelweekly 해쉬태그와 함께 트윗할 예정입니다. 또한 앞으로 이 포스트에 대한 몇몇 아이디어를 가지고 있습니다. 지켜봐 주시기 바랍니다 :)

 만약 당신의 좋은 자료들, 패키지, 기사와 이름이 소개되기를 바란다면 트위터에서 제게 멘션을 주거나 이메일을 보내주세요.

## StackExchange 제안에 무슨일이 있었나요?(What Happened To The StackExchange Proposal?)

 간단하게 이야기 하자면 [제안은 거부되었습니다.](http://discuss.area51.stackexchange.com/questions/10046/no-really-what-part-of-this-isnt-already-on-topic-for-stack-overflow). [Stack Exchange](http://stackexchange.com/) 관리자들은 Laravel 에 대해 별도의 사이트기 필요하다고 느끼지 않았으며 StackOverflow에 이미 우리가 사용할 수 있는 플랫폼을 제공하고 있다고 지적했습니다.

 지금 이 일이 나쁜것은 아닙니다. 그들이 말해주었 듯이 우리는 여전히 좋은 질문을 할 수 있는 플랫폼인 StackOverFlow를 사용할 수 있습니다. #laravel 태그와 함께 질문을 올리세요. 별도의 Laravel 플랫폼이 되지는 않더라도 기본적으로 이 것은 여전히 같은 효과를 나타냅니다.

 도움을 주신 여러분들의 투표에 정말 감사드립니다.

## Laravel 소셜 그룹(Laravel Social Groups)

 Laravel 을 위한 몇몇 소셜그룹들이 존재합니다. 여기에 링크를 정리하였습니다:

- [Facebook](https://www.facebook.com/groups/LaravelCommunity/)
- [Google+](https://plus.google.com/communities/106838454910116161868)
- [LinkedIn](http://www.linkedin.com/groups/Laravel-PHP-Framework-4419933)
- [Reddit](http://www.reddit.com/r/laravel/)

## Laravel 4: 작업중 모드(Maintenance Mode)

https://twitter.com/laravelphp/status/330080201084121088

 이 기능은 최근 Laravel 4 베타 5버전에 추가된 기능으로 Artisan 커맨드를 통해서 어플리케이션이 작업중 모드로 설정할 수 있게 합니다. 이 기능은 사용자들의 이용을 차단하고 그 동안 사이트를 업그레이드하거나 프로그램을 수정 할 수 있도록 합니다.

## Laravel 4: 소프트삭제(Soft Delete)

https://twitter.com/laravelphp/status/330328333332127745

 레코드를 소프트 삭제 하면 실제로 데이터베이스 에서 제거하지 않고 레코드를 삭제 하는 것을 의미합니다. 이것은 당신이 레코드를 삭제함으로써 잃고 싶지 않은 정의 관계가 많은 경우에 유용 할 수 있습니다.

 소프트 삭제에 대해서 좀 더 많은 내용을 메뉴얼을 통해서 확인 할 수 있습니다. [the Laravel 4 docs](http://four.laravel.com/docs/eloquent#soft-deleting).

## Laravel 4: 하위 폴더에서의 컨트롤러 생성(Generate Controllers In Subdirs)

https://twitter.com/jeffrey_way/status/330347895742160897

 이제 Artisan을 통해서 컨트롤러를 생성할 때, 컨트롤러 앞에 하위 폴더나 네임스페이스를 표시함으로써 해당 하위 디렉토리에 컨트롤러를 생성할 수 있습니다. 네임 스페이스를 명시 할 경우, 네임 스페이스는 파일에 자동으로 추가됩니다.

##더 읽어볼만한 자료들(Resources)

- [Global site messages in Laravel 4](http://toddish.co.uk/blog/global-site-messages-in-laravel-4/) by [Todd Francis](https://twitter.com/toddish)
- [Custom Artisan Commands And You](https://tutsplus.com/course/custom-artisan-commands-and-you/) by [Tutsplus](https://tutsplus.com) (Partialy Paid) 
- [Laravel 4 Quick Tip: Custom Error Pages](http://driesvints.com/blog/laravel-4-quick-tip-custom-error-pages/) by [Myself](https://twitter.com/driesvints)
- [Laravel 4 + IronMQ Push Queues = Insane Goodness](http://blog.iron.io/2013/05/laravel-4-ironmq-push-queues-insane.html) by [IronMQ](http://www.iron.io/)

## 유용한 패키지 Packages

- [Basset 4.0 (pre-beta)](http://jasonlewis.me/code/basset/4.0) by [Jason Lewis](https://twitter.com/jasonclewis)
- [Handling Proxies in Laravel 4](http://fideloper.com/laravel-4-trusted-proxies) by [Chris Fidao](https://twitter.com/fideloper)
- [Laravel Test Helpers (Beta)](https://github.com/JeffreyWay/Laravel-Test-Helpers) by [Jeffrey Way](https://twitter.com/jeffrey_way)
- [Laravel Breadcrumbs](https://github.com/davejamesmiller/laravel-breadcrumbs) by [Dave James Miller](https://twitter.com/DaveJamesMiller)
- [Async Database Logs for Laravel 4](https://github.com/conradkleinespel/database-log-laravel4) by [Conrad Kleinespel](https://twitter.com/conradktweets)

*원 글은 다음 링크에서 확인하실 수 있습니다. [Original Link](http://driesvints.com/blog/laravel-weekly-8)*


*오역이나, 기타 문법, 문맥적으로 매끄럽지 못한 부분에 대한 사항은 [@findstar](https://twitter.com/findstar) 이나 뎃글 주시면 수정하겠습니다.*


*원글에 대한 저작권한은 [@driesvints](https://twitter.com/driesvints) 에게 있습니다.*