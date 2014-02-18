http://driesvints.com/blog/laravel-4-learnings-week-5

#Laravel 4 Learnings: week 5

*이글은 [weekly-laravel-weekly-5](http://driesvints.com/blog/laravel-4-learnings-week-5) 의 글을 번역한것입니다. 원 저작자인 dries vints 의 동의를 얻어 번역글을 게제합니다. 가급적 이해하는데 도움이 되도록 의역이 포함되어 있을 수 있습니다. 문맥이 매끄럽지 못한 부분은 번역주를 붙여두었습니다.*

 우와, 벌써 라라벨 위클리를 시작한지 5주나 지났나요? 시간이 참 빠르네요. 많은 분들이 보내주신 성원과 반응에 감사드리고 싶습니다.  다시한번 읽어주셔서 감사합니다. 라라벨 4에 대해서 어떤 좋은 블로그 글이나 패키지 또는 다른 어떤 소개할 만한 것을 알고 계신다면 제게 메일이나 멘션을 주세요, 그럼 다음주 포스트에 포함시키도록 하겠습니다. :)

##새로운 라라벨 4 스크린캐스트(New Laravel 4 Screencast)

 Taylor가 말하는 라라벨4 프레임워크에 새롭게 추가되는 기능들에 대한 [스크린캐스트](http://vimeo.com/63892510)가 올라왔습니다. 다음 링크에서 확인하세요.

http://vimeo.com/63892510


##Laracon EU: 발표제안(A Call For Talk Proposals)

[Laracon EU](http://laravel.io/topic/23/laracon-eu-a-call-for-talk-proposals)가 본격적으로 구체적인 움직임을 띄기 시작했습니다. [Shawn McCool](https://twitter.com/ShawnMcCool)가 최근에 진행한 설문조사는 좋은 반응들이 이어졌습니다. 그는 괜찮은 컨퍼런스가 될것이라고 자신했습니다. 컨퍼런스는 아마도 2013의 늦여름쯤에 개최될것 같다고 이야기 했습니다.

 Laracon EU가 시작되기 위해서 컨퍼런스의 발표자가 필요로 합니다. 만약 Laracon EU에서 발표를 진행하는 것에 관심이 있다면 [발표자 신청](https://heybigname.typeform.com/to/bY3H46)을 하실 수 있습니다.


##Laravel 4 기본 : JSON(Primer: JSON)

https://twitter.com/daylerees/status/323043035237740546

[Dayle Rees](https://twitter.com/daylerees) 가 "Code Bright" 책에 곧 추가될 챕터에 대해서 이야기했습니다. [관련 내용은 여기에서 볼 수 있습니다.!](http://daylerees.com/laravel-four-primer-json)


##HTTP Basic Auth

https://twitter.com/laravelphp/status/321290995155206145

HTTP 기본 인증을 구현하려 한다면 라라벨 4 코어에 있는 것보다 더 쉬울 수 없을 것입니다. 라우트에 대한 필터를 추가하면 브라우저에서 로그인을 위한 프롬프트 창을 보여줍니다. 사용자의 로그인과 인증을 라라벨에서 자동으로 처리합니다.

```
Route::get('basicauth', array('before' => 'auth.basic', function()
{
    return 'Logged in!';
}));
```

##에러 표시를 위한 "Whoops" 라이브러리 (Improved Error Display With The “Whoops” Library)

https://twitter.com/laravelphp/status/322416887680098304

 낡은 심포니 에러 화면을 대체하여 Whoops 라이브러리가 좀 더 향상된 에러 화면을 제공합니다.

##데이타베이스 테이블의 컬럼명 수정 지원(Support For Renaming Database Table Columns)

 라라벨4에서 데이타베이스 테이블의 컬럼명을 수정하는 기능이 추가되었습니다. 첫번째 파라미터는 원래의 이름, 그리고 두번재 파라미터는 새롭게 변경할 이름을 입력하면 됩니다.

```
Schema::table('addresses', function($table)
{
    $table->renameColumn('location', 'city');
});
```


##더 읽어볼만한 자료들(Resources)

- [Blade Syntax Highlighter for Sublime Text](https://github.com/Medalink/laravel-blade) by [Eric Percifiel](https://twitter.com/medalink7)
- [How To Contribute To Laravel](http://driesvints.com/blog/how-to-contribute-to-laravel-4/) 4 by myself
- [Using Dependency Injection and IoC in Laravel 4 controllers](http://www.nathandavison.com/posts/view/16/using-dependency-injection-and-ioc-in-laravel-4-controllers) by [Nathan Davison](http://www.nathandavison.com/)
- [A Bit Of Everything](http://niallobrien.me/2013/04/a-bit-of-everything/) by [Niall O’Brien](https://twitter.com/niall_obrien)
- [Quick tip on swapping Facades with Mocks when testing](https://gist.github.com/JeffreyWay/5348385) by [Jeffrey Way](https://twitter.com/jeffrey_way)


##스크린캐스트 자료(Screencasts)

- [Validation Services](https://tutsplus.com/lesson/validation-services/) by [Tutsplus](https://tutsplus.com/)
- [Validating With Models and Event Listeners](https://tutsplus.com/lesson/validating-with-models-and-event-listeners/) by [Tutsplus](https://tutsplus.com/)

##Meetups

- [Laravel Meetup Germany](http://meetup.laravel.de/) by [Franz Liedke](https://twitter.com/franzliedke)
- [Danish Laravel Meetup](http://forums.laravel.io/viewtopic.php?id=7497) by [Peter Suhm](https://twitter.com/petersuhm)

##유용한 패키지(Packages)

- v1.0 of [Revisionable](https://github.com/VentureCraft/revisionable) by [Chris Duell](https://github.com/VentureCraft/revisionable) is now released


*원 글은 다음 링크에서 확인하실 수 있습니다. [Original Link](http://driesvints.com/blog/laravel-4-learnings-week-5)*


*오역이나, 기타 문법, 문맥적으로 매끄럽지 못한 부분에 대한 사항은 [@findstar](https://twitter.com/findstar) 이나 뎃글 주시면 수정하겠습니다.*


*원글에 대한 저작권한은 [@driesvints](https://twitter.com/driesvints) 에게 있습니다.*