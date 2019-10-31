# act1

```
SceneSetup.act1();
```

(...300)

n: 그리고 이것은 인간의 불안감입니다

n: _당신_ 은 이 사람의 불안감입니다

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}

# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: 오! 또 온 거야?

`hong({eyes:"0_neutral"})`

n: 당신의 임무는 인간을 *위험* 으로부터 보호하는 것입니다

`bb({eyes:"look", mouth:"small_lock"})`

n: 사실은, 이 게임을 다시 시작하는 것만으로도 이미 *위험* 에 빠졌습니다

n: 어서, 주의를 주세요!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: 인간! 내 말을 들어, 우린 지금 위험해! 플레이어가...

[...다시 우릴 고문할거야!](#act1_replay_torture)

[...다른 엔딩을 찾지 못 할 거야!](#act1_replay_alternate)

[...해설적 충돌과 맞닥뜨릴 거야!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: 그는 우리를 울게 만들거야!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: 그는 우리를 공황 발작을 일으켜서 핸드폰을 부수게 할 거야!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: 그는 우리가 파티 주최자을 때리지 못하게 할거야!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: 그는 우리가 동정어리고 안티-빌런인 파티 주최자을 때리게 할 거야!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: 뭐, 최소한에 우리를 지붕에서 떨어트리진 않을 테니--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: 그는 우린 지붕에서 떨어지게 만들거야.
{{/if}}

`bb({body:"fear"});`

b: 이 모든 새로운 두려움들은 우리를 씁쓸하게 만들거야. 그러면 우리는--

(#act1_replay_end)

#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: 그래, *전반적으로* 이야기는 하나지만, 각 장마다 두 개의 엔딩이 있고 선택지에 따라서 대사도 달라지는ㄷ--

`bb({body:"fear"});`

b: 플레이어는 실망하고 이 창을 닫고, 프로그램을 지우고, 그러면 우리는--

(#act1_replay_end)

# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: 해설적 뭐?

`bb({eyes:"normal"});`

b: 이 이야기는 불안감과 건강한 관계를 유지하는 방법을 *선택* 할 수 있다는 주제를 가지고 있는데,

`bb({eyes:"normal_right"});`

b: 하지만 다시 시작하면 같은 이야기가 나오고, 결국 *선택* 은 중요하지 않다는 걸 알게 되고,

`bb({eyes:"narrow_eyebrow"});`

b: 이 게임이 전하고자 하는 메세지와 게임 자체의 모순이 탄로나버리면서,

`bb({eyes:"fear"});`

b: 이 이야기 속 세상의 정체도 드러나버리면,

`bb({body:"fear"});`

b: 그러면 우리는--

(#act1_replay_end)

# act1_replay_end

`bb({body:"panic"})`

b: 죽을거야아아아아아아아

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: 알았어. 원래의 캐릭터로 돌아와.

```
Game.clearText();
```

n4: (당신의 _불안감_ 이 어쩌구저쩌구 _당신_ 이 가장 불안해하는 것과 비슷하게 어쩌구저쩌구 뭐 해야 하는지 이미 아시죠?)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)

# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: 오 좋아, 내 늑대가 돌아왔네. 환상적인걸.

`hong({eyes:"0_neutral"})`

n: 당신의 임무는 인간을 *위험* 으로부터 보호하는 것입니다

`bb({eyes:"look", mouth:"small_lock"})`

n: 사실, 저 샌드위치가 인간을 *위험* 에 빠트리고 있군요

n: 어서 주의를 주세요!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: 인간! 내 말을 들어, 우린 지금 위험에 빠졌어! 뭐가 위험하냐면...

`bb({body:"squeeze"})`

n4: ( _당신_ 의 불안감이 게임을 플레이하게 두세요! _당신_ 이 불안해하는 것과 가장 비슷한 선택지를 고르세요)

(#act1_normal_choice)

# act1_normal_choice

[혼자서 점심을 먹고 있잖아! 또!](#act1a_alone) `bb({body:"squeeze_talk"})`

[우리는 먹는동안 뭘 할 수 없다고!](#act1a_productive) `bb({body:"squeeze_talk"})`

[저 '하얀 식빵'은 건강에 나빠!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: 너 외로움을 느끼면 담배를 하루에 15 개비를 피는 것만큼 일찍 죽을 수 있다는 사실 몰라?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: 음, 출처 밝혀준 건 고마운데--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: 내 말의 의미는 우리가 *지금 당장* 다른 사람과 어울리지 않으면 우리는-

`bb({body:"panic"})`

b: 죽을거야아아아아아아아

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: 당신은 *사랑받지 못함에 대한 공포* 를 사용했다.

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: 빨리 노트북 꺼내서 작업이라도 좀 해!

`hong({eyes:"0_annoyed"})`

h: 음, 키보드에 빵가루 흘리기는 싫은ㄷ--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 사회에 공헌하는 게 없으면 우린 사회의 기생충이나 다름 없어!

b: 사회단체는 사회운동가들을 죽이기 위해 사회의 의사에게 갈거고, 그러면 우리는--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 죽을거야아아아아아아아

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: 당신은 *나쁜 사람이 되는 것에 대한 공포* 를 사용했다.

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: 그 연구들은 검증된 거 맞--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 가공된 밀을 먹으면 혈당이 너무 높아져서 팔다리를 잘라야 할 거고, 그러면 우리는-

`bb({body:"panic"})`

b: 죽을거야아아아아아아아

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: 당신은 *상처받는 것에 대한 공포* 를 사용했다.

(#act1b)

# act1b

n: "효과가 굉장했다!"

`bb({mouth:"smile", eyes:"smile"});`

b: 봤지, 인간? 난 너를 지키는 충직한 늑대라구!

`bb({body:"pride_talk"});`

b: 네 감을 믿어! 네 감정은 항상 옳아!

`bb({body:"pride"});`

n: 인간의 HP를 0으로 만드세요.

n: 인간의 물리적인, 사회적인, 정신적인 건강을 보호하기 위해 당신은 다음 기술을 사용할 수 있습니다.

n: *상처받는 것에 대한 공포*, #harm#

n: *사랑받지 못함에 대한 공포*, #alone#

n: *나쁜 사람이 되는 것에 대한 *공포* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (꿀팁: 여러분들의 깊은 곳에 있는 두려움을 자극하는 선택지를 골라보세요!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: 내 폰이나 봐야겠다.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: 당신의 인간을 보호하십시오

n: 이 세상으로부터. 다른 사람들로부터. 자기 자신으로부터

n: 행운을 빕니다

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: 라운드 1: *FIGHT!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: 음. 페이스북에 이번 주 주말에 파티가 있다고 하네.

`bb({eyes:"uncertain"});`

b: 그 이상한 녀석은 주말*마다* 파티 열지 않아?

`bb({eyes:"uncertain_right"});`

b: 대체 어떤 공허함을 채우려고 하는 거지? 분명 심각하게 망가진 사람일 게 뻔해!

`hong({eyes:"surprise"});`

h: 게다가, 나 초대까지 받았는데?

`bb({eyes:"fear", mouth:"normal"});`

b: 그렇다면!

[간다고 해, 안 그러면 고독사할 거야!](#act1c_loner)

[안 간다고 해, 거긴 독극물 투성이라구!](#act1c_drugs)

[무시해, 우리가 가면 파티 분위기 망칠거야.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: 하루에 담배 15개비라니까, 인간! 15개비!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: 그러면 아무도 우리 장례식에 오지 않을 거고, 우리 유골은 바다에 마구 흩뿌려져 고래밥이 돼서,
{{/if}}

{{if !_.fifteencigs}}
b: 고래 똥이 될 거야! 
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: 그러니까, 우린 파티에 가야 해!
{{/if}}

{{if _.parasite}}
b: 단, 거기서 일할 수 있도록 노트북 꼭 챙겨 가. 사회의 기생충이 되면 안 되니까.
{{/if}}

{{if _.whitebread}}
b: 단, '하얀 식빵'을 대접하지 않는다면 말이야.
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: 쳇. 너만 입닫는다면야, 좋아.

h: 간다고 할게.

{{if _.whalepoop}}
b: 고래 똥이라니까, 인간! 고래 똥!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: 아님 더 최악인... '하얀 식빵'이 있겠지.
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: 너무 많은 필로폰이랑 '하얀 식빵'에 중독되서 화장터 화구에도 들어가지 못할 정도로 살찐 시체가 될 거야!
{{/if}}

{{if !_.whitebread}}
b: 온갖 약물에 중독돼서 장의사가 우릴 보고는 *벌써* 방부제 친 줄 알 거야!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: 게다가 파티를 즐길 수 없어. 우리는 일을 하지 않으면 우리는 끔찍한 사회의 기생충이 될거야!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: 쳇. 너만 입닫는다면야, 좋아.

h: 안 간다고 할게

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: 우리가 하는거라곤 하루에 담배 15개피를 피는것마냥 외로움때문에 구석에 찌그러져서 우는 것 뿐이잖아.
{{/if}}

{{if _.parasite}}
b: 우리가 파티에 가면 늘 하는거라곤 어떻게 해야 생산적인 사람이 될 지 걱정하는 거잖아.
{{/if}}

{{if _.whitebread}}
b: 우리가 가면 늘 하는거라곤 패스트푸드가 우릴 죽일 거라고 걱정하는 거잖아.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: 그러게, 왜 그럴까나.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: 파티 가도 다들 기분 나빠하고, 그렇다고 거절해도 다들 기분 나빠할걸!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: 뭘 하든 기분 나빠할 거니까, 그래서 우리도 기분이 나빠야만 해!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: 어휴. 너만 입닫는다면야, 좋아.

h: 그냥 무시할게.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: 어쨌든, 페이스북은 이쯤 할래. 좀 차분하고, 내 불안감을 줄여줄만한게 필요해.

`hong({eyes:"neutral"});`

h: 트위터엔 뭐 올라왔으려나?

`bb({eyes:"look"});`

[안 돼, 저 끔찍한 뉴스를 좀 봐!](#act1d_news)

[안 돼, 저 트윗 혹시 *우리*를 저격한 글 아니야?](#act1d_subtweet)

[오, 고양이가 우유 마시는 움짤이네](#act1d_milk)

# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: 세상에, 세상이 멸망하는 기분이 들어, 안그래?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: 마치 전부 끝장나고, 세상이 멸망하고 모든 것들이 죽어버리고 아무 것도 못 하는 채로 망하는 것처럼 말이야.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: 그 기사 리트윗하자!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 그래, 리트윗 할 테니까 제발 조용히 해!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: 에라이, 스냅챗이나 봐야지.

(#act1e)

# act1d_subtweet

`bb({eyes:"fear"});`

b: 저격트윗이네! 누구한테 하는진 안써있긴한데.. 교활하고, 엉큼한 저격글이야!

`hong({eyes:"annoyed"});`

h: 아마 아닐걸?

`bb({eyes:"narrow", mouth:"small"});`

b: 하지만 우리 뒷담화 하는 거면 어떡해

h: 그럴 일 없--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: 그것도 우리 바로 앞에서!

`hong({eyes:"sad", mouth:"sad"});`

h: 아니--

`bb({eyes:"narrow", mouth:"small"});`

b: 그치만 *만약 그러면*

h: 닥--

`bb({eyes:"narrow_eyebrow"});`

b: *또 몰라*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: 어.. 그래, 스냅챗이나 보자.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: 헤 완전 귀엽다, 이거 리트윗하자, 내 생각엔--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: 고양이는 우유를 소화 못 해. 이런 동물학대 영상을 보고 즐기다니, 우리는 끔찍한 사람이야.

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)

`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: 어.. 그래, 스냅챗이나 보자.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: 흠, 어젯밤에 올라온 사진이네. *저게*  매 주마다 여는 파티였구나.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: 윽, 내 불안감이 견디기엔 사람이 너무 많아.

h: 역시 간다고 하지 말 걸 그랬나?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[대답을 바꾸려고? 찐따처럼?!](#act1e_yes_dontchange)

[대답을 바꿔! 너무 붐벼!](#act1e_yes_changetono)

{{if _.subtweet}}
[음, 그 저격글 확실히 우리 얘기 맞네.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[잠깐, 팩트체크도 안 하고 리트윗했는데.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[근데 너, 지금 자세가 정말 안좋은건 알기나해?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 우리가 오길 기대하고 있을텐데, 그 믿음을 배신한다고? 혼자 죽고 싶어서 그래?!

{{if _.fifteencigs}}
b: 담배. 15개비.
{{/if}}

{{if _.whalepoop}}
b: 고래. 똥.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 조용이해, 제발! 그대로 간다고 할게!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: "사람의 쇄도"가 뭔지 몰라?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 2003년 로드아릴랜드 클럽에서 불이 났었는데, 겁에 질린 사람들이 출구에 너무 몰려서 100명의 사람들이 불에 타 죽었어-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 그런 게 우리한테 일어났으면 좋겠어?-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: 가지마 가지마 가지마 가지마 가지마 가지마 가지마 가지마 가ㅈ-

```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 알았어, 알았어! 안 간다고 하면되잖아! 제발!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: 흠... 정말 재밌어 보이는걸.

h: 역시 안 간다고 하지 말 걸 그랬나?

`bb({mouth:"normal", eyes:"normal"});`

[대답을 바꾸려고? 찐따처럼?!](#act1e_no_dontchange)

[대답을 바꿔! 혼자 죽지 마!](#act1e_no_changetoyes)

{{if _.subtweet}}
[음, 그 저격글 확실히 우리 얘기 맞네.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[잠깐, 팩트체크 안 하고 리트윗했는데.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[근데 너, 지금 자세가 정말 안좋은건 알기나해?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: 모두들 기대하고 있을 거야!

b: ...우리같이 {{if _.whitebread}}'하얀 식빵'이나 씹어먹는{{/if}} 역겹고 혐오스러운 사람들이 파티에 없을테니 정말 재밌는 파티를 즐길 수 있을--

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 조용이해, 제발! 안 간다고 하면 되잖아!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 지독한 외로움은 코르티솔 수치를 심혈관 질환이나 심장마비를 일으킬 수 있을 정도로 높여버리지!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: 담배. 15개비.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 조용이해, 제발! 간다고 하면 되잖아! 좀!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 우리가 리트윗한 문제있는 모든 트윗들이 전부 되돌아올 거야!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: 우린 밖으로 불려나와서는 말 안장에 밧줄로 꽁꽁 묶인 채, 초고속 정보통신망으로 질질 끌려가고 말겠지!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 대체 왜 그러는 거야?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 우리가 잘못 된 정보를 퍼트렸어! 자유로운 언론에 대한 신뢰를 박살내다니!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 우리 때문에 민주주의의 폐허에서 파시즘이 일어날 거야!!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: 대체 왜 그러는 거야?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 척추 구부려서 폴더폰처럼 접고다닐거야?! 핸드폰 볼 때 허리 좀 펴!

```
bb({body:"meta"});
```

b: 화면보고 있는 너도 마찬가지야.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: 대체 왜 그러는 거야?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: 흠... 정말 재밌어 보이는걸.

h: 역시 무시하지 말 걸 그랬나?

`bb({mouth:"normal", eyes:"normal"});`

[계속 무시해, 우린 여전히 분위기 깨는 사람들이야.](#act1e_ignore_continue)

[사실, 간다고 해.](#act1e_ignore_changetoyes)

[사실, 안 간다고 해.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: 그래도 계속 무시하는 건 좀 무례하지 않나, 안그래?

`bb({eyes:"normal_right"});`

b: 다른 사람들도 *우릴* 무시하는데, 뭐. 

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: 그냥 비긴 셈 치지 뭐.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: 나... 가서 놀게 허락해 주는 거야??

b: 뭐, 사실은, 외로우면 *죽을 수도* 있으니까.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: 사람들이 너무 붐빌거야. 분명 위험할거야.

(#act1e_yes_changetono)

# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: 어? '틴더' 알림왔네.

`bb({eyes:"uncertain"})`

b: 잠깐, 그 원나잇 어플??

`hong({eyes:"annoyed"})`

h: 원나잇 어플이라니. 이건 그냥 새로운 친구를 만나는--

`bb({eyes:"narrow"})`

b: 원나잇 맞잖아.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: 오, 나 매칭됐어! 얘 귀엽게 생겼네!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: 제발 이번엔 망치지 ㅁ-

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: 삐! 삐! 삐! 삐! 삐! 삐!

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[우린 다른 사람들에게 *이용*당할 거야](#act1f_used_by_others)

[우린 단지 다른 사람들을 *이용*하는 거야](#act1f_using_others)

[저 사람은 연쇄 살인마야](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: 모르는 사람과의 원나잇은 ^아랫도리^는 채울 수 있어도

b: 마음 속에 난 구멍은...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *못채워*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 중요한 건 우린 고독사로 죽을 거야!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: 설마 남의 ^성기^를 포켓몬처럼 수집하는 거 아니지?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (포켓몬스터 오프닝 테마곡)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ 난 세상에서 제일가는-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ 최고의 ^걸레^가 될 거야-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ 허벅지와 ^후장^, 풍만한 가슴-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ 그리고 축축한 ^좆^과 ^구슬^!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ 변태-몬! 전부 다 모-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 중요한 건 우린 영악한 자식이란 거야.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: 널 우물에 가두고 '하얀 식빵'만 먹여서 살찌운 다음, 네 피부를 양복처럼 입을지도 몰라!
{{/if}}

{{if _.parasite}}
b: 널 타이머 시계로 두들겨 패면서 이렇게 말할 거야 "생산적인 사람이 되어야지, 이 기생충아!"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: 네 몸으로 피투성이 색종이 조각을 만들고, 내장을 띠로 만들어 장식하고, 음료수에 네 피를 섞을 거야!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: 이런 파티 초대는 어때?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: 난 이 게임이 정말 지겨워.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"외로움은 우릴 죽일거야"... {{/if}}
{{if _.parasite}}"우린 사회의 기생충이야"... {{/if}}
{{if _.whitebread}}"'하얀 식빵'은 우릴 죽일거야"... {{/if}}
{{if _.subtweet}}"우리 뒷담화를 하고 있어"... {{/if}}
{{if _.badnews}}"세상이 멸망해"... {{/if}}
{{if _.hookuphole}}"고독사로 죽을 거야"... {{/if}}
{{if _.serialkiller}}"저 사람들은 연쇄살인마"... {{/if}}
{{if _.catmilk}}"고양이는 우유를 소화 못 해"... {{/if}}
{{if _.pokemon}}"게다가 ^씨발^같은 노래 패러디까지"... {{/if}}

h: 난 그냥 내 삶을 살고 싶어.

h: 이 모든 고통에서... 자유로워지고 싶다구.

`bb({eyes:"look_sad"});`

b: 저기... 인간...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: 괜찮을 거야.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: 네 충직한 늑대로서, 내가 언제나 위험 요소를 경계하고 안전하게 보호할게.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: 약속할게.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: 마지막 앱이네. 인스타그램. 넌 뭐 올라왔니?

`hong({eyes:"sad"});`

h: 이건... 또 파티 사진들이잖아.

`hong({mouth:"sad"});`

h: 모두 행복해보여. 걱정거리 없이, 불안감 없이.

`hong({mouth:"anger"});`

h: 난 왜 저 사람들처럼 못 하지? 왜 *평범하게* 살 수 없는 걸까?

`bb({eyes:"normal_right"});`

b: 파티 얘기 나와서 그런데, 이번 주말 파티 말야. 내 "최종" 결정은

`bb({eyes:"normal"});`

[우린 가야해.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[우린 가지말아야해.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: 가ㅈ--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^좆^.*

`hong({body:"2_you"});`

h: 까.

(...500)

b: ㅁ...

(...1500)

`bb({eyes:"wat_2"});`

b: 뭐?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: 난 파티 *간다고* 말할거야.

{{if _.act1g=="go"}}
h: 네가 가라고 해서가 아니라, *내가* 가고 싶어서야.
{{/if}}

{{if _.act1g=="dont"}}
h: 정확한 이유로는 "네가 가지 말라고" 하니까.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: 넌 날 통제할 수 "없어".

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: 그럼 실례. 이 ^염병할^ 장소에서 맛있는 샌드위치 먹을 거야.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[아우~~ 우린 다 죽을 거야](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[아우~~ 모두들 우릴 미워해](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[아우~~ 우린 못된 사람들이야](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: 아우~~ 우린 다 죽을 거야 아우~~~~~~

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: 아우~~ 모두들 우릴 미워해 아우~~~~~~

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: 아우~~ 우린 못된 사람들이야 아우~~~~~~

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: 축하합니다

(...500)

n: 당신은 성공적으로 인간을 물리적인, 사회적인, 정신적인 건강을 지켜냈습니다

n: 자, 저 고마워하는 거 보세요!

(...500)

n: 이제 HP가 0이 됐으니, 행동을 직접 선택할 수 있습니다.

`bb({mouth:"smile", eyes:"normal"});`

n: 야생의 "엔딩"이 튀어나왔다.

`bb({mouth:"small_lock", eyes:"fear"});`

n: *무엇을 할까?*

[{싸운다: 짜증나는 폰을 혼쭐내준다!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{도망간다: 몸을 공처럼 말고 흐느낀다!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: 네 폰 때문에 공황발작을 일으키고 있었어!

`bb({eyes:"anger"})`

b: 주커버그와 그 일당들이, 벤처 투자자들의 돈 때문에 네 정신 건강을 훔친 거야!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 폰을 혼내! 파괴해! 죽여버려!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: 이 세상은 전부 위험 투성이야!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 아르마딜로처럼 몸을 말아! 그리고 스스로를 지켜!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: 몸을 말고 울어 몸을 말고 울어 몸을 말고 울어 몸을 말고 울어 몸을 말고 울어 몸을 말고 울어 몸을 말고 울--

(#act1j)

# act1j

`SceneSetup.act1_outro()`
