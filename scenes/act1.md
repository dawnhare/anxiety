# act1

```
SceneSetup.act1();
```

(...300)

n: 그리고 이것은 인간의 불안감입니다

n: _당신_ 이 사람의 불안감입니다

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

n: 사실, 이 게임을 다시 시작하는 것만으로도 이미 당신의 인간은 *위험* 에 빠졌습니다

n: 빨리, 주의를 주세요!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: 인간! 내 말을 들어, 우린 지금 위험해! 플레이어가...

[...다시 우리를 고문시킬 거야!](#act1_replay_torture)

[...다른 엔딩을 찾지 못 할 거야!](#act1_replay_alternate)

[...해설적 충돌과 맞닥뜨릴 거야!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: 플레이어는 우리를 울게 만들 거야!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: 플레이어는 우리가 공황 발작을 일으켜서 핸드폰을 부수게 할 거야!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: 플레이어는 우리가 파티 호스트를 때리지 *못하게* 할 거야!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: 플레이어는 우리가 동정어리고 정의로운 파티 호스트를 때리게 할 거야!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: 뭐 최소한에 우리를 지붕에서 떨어트리진 않을 테니--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: 우린 지붕에서 떨어질 거야.
{{/if}}

`bb({body:"fear"});`

b: 이 모든 새로운 끔찍한 일들이 우리한테 일어나고 나면--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: 그래, *전반적으로* 이야기는 하나지만, 각 장마다 두 개의 엔딩이 있고 선택지에 따라서 대사도 달라지는ㄷ--
`bb({body:"fear"});`

b: 플레이어는 실망하고 이 브라우저 탭을 닫고, 프로그램을 지우고, 그러면 우리는--

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

b: 게임을 다시 플레이하고 같은 이야기가 나오면 결국 *선택* 은 중요하지 않다는 걸 알게 되고,

`bb({eyes:"narrow_eyebrow"});`

b: 이 게임이 전하고자 하는 내용과 게임 자체의 모순이 탄로나버리면서,

`bb({eyes:"fear"});`

b: 이 이야기 속 세상의 정체도 드러나버리면,

`bb({body:"fear"});`

b: 우리는--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: 죽을 거야아아아아아아아

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

h: 그래 그럼 다시 분위기 잡자.

```
Game.clearText();
```

n4: (당신의 _불안감_ 이 어쩌구 _당신_ 이 가장 불안해하는 것과 비슷하게 저쩌구 뭐 해야 하는지 이미 아시죠?)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: 아, 그래. 내 늑대가 돌아왔네. 아이고 좋아라.

`hong({eyes:"0_neutral"})`

n: 당신의 임무는 인간을 *위험* 으로부터 보호하는 것입니다

`bb({eyes:"look", mouth:"small_lock"})`

n: 지금 저 샌드위치가 인간을 *위험* 에 빠트리고 있군요

n: 빨리, 주의를 주세요!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: 인간! 내 말을 들어, 우린 지금 위험에 빠졌어!

`bb({body:"squeeze"})`

n4: (_당신_ 의 불안감이 게임을 플레이하게 두세요! _당신_ 이 불안해하는 것과 제일 비슷한 선택지를 고르세요)

(#act1_normal_choice)

# act1_normal_choice

[혼자서 점심을 먹고 있잖아! 또!](#act1a_alone) `bb({body:"squeeze_talk"})`

[밥을 먹는 동안 시간이 낭비되고 있어!](#act1a_productive) `bb({body:"squeeze_talk"})`

[저 흰 식빵은 건강에 나빠!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: 너 외로움을 느끼면 담배를 하루에 15 개비를 피는 것만큼 일찍 죽을 수 있다는 사실 몰라?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (출처: Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: 아, 출처 밝혀준 건 고마운데--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: 우리가 *지금 당장* 다른 사람과 어울리지 않으면 우리는-

`bb({body:"panic"})`

b: 죽을 거야아아아아아아아

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: 당신은 *사랑받지 않음에 대한 공포* 를 사용했습니다

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: 빨리 노트북 꺼내서 작업이라도 조금 해!

`hong({eyes:"0_annoyed"})`

h: 아, 키보드에 빵가루 흘리기는 싫은ㄷ--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 사회에 공헌하는 게 없으면 우린 사회의 기생충이나 다름 없어!

b: 사회가 사회 병원으로 가서 사회의 기생충들을 죽이는 구충제를 받게 되면 우리는--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 죽을 거야아아아아아아아

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: 당신은 *나쁜 사람이 되는 것에 대한 공포* 를 사용했습니다

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: 그 연구 검증된 거 맞--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 가공된 밀을 먹으면 혈당이 너무 높아져서 팔다리를 잘라야 할 거고 그렇게 되면 우리는-

`bb({body:"panic"})`

b: 죽을 거야아아아아아아아

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: 당신은 *해를 입는 것에 대한 공포* 를 사용했습니다

(#act1b)

# act1b

n: 매우 효과적입니다

`bb({mouth:"smile", eyes:"smile"});`

b: 봤지? 난 너를 지키는 충직한 늑대라고!

`bb({body:"pride_talk"});`

b: 네 감을 믿어! 네 감정은 항상 옳아!

`bb({body:"pride"});`

n: 인간의 에너지를 0 까지 내리십시오

n: 인간의 물리적 + 사회적 + 정신적 건강을 보호하기 위해 당신은:

n: *해를 입는 것*에 대한 공포, #harm#

n: *사랑받지 않음*에 대한 공포, #alone#

n: *나쁜 사람이 되는 것*에 대한 공포를 사용할 수 있습니다 #bad#

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

n: 라운드 1: *파이트!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: 흠. 이번 주 주말에 파티가 있다고 페북에 뜨네.

`bb({eyes:"uncertain"});`

b: 그 이상한 녀석은 *매 주* 마다 파티 열지 않아?

`bb({eyes:"uncertain_right"});`

b: 대체 그 인간은 어떤 공허함을 채우려고 하는 거지? 심각하게 망가진 사람일 게 뻔해!

`hong({eyes:"surprise"});`

h: 나 초대까지 받았는데?

`bb({eyes:"fear", mouth:"normal"});`

b: 그럼 답이 나왔네!

[간다고 해, 안 그러면 고독사할 거야!](#act1c_loner)


[안 간다고 해, 거긴 독극물 투성이라구!](#act1c_drugs)


[무시해, 우리가 가면 분위기 망칠 거야.](#act1c_sad)


# act1c_loner

{{if _.fifteencigs}}
b: 담배 15개비라니까, 인간! 15개비!

{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: 그러면 아무도 우리 장례식에 오지 않을 거고, 우리 유골은 바다에 마구 흩뿌려져 고래밥이 되고

{{/if}}

{{if !_.fifteencigs}}
b:고래 똥이 될 거야! 

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
b: 단, 사회의 기생충이 되면 안 되니까 거기서 일할 수 있도록 노트북 꼭 챙겨 가.

{{/if}}

{{if _.whitebread}}
b: 단, 흰 식빵만 없다면 말야.

{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: 쳇. 조용히 한다면야, 좋아.


h: 간다고 할게.


{{if _.whalepoop}}
b: 고래 똥이라니까, 인간! 고래 똥!

{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: 아님 더 나쁜...흰 식빵이 있겠지

{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: 메스암페타인이랑 흰 식빵에 너무 중독되서 화장터 화구에도 들어가지 못할 정도로 살찐 시체가 될 거야!

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
b: 끔찍한 기생충이 되기 싫으면 파티 대신 일을 해야지! 

{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: 쳇. 조용히 한다면야, 좋아.


h: 안 간다고 할게


`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: 우리 파티 가면 늘 외로움은 하루에 담배 15개비 피는 것만큼 치명적이라고 걱정만 하잖아.

{{/if}}

{{if _.parasite}}
b: 우리 파티 가면 늘 어떻게 해야 생산적인 사람이 될 지 걱정만 하잖아.

{{/if}}

{{if _.whitebread}}
b: 우리 파티 가면 늘 정크 푸드가 우릴 죽일 거라고 걱정만 하잖아.

{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: 으, 왜 그럴까


`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: 파티 가도 다들 기분 나빠하고, 그렇다고 거절해도 다들 기분 나빠할걸!


`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: 뭘 하든 기분 나빠할 거니까 우리도 기분 나빠야 해!


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: 어휴. 조용히 한다면야, 좋아.


h: 그냥 무시할게.


`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: 그나저나, 페이스북은 너무 과해. 차분하고, 내 불안감을 줄여주는 게 필요해


`hong({eyes:"neutral"});`

h: 트위터에 뭐 올라왔나?


`bb({eyes:"look"});`

[안 돼, 저 끔찍한 뉴스를 좀 봐!](#act1d_news)


[안 돼, 저 트윗 혹시 *우리*를 저격한 글 아니야?](#act1d_subtweet)


[봐봐, 고양이가 우유를 마시는 영상이네](#act1d_milk)



# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: 세상이 멸망하는 기분이 들어, 그치?


```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: 마치 전부 끝장나고 세상이 멸망하고 모든 것들이 죽어버리고 아무 것도 못 하는 채로 망하는 것처럼 말이야

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

h: 에라이, 스냅챗이나 봐야지


(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: 서브트윗이네! 교활하고, 엉큼한 서브트윗!


`hong({eyes:"annoyed"});`

h: 아마 아닐걸?


`bb({eyes:"narrow", mouth:"small"});`

b: 하지만 우리 뒷담화 하는 거면 어떡해


h: 그럴 일 없--


`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: 그것도 우리 바로 뒤에서!


`hong({eyes:"sad", mouth:"sad"});`

h: 아니--


`bb({eyes:"narrow", mouth:"small"});`

b: 그치만 *만약 그러면*


h: ㅈ--


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

h: 그, 그럼 스냅챗이나 보자.


(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: 헤헤, 그러네, 귀엽다, 리트윗을 해--


```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: 고양이는 우유를 소화 못 해 이런 학대 영상을 보고 즐기다니 우리는 끔찍한 사람이야

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

h: 그-럼, 스냅챗이나 보자.


(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: 흠, 어젯밤에 올라온 사진이네. *저게* 주마다 열리는 파티였구나.


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


[대답을 바꿔야지! 너무 많아!](#act1e_yes_changetono)


{{if _.subtweet}}
[역시 저 서브트윗은 우리 저격이었어.](#act1e_ignore_subtweet)

{{/if}}

{{if _.badnews}}
[잠깐, 팩트체크 안 하고 리트윗했는데.](#act1e_ignore_factcheck)

{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[근데 너, 자세 정말 안 좋은 거 알아?](#act1e_ignore_posture)

{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 우리가 오길 기대하고 있을 텐데 그 믿음을 배신한다고? 혼자 죽고 싶어서 그래?!


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

h: 알았어, 알았어! 그대로 간다고 할게!


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

b: 2003년 로드아릴랜드 나이트클럽에서 불이 났었는데, 겁에 질린 사람들이 출구에 너무 몰려서 100명의 사람들이 불에 타 죽었어


```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 그 사건이 우리에게 일어났으면 좋겠니?

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

h: 알았어, 알았어! 안 간다고 바꾸면 되잖아! 좀!


(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: 흠...정말 재밌어 보이는걸.


h: 역시 안 간다고 하지 말 걸 그랬나?


`bb({mouth:"normal", eyes:"normal"});`

[대답을 바꾸려고? 찐따처럼?!](#act1e_no_dontchange)


[대답을 바꿔! 혼자 죽지 마!](#act1e_no_changetoyes)


{{if _.subtweet}}
[음, 확실히 우리 얘기 맞네](#act1e_ignore_subtweet)

{{/if}}

{{if _.badnews}}
[잠깐, 팩트체크 안 하고 리트윗했는데.](#act1e_ignore_factcheck)

{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[근데 너, 자세 정말 안 좋은 거 알아?](#act1e_ignore_posture)

{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: 모두들 기대하고 있을 거야!


b: 우리같이 {{if _.whitebread}}빵이나 씹어먹는 {{/if}}역겹고 혐오스러운 사람들이 파티에 안 가니까 정말 재밌는 파티를 즐길 수 있을 --



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

h: 알았어, 알았어! 안 간다고 하면 되잖아!


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

h: 알았어, 알았어! 간다고 하면 되잖아! 좀!


(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 우리가 쓴 심각한 트윗들이 전부 되돌아올 거야!


```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: 우린 밖으로 불려나와서는 말 안장에 밧줄로 꽁꽁 묶인 채 초고속 정보통신망으로 질질 끌려가고 말겠지!

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
//Why are you like this?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 우리가 잘못 된 정보를 퍼트렸어! 자유 언론에 대한 신뢰를 박살내다니!


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

b: 척추 구부려서 프레첼 만들 일 있니?! 폰 볼 때 허리 좀 펴!


```
bb({body:"meta"});
```

b: 너도 마찬가지야.


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

h: 흠...정말 재밌어 보이는걸.


h: 역시 무시하지 말 걸 그랬나?


`bb({mouth:"normal", eyes:"normal"});`

[계속 무시해, 우린 여전히 분위기 깨는 사람들이야](#act1e_ignore_continue)


[사실, 간다고 해.](#act1e_ignore_changetoyes)


[사실, 안 간다고 해.](#act1e_ignore_changetono)


# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: 그래도 계속 무시하는 건 좀 무례하지 않나?


`bb({eyes:"normal_right"});`

b: 하긴, 다른 사람들도 *우릴* 무시하니까.


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

h: 나...놀아도 되는 거지?


b: 뭐, 사실은, 외로우면 *죽을 수도* 있으니까


`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: It's too crowded. Crowds are dangerous.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: 아무튼, 틴더 알림 올라왔어


`bb({eyes:"uncertain"})`

b: 잠깐, 그 원나잇 어플??


`hong({eyes:"annoyed"})`

h: 원나잇 어플이라니. 이건 그냥 새로운 친구를 만나는--


`bb({eyes:"narrow"})`

b: 원나잇 맞잖아
.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: 오, 나 매칭됐어! 귀엽게 생겼네!


```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: 제발 이번엔 망치지 ㅁ-


```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: 위험! 위험! 위험! 위험! 위험! 위험! 위험! 위험! 위험! 위험!


`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[다른 사람들에게 *이용*당할 거야](#act1f_used_by_others)


[다른 사람들을 *이용*하는 거야](#act1f_using_others)


[저 사람은 연쇄 살인마야](#act1f_killer)


# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: 모르는 사람과의 원나잇은 아랫도리는 채울 수 있어도


b: 마음 속에 난 구멍은...


`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: 절대 못 채워


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

b: 설마 남의 거시기를 포켓몬처럼 수집하는 거 아니지?


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

b: ♫ ^창녀^가 될 거야-


(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ 넓적다리와 ^후장^, 풍만한 가슴


(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ 그리고 축축한 ^부랄좆^을 찾아서!


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

b: 중요한 건 우린 영악한 자식이야


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
b: 널 우물에 가두고 네 살가죽으로 옷을 만들 어 입을 수 있을 정도로 흰 식빵만 먹여서 살찌울 거야!

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

h: 난 더 이상 못 하겠어

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"외로움은 우릴 해쳐"... {{/if}}
{{if _.parasite}}"우린 사회의 기생충"... {{/if}}
{{if _.whitebread}}"흰 빵은 우릴 죽일 거야"... {{/if}}
{{if _.subtweet}}"우리 뒷담화를 하고 있어"... {{/if}}
{{if _.badnews}}"세상이 멸망해"... {{/if}}
{{if _.hookuphole}}"고독사로 죽을 거야"... {{/if}}
{{if _.serialkiller}}"저 사람들은 연쇄살인마"... {{/if}}
{{if _.catmilk}}"고양이는 우유를 소화 못 해"... {{/if}}
{{if _.pokemon}}"^개좆^같은 노래 패러디"... {{/if}}

h: 난 그냥 내 삶을 살고 싶어.


h: 이 모든 고통에서 자유로워지고...싶다구.


`bb({eyes:"look_sad"});`

b: 저기...인간...


`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: 괜찮을 거야


(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: 네 충직한 늑대로서, 내가 언제나 위험 요소를 경계하고 안전하게 보호해 주겠어.


`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: 약속할게.


(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: 마지막이네. 인스타그램. 넌 뭐 올라왔니?


`hong({eyes:"sad"});`

h: 이건...또 파티 사진들이잖아.


`hong({mouth:"sad"});`

h: 걱정거리 없이, 불안감 없이, 모두들 행복해 보여. 


`hong({mouth:"anger"});`

h: 난 왜 저 사람들처럼 못 하지? 왜 난 "평범하게" 살 수 없는 걸까?


`bb({eyes:"normal_right"});`

b: 파티 얘기 나와서 그런데, 이번 주말 파티 말야. 내 최종 결정은:


`bb({eyes:"normal"});`

[가자](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`


[가지 말자](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`


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

b: ㅁ


(...1500)

`bb({eyes:"wat_2"});`

b: 뭐?


`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: 난 파티 간다고 얘기하겠어


{{if _.act1g=="go"}}
h: 네가 가라고 해서가 아니라, *내가* 가고 싶어서야.

{{/if}}

{{if _.act1g=="dont"}}
h: 그렇게나 가지 말라고 얘기하니까.

{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: 넌 날 통제할 수 없어.


```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: 그럼 실례, 이 ^염병할^ 장소에서 맛있는 샌드위치 먹을 거야.


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

[으아아아 우린 다 죽을 거야](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`


[으아아아 모두들 우릴 미워해](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`


[으아아아 우린 못된 사람들이야](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`


# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: 으아아아 우린 다 죽을 거야 으아아아아아아
//AHHHH WE'RE GONNA DIE AAAAAAHHHHHHH

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


b: 으아아아 모두들 우릴 미워해 으아아아아아아


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

b: 으아아아 우린 못된 사람들이야 으아아아아아아

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

n: 당신은 성공적으로 인간을 물리적 + 사회적 + 정신적 건강을 지켜냈습니다


n: 햐, 저 감사해하는 거 보세요!


(...500)

n: 이제 에너지가 0이 됐으니, 행동을 직접 선택할 수 있습니다.


`bb({mouth:"smile", eyes:"normal"});`

n: 엔딩을 선택해 주세요


`bb({mouth:"small_lock", eyes:"fear"});`

n: *마무리 일격*
//*FINISH THEM*

[{전투: 짜증나는 폰을 혼쭐내준다!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`


[{도주: 몸을 공처럼 말고 흐느낀다!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`


# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: 네 폰이 공황발작을 일으키고 있었어!


`bb({eyes:"anger"})`

b: 주커버그와 그 일당들이 벤처 투자자들의 돈 때문에 네 정신 건강을 훔친 거야!


```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 폰에게 벌을 줘! 파괴해! 죽여!


```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽여 죽--


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
