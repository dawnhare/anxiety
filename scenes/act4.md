# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (자동 저장 완료)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *하아*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: 그래서 도대체 이 ^좆같은^ 이야기의 교훈은 뭐야?

`hong({body:"one_up", eyes:"annoyed"})`

h: *배운 게* 있기나 해? 난 멍청하게 *굴었고*, 내 "친구들"*은* 날 이용해먹기나 하고, 그리고 우리 둘 다 거의 *죽을뻔* 했잖아.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[그래, 병원비는 말할 것도 없지.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[그래, 간 손상은 말할 것도 없지.](#act4a_liver)
{{/if}}

[그래, 그게  최악의 시나리오*였어*.](#act4a_worst)

[그래, 내가 옳았어.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: 그러게. 건강보험이 내가 "멍청한 ^새끼^"인거 까지 보장해주진 않을 거 같은데.

`hong({eyes:"annoyed", mouth:"normal"});`

b: 그래도... 살았잖아!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: 분명 기대수명을 몇년 정도 갉아 먹긴 했지만...

`bb({eyes:"surprise"});`

b: 그래도 최소한 기대 수명이 남아있잖아! 우린 살았으니까!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: 그래도...

h: 응?

`bb({eyes:"surprise"});`

b: 살았잖아!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: 그리고... 네 말도 맞았어.

`hong({eyes:"surprise"});`

h: 응?

`bb({eyes:"normal"});`

b: 네 말대로 난 양치기-늑대였어. 그래서 *진짜* 위험이 왔을 때, 네가 –이성적으로– 내 말을 믿지 않을만 한 거지.

`bb({eyes:"surprise_r"});`

b: 그래도, 살았잖아!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: 그 난리를 겪고도 우린 아직 여기 있어.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: 거의 죽을 뻔한 경험이었는데 너 꽤 침착하다?
{{/if}}

{{if !_.INJURED}}
h: 진짜 요단강 건널 뻔한 경험이었는데 너 꽤 침착하다?
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: 덕분인지 다른 것들은 비교적 덜 무서워 보여. 그래서 생각해봤는데,

`bb({eyes:"normal", mouth:"normal"});`

b: 내가 너랑 싸우는게 엿같으면, 그게 널 보호해주지 않으니까...

h: 근데 너랑 싸우는 것도 *마찬가지*인걸, 네가 더 시끄럽게 소리치게만 만드니까...

`bb({eyes:"normal_r"})`

b: 그럼 어쩌면...

`bb({eyes:"normal"})`

h: 어쩌면 우린 굳이 싸울 필요는 없겠지.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: 난 엄청 나쁜 늑대가 아니지만, 그렇지만 '경비-늑대'도 아니야.

`bb({eyes:"sad_d"})`

b: 그저 상처받은 떠돌이 개일 뿐이지.

`bb({eyes:"sad"})`

b: 우린 힘든 일을 함께 겪었어. 어쩌면 홀대 받거나 트라우마가 있는지도 몰라. 그러니 가끔 내가 과하게 반응하면서 이렇게 짖어대는 거지,

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: 왈 왈 왈 왈 왈

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: 그치만 겁쟁이 개가 되는 건 *싫어!* 착한 개가 돼서, 널 지켜주고 싶어!

`bb({eyes:"sad", mouth:"normal"});`

b: 인간... 이 늑대를 길들여줄 수 있겠어?

`hong({eyes:"sad"})`

h: 어... 해볼게.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: 좋아. 감정과 건전한 관계. 관계에는 소통이 필요하지. 좋아, 서로 소통해보자.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: 앞으로 5분 동안은 정말 오글거리긴야 하겠는데, 그냥 될때까지 그려러니 하자.

```
hong({body:"hands_2", mouth:"normal"});
```

h: 친애하는 내 안의 늑대에게... *네* 마음은 좀 어때?

n2: 사용된 공포:

n2: *상처받음* {{_.attack_harm_total}}, *사랑받지 않음* {{_.attack_alone_total}}, *나쁜 사람이 됨* {{_.attack_bad_total}}

n2: 어떤 공포에 대해 먼저 말하고 싶나요? (다른 것들도 나중에 선택할 수 있습니다.)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[우리가 다칠까봐 두려워.](#act4_harm)

[우리가 혼자가 될까봐 두려워.](#act4_alone)

[우리가 나쁜 사람은 아닐까 두려워.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: 난 네가 신체적으로 안전하도록 지켜주고 싶어.

`bb({eyes:"sad_d"})`

b: 그렇지만 온 *세상*이 위험해 보인단 말야. 온갖 비극과 사악함으로 가득 찼어.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: 음... 잘 모르겠는데, *내가* 고르는건 이만하고 *넌* 어때, 인간?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: 다시 네 차례야. 네 생각은 어때?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: 더 생각할 건 없어, 인간?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[네 말이 맞아. 그러니까 서로 지켜주자.](#act4_harm_skills)

[그럼 *더 많은* 위험에 노출되어 보자.](#act4_harm_exposure)

[고마워.](#act4_thanks) `_.thanks_for = "신체의 안전";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: 그치만... 어떻게? 난 송곳니랑 발톱도 있는걸? 아, 물론 이건 비유지만.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: 호신술 배워보는 건 어떨까? 아님 서로 보호해주는 공동체에 들어간다던가? 우리 전반적인 건강이나 개인적인 경계선을 개선시켜볼 수도 있고.

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: 그것도 그렇지만...

[대체 어디서부터 시작해야 해?](#act4_harm_skills_start)

[그래도 안 통한다면?](#act4_harm_skills_work)

[너무 과하게 "안전"을 원하면 어쩌지?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: 할 게 너무나도 많아. 스스로 고칠 점이 너무나도 많다고. 대체 어디서부터 *시작해야* 할까?

`hong({ body:"shrug", eyes:"surprise" })`

h: 지금 하고 있잖아.

`bb({ eyes:"normal", mouth:"narrow" })`

b: 응?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: 서로 올바른 소통을 연습하고 있잖아. 그러면 위험을 더 잘 감지하게 되겠지. 과잉반응도 적어질 테고.

`hong({ eyes:"surprise" });`

h: 그러면 우릴 위험으로부터 지키는데 도움이 될 거야!

`hong({ eyes:"normal", mouth:"normal" });`

h: 따라서 *이건* 일종의, 호신술 훈련인 셈이지.

`bb({ eyes:"normal_r" })`

b: 음, 난 그보다 이런 걸 기대하고 있었는데

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: 그래, 우린 서로 100%지킬 방법은 없겠지...

`hong({ body:"one_up" });`

h: 그래도 1%라도 향상한다면, 의미는 분명 있지 않을까?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: 유리잔이 99% 비어있는 것 보다 1% 차있는 거로 보겠다고? 

`bb({ eyes:"normal" });`

h: 사막에서 조난당했다면 그래도 의미는 있을걸.

`bb({ eyes:"closed" });`

b: 그렇다면 뭐, 원샷!

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: 내 말은, 네가 내 경고를 무시한 것도 *내가* 과하게 나가서 그런거잖아!

`bb({ body:"normal", eyes:"normal" })`

h: 그러네, 네 말이 맞아. 적절하게 안전해야지. 모든 걸 적절히.

`bb({ eyes:"suspect" })`

b: 잠깐, *모든걸* 적절히?

`hong({ eyes:"annoyed" })`

h: *적절한 정도*만 적절하게.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: 반복해서 일관되게 말해줘서 고마워.

(#act4_something_else)

# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *뭐라고*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: 예를 들어, 천둥 소리를 무서워하는 개가 있다고 치자.

`hong({ body:"hands_1" });`

h: 이건 훈련사들이 쓰는 기법 중 하난데, 천둥 소리를 녹음하고 이걸 작게 틀어. 개가 침착하게 있으면, 보상을 해 주는 거지.

`hong({ body:"hands_2" });`

h: 그렇게 며칠동안, 개가 천둥 소리에 대한 두려움을 극복할 때까지 볼륨을 조금씩, 조금씩 크게 키우는 거야.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: 노출치료라고 하는거지!

`hong({ body:"point", eyes:"normal" });`

h: 너도 개니까, 네게도 통할 거야. 그치? 모든 포유류는 똑같은 '투쟁 또는 도피' 반응이 있으니까.

`hong({ body:"normal" });`

[만약 *너무* 무덤덤해지면 어떡하지?](#act4_harm_exposure_overboard)

[만약 우리가 *진짜* 위험에 노출되면 어떡해?](#act4_harm_exposure_hurt)

[난 개가 아니라 늑대야.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: 그럼 네가 귀여운 강아지로 길들여질 때까지 인내하고, 친절하게 대해 줄게.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: 아이궁.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: 공포를 차단하면 어떻게 되는지 *방금*  봤었잖아. *정말로* 위험한 상황에 처하게 된다구.

`bb({ eyes:"angry_r", body:"one_up" })`

b: 게다가, *너무* 무덤덤해져서 싸이코패스가 되진 않을까?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: 이러다 공포 스릴러 살인 영화를 보면서 사이코패스처럼 생각할지도 몰라!

`hong({ eyes:"annoyed" })`

h: 난... 그거랑 천둥소리 가운데에 선이 있을 거 같은데.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: 그치만 정확히 *어딘데?* 인간? *어디*?!

`hong({ eyes:"surprise", body:"one_up" })`

h: 그건 몰라. 그치만 *네가* 도와주면 돼!

`hong({ eyes:"normal", body:"normal" })`

h: 너랑 협력하고 상의해가면, 선을 그을 수 있을거야.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: 좋아. 근데 난 늑대라서 손가락 못 쓰니까 선 긋는 건 네가 해야 해.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: 예를 들자면, *지붕* 위에서 뛰어 내렸잖아!
{{/if}}

{{if !_.INJURED}}
b: 예를 들자면, *지붕*위에서 거의 떨어질 뻔 했잖아!
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: 그래, 맞아. 어쩌면 도를 넘을 수도 *있지*.

`hong({ eyes:"normal" });`

h: 그렇지만 그래서, 노출 치료를 하면 조금씩, 위로 한 발짝씩 올라갈 수 있는 거야.

h: *진짜* 위험에 다다르기 전에 멈추는 거지.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: 그래, 시끄러운 천둥 소리 듣는 거랑, 태풍 한 가운데서 뾰족한 모자 쓰고 나가는 거 사이엔 선 그을 수 있지.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: 잠깐, 내 느낌에 대해 할 말 전혀 없어? 그냥... "고마운게" 다야?

`hong({ eyes:"surprise", body:"shrug" })`

h: 그리고.. 내 {{_.thanks_for}}에 대해 걱정하고 있다고 말해줘서 고마워..

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: 괜찮아?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: 내게 *고맙다*고 한 적은 이번이 처음이야.

`hong({ mouth:"smile" });`

h: 으이구, 이 큰 털복숭이 공황-늑대.

(#act4_something_else)

# act4_thanks_2

h: 과잉반응 해도, 내 {{_.thanks_for}}을 돌봐주려 해서 고마워.

`bb({ eyes:"annoyed" })`

b: 잠깐만... 이런 두려움에 대해서 다루기 싫어서 그냥 "고맙다" 하고 넘어가려는 건 아니지?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: 글쎄, 여러모로 좀 복잡해서. 그리고 항상 대답이 준비된 것도 아니고.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: 인생이 무슨 대답을 3지선다에서 고르는 것도 아니잖아.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: 그치만 지금으로서는, 적어도 고맙다고 말하는 거 정도는 할 수 있지.

b: 그럼 나도, 내 말을 침착하게 들어 줘서 고마워.

`bb({ eyes:"closed" });`

b: 이 털 없는 작은 포유류야.

(#act4_something_else)

# act4_thanks_3

h: 네 울음소리가 날 무섭게 하긴 해도, 넌 단지 내 {{_.thanks_for}}을 보호하려는 거잖아.

`bb({ eyes:"smile_r" });`

b: 그래, 근데 계속 날 이렇게 칭찬하다가는 인터넷에서 우릴 이상하게 볼지몰라.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: 에이, 난 그냥 연약한 대학생 꼬맹이고, 넌 크고 무서운 늑대인데 별 일이야 있겠-

`hong({ eyes:"normal", body:"point" });`

h: 아냐, 됐어 그냥 말하지 마.

(#act4_something_else)

# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: 난 네가 인간으로써 어딘가에 속해있다는 걸 깊이 만족하도록 하고 싶어...

`bb({ eyes:"sad_u" });`

b: 그치만 만약 누가 우릴 알게 된다면, –우리의 *진짜* 모습–을 알게 된다면, 겁먹고 달아날까봐 두려워.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: 음... 잘 모르겠는데, *내가* 고르는건 이만하고 *넌* 어때, 인간?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: 다시 네 차례야. 네 생각은 어때?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: 더 생각할 건 없어, 인간?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[그래. 우리 사회적인 생활에도 좀 손을 써보자.](#act4_alone_skills)

[사람들이 우릴 좋아할 거 같은데. 한번 알아볼까?](#act4_alone_experiment)

[고마워.](#act4_thanks) `_.thanks_for = "사회적 소속감";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: 질문을 하거나, 경청하고, 공감하고, 마음을 여는 등의 사회적인 기술을 연습해 볼 수 있지 않을까?

`hong({ eyes:"normal_l" });`

h: 친구들과 약속을 잡거나, 동아리에 정기적으로 참여하는 사회성있는 습관을 기르는 것도 어때?

`hong({ body:"one_up" });`

h: 거절을 더 편안하게 받아들이는 법을 배울 수도 있을 거야.

`hong({ eyes:"normal" });`

h: 아님 우릴 기피하는 게 아니라는 걸 배울 수도 있겠지. 그냥 피곤하다거나 낮짝이 원래 ^좆같을^ 수도 있잖아.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: 그거 참 선택지도 많다. 근데, "사회성 기술 배우는 거" 말야...

[우리 입맛대로 *조작하는* 거 아닐까?](#act4_alone_skills_manipulative)

[우릴 *휘둘리기 쉽게* 하려는거 아닐까?](#act4_alone_skills_manipulated)

[그래도 실패한다면?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: 피해자의 감정을 잘 읽는 연쇄살인마도 사실상 굉장한 "공감능력"을 가진 거 알아?

`bb({ eyes:"annoyed" });`

b: 왜 유명한 연쇄살인마들 보면 친구가 많고 영향력 있는 사람들이잖아? 

`hong({ eyes:"annoyed", body:"chin" });`

h: 그래, 네 말이 맞는거 같아.

h: "사회성 기술"은 우리가 다른 사람들을 *위해서* 배려해주는 게 아니면 아무 의미 없지.

`hong({ body:"normal" });`

h: 기본적으로, ^좆^같이 굴지 않으면 돼.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: 오, 동기 유발 표어감으로 딱인데?

`hong({ body:"shrug", mouth:"narrow" });`

h: “^좆^같이 굴지 마세요™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: 사람들이 짓밟고 발을 닦아도 웃으면서 감사합니다 하는 발닦개가 될 거야!

`bb({ mouth:"scream", eyes:"scream" })`

b: 하도 키스를 해서, 갈색 립스틱 바른 것처럼 보이겠지!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: 그래, 맞아. 남들한테 잘 해 주는 게 다는 아니지. *선을 긋는 것*도 사회적 기술이야.

`hong( body:"one_up" });`

h: 우리 집을 지탱할 벽이 없다면, 다른 사람들을 우리 집으로 초대할 순 없잖아?

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: 그리고... 립스틱 뭐? *우웩*.

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: 아마도 실패하겠지. 아니, 실패하게 *될 거야*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: 그래도 괜찮아! 누구나 처음엔 실패하면서 배우는 거잖아!

`hong({ body:"normal", eyes:"normal" });`

h: 그니까 같이 실패해 가면서 나아가자, 알겠지?

`bb({ eyes:"normal_r" });`

b: 그래, 최악의 경우엔 이 마을을 떠나서 새로운 삶을 누려보지 뭐.

`bb({ eyes:"normal" });`

h: 맞아, 그거 요즘에 비트코인 2개면 된다더라.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: 실험을 좀 해보자!

`hong({ body:"chin" });`

h: 친구한테 같이 어울리자고 먼저 톡 보낼 수도 있고, 오랜 친구와 다시 연락해 볼 수도 있고, 아님 그냥 택시기사 아저씨랑 얘기 나눌 수도 있고.

`hong({ body:"normal" });`

h: 우리 생각보다 호감형일 지도 모르잖아.

`bb({ eyes:"annoyed" });`

[만약 이게 "별 거 아닌" 성공이면 어떡해?](#act4_alone_experiment_cheap)

[만약 이게 민폐끼치는 거면 어떡해?](#act4_alone_experiment_burden)

[그치만 잡담은 우리의 *진짜*모습이 아니잖아!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: 얕은 미소만 짓고 있으면, 다른 사람과 진정으로 이어지지 못할 거야.

`bb({ eyes:"super_sad" });`

b: 그렇다고 본모습을 보이면 우리의 망가진 속마음을 보게 될 텐데!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: 굴러봐.

b: 뭐?

`hong({body:"hands_1"})`

h: 개는 사랑과 신뢰를 보여주고 싶을 때, 배를 보여줌으로써 위험에 노출시키지.

`hong({body:"one_up"})`

h: 아직은 안심할 수 있을 정도로 강하지 않을지도 모르지만, 훈련을 계속하면

`hong({body:"normal", eyes:"surprise"})`

h: 언젠가는, 망가졌어도 인간다운 우리의 본 모습을 보여줄 수도 있을 거야.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: 간식 주면 구를게.

`bb({ eyes:"normal", mouth:"normal" });`

h: 안돼.

(#act4_something_else)

# act4_alone_experiment_cheap

b: 택시기사 아저씨한테 인사하는 게 인싸-올림픽 금메달감은 아니잖아.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: *우리들*을 위한 거지!

`hong({ body:"one_up", eyes:"annoyed" });`

h: "사회"라는 경기장에서 우린 페더급도 안 될걸? 한... 쿼크급?

`hong({ body:"normal", eyes:"normal" });`

h: 별 거 아닌 하찮은 승리라도 뭐 어때. 천리 길도 한 걸음부터야.

b: 맞아! 인사하고 난 뒤에 더 얘기할 수도 있어. 예를 들면...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"잘 지내시나요?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"별로요!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: 택시기사 아저씨는 그냥 운전이나 하고싶을텐데, 우리가 사회성이 얼마나 떨어지는지 *실험*하는 건 민폐가 아닐까?

`bb({ eyes:"annoyed" })`

h: 정말로 우리가 *민폐*라면...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: 그것도 알게 돼서 좋은 거지!

`hong({ eyes:"normal" });`

h: 사전에 민폐될 만한 건 뭔지 물어본다거나, 어디까지가 선인지, 그리고 그 선을 존중해주는 법도 배워갈 수 있으니까.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: 그, 심리상담가들 책자에 나온 "대인관계 기술" 같은 ^지랄염병^ 있잖아. 

(#act4_something_else)

# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: 네 도덕적 욕구를 채워주고 싶어. 네가 더 좋은 사람이 되려고 하는 욕구...

`bb({ eyes:"sad_d" })`

b: 그렇지만 우리 마음 속 깊은 곳이 근본적으로... 망가졌어.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: 망가진 게 *아니*라고 할 생각 마. *옥상*에서 뛰어내렸잖아.
{{/if}}

{{if !_.INJURED}}
b: 망가진 게 *아니*라고 할 생각 마. *옥상*에서 뛰어내릴 뻔 했잖아.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: 음... 잘 모르겠는데, *내가* 고르는건 이만하고 *넌* 어때, 인간?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: 다시 네 차례야. 네 생각은 어때?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: 더 생각할 건 없어, 인간?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[그래, 망가져있네. 한번 고쳐보자.](#act4_bad_fix)

[그래, 망가져있네. 받아들여 보자.](#act4_bad_accept)

[고마워.](#act4_thanks) `_.thanks_for = "도덕적 건강";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: 좋은 습관을 조금씩 기를 수도 있고, 우리가 가치있게 여기는 것과 우리 삶을 일치시켜 볼 수 있고,

`hong({body:"one_up"});`

h: 필요하다면, 정신과 상담이나 심리 상담 같은 전문적인 도움도 받을 수 있지.

`hong({body:"normal"});`

h: 방법은 있어.

[하지만 다 못 고치면 어떡해?](#act4_bad_fix_cant)

[하지만 우릴 *너무* 고쳐 버리면?](#act4_bad_fix_too_much)

[전문적인 치료받을 돈도 없잖아.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: 그래, 그 말도 맞아.

h: 전부 다 고칠 순 없어.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: 으아아! 역시 우린 망가진 거야!

`hong({eyes:"surprise"});`

h: 하지만 비교적 덜 망가질 순 있어.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: 상처는 시간이 지나면 낫지만, 흉터는 그대로 남아. 그래도 괜찮아.

`bb({eyes:"annoyed_r"});`

b: 나도 그래. 그리고 말야,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: 흉터는 *섹시해*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: 아, 쫌, 제발.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: 인정하기 정말 싫지만... 내 일부는 *이 장애*를 가지길 원하고 있어.

`bb({ eyes:"angry" })`

b: 그러니까, 그게 없으면 *지루하지* 않을까?

`bb({ eyes:"sad_r", body:"one_up" })`

b: *결함*이 없다면, "예술"은 밋밋하고 재미없는 게 되지 않을까?

`bb({ eyes:"sad_u", body:"two_up" })`

b: 그리고 결함이 없다면, 결함을 가진 친구들과는 전혀 이어질 수 없지 않을까?

`bb({ eyes:"sad", body:"chest" })`

b: 게다가 이런 삶에 만족하게 되면, 대단한 장면들을 보는걸 그만두고 우리의 드라이브는 끝이나게돼.

`hong({ MOUTH_LOCK:true })`

h: ...

h: 두려워할 게 없어지는 게 두렵다...

h: 그럴 일은 없을 것 같아.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: 휴! 정말 다행이야! 야호!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "의사 선생님, 전 지금 제가 어떤지 물어보시는 그 말씀을 들으려 시간당 10만원씩 쓰고 있어서 너무 불안해요."

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "어흠, 그럼 지금 어떠신지요?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: 아, 완전 적절한 걱정이야.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: 많은 사람들이 돈이 부족해서 정신과 치료를 받지 못한다는 게 진짜 싫어.

`hong({ eyes:"normal", mouth:"normal" });`

h: 그래도 그보다 싸거나, 아예 무료인 방법도 있어 

`hong({ body:"chin" })`

h: 지원 단체라든가, 온라인 상담이라든가, 또래상담, 비영리 보건소 등을 이용하거나...

`hong({ body:"hands_1" })`

h: 명상이나, 숙면, 친구들과 대화하기, 새로운 걸 배우는 등의 습관을 기르는 것도 좋고

`hong({ body:"hands_2" })`

h: 도서관에서 근거에 기초한 심리 치료에 관한 책을 빌리는 것 등등...

`hong({ body:"one_up" })`

h: 이 게임 끝에는 도움을 받을 수 있는 정보들이 있어!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: 플레이어에게 말하는것도 중요하겠지.

`hong({ body:"point" });`

h: 정신 건강 같은 건 서사적 관습보다 더 중요하거든.

(#act4_something_else)

# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: 그게 상담사들이 말하는 거잖아? 좋은 감정, 나쁜 감정 모두 받아들여라?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: 잠깐.

["받아들인다는" 게 *포기한다는* 의미야?](#act4_bad_accept_give_up)

["받아들인다는" 게 *괜찮다는* 의미야?](#act4_bad_accept_approve)

["받아들인다는" 게 *말 그대로*의 의미야?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: 마틴 루터 킹이 "어이구 버스 앞자리에 못앉는구먼, 그냥 받아들이지 뭐"라고 했을 거 같아?

`bb({ eyes:"angry_r", body:"two_up" });`

b: 왜 자립 산업 단지는 백기를 흔드는 것이 무슨 엄청난 지혜라도 되는 줄 아는 거야?

`bb({ eyes:"annoyed", body:"normal" });`

h: 내 생각에 치료사는 나쁜 것을 "인정"하라는 것 같아. 해결하기 쉽지 않다는 걸 인정하는 것을.

h: 변화하려는 의지를 꼭 포기하라는 뜻은 아니라는 거야.

`bb({ eyes:"suspect" });`

b: 그러면 그걸 *받아들인다*는 게 아니라, *인정한다*고 말해야지.

`hong({ body:"chin", eyes:"annoyed" });`

h: 맞네, 그러고 보니 "받아들인다"는 말 뜻이 좀 헷갈리는구나.

`bb({ eyes:"closed", mouth:"narrow" });`

b: 그건 "인정".

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: 망가지는게 좋을거 같아? 아니야!

`bb({ eyes:"angry_r", body:"one_up" });`

b: 정신질환을 미화하는 망할 할리우드 시나리오 작가들은 전부 다 똥덩어리야!

`bb({ eyes:"angry", body:"two_up" });`

b: 정신적 장애는 정말 거지같아! 사람들의 *삶도* 앗아가잖아! 그런 걸 왜 *받아들여야* 해?!

`bb({ body:"normal" });`

h: 내 생각에 감정을 *받아들이라*는 의미는, 인내심을 가지라는 것 같아.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: 늪에서 발버둥칠수록 가라앉지만, 가만히 엎드리면 나올 수 있는 것처럼 말이지.

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: 너랑 싸우고, 난 공포로 인해 옥상에서 뛰어내리게 했지.
{{/if}}

{{if !_.INJURED}}
h: 너랑 싸우고, 난 공포로 인해 옥상에서 뛰어내릴뻔 했지.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: 그 대신에 지금처럼 싸우지 말고, 서로를 인내하는 것이 해결 방안이야.

`bb({ eyes:"annoyed" });`

b: 그럼 "받아들인다" 같은 애매하고 헷갈리는 용어가 아니라 *그렇게* 말했어야지.

`hong({ body:"chin", eyes:"annoyed" });`

h: 맞네, 그러고 보니 "받아들인다"라는 말이 좀 그렇구나.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: 그런 받아들임은 *받아들일* 수 없어.

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: 이미 날 받아들일 순 없다는 거 *알잖아!*

`bb({ eyes:"sad_u", body:"two_up" });`

b: 가장 큰 문제는 널 도와주고 싶지만, 내가 제대로 전달하지 못 하는 거라구!

`bb({ eyes:"sad", body:"normal" });`

h: 내 생각에 감정을 받아들이라는 의미는 싸우지도, 무시하지도 말라는 것 같아.

`hong({ eyes:"surprise", body:"one_up" });`

h: 네 말을 듣고, *협력*하되, 100% 곧이곧대로 듣지는 말라는 거지.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: 그럼 "받아들인다" 같은 애매하고 헷갈리는 용어가 아니라 *그렇게* 말했어야지.

`hong({ body:"chin", eyes:"annoyed" });`

h: 내 생각엔 그 사람들도 단어 선정은 영 별로야.

(#act4_something_else)

# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: 아무튼, 더 얘기할 거 있어?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: 그럼, 이제 가슴에서 더 털어낼 건 없어?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[우리가 다칠까봐 두려워.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[우리가 혼자가 될까봐 두려워.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[우리가 나쁜 사람은 아닐까 두려워.](#act4_bad)
{{/if}}

[아냐, 이제 됐어.](#act4c_prelude)

# act4_something_else_2

h: 자, 이렇게 우리가 가진 공포에 대해서 얘기해 봤어.

b: 응, 3가지 공포가 있지.

h: 그렇지, 딱 3개

b: 편하네.

(#act4c)

# act4c_prelude

h: 좋은 대화였어.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: 이건 *게임*같은 게 아니야

`bb({eyes:"angry_d", body:"one_up"})`

b: 감정과 건전한 관계를 만드는 건 화면에 뜬 버튼 클릭하는 것처럼 간단한 게 아니라구.

`bb({eyes:"sad", body:"normal"})`

b: 정말 우리가 잘 어울릴 수 *있을까*?

b: 한 팀으로서 협력할 수 *있을까*?

`hong({eyes:"sad", body:"one_up"})`

h: 글쎄,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: 저-기...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: 여, 여, 옆에서 같이 밥 먹어도 괜찮아?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *이런 애*가 좋다고? 그리고 얜 무슨 싸이코 연쇄 살인마처럼 왜 혼자 앉아 있대?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: 좋아하는 사람한테 옆에 앉아도 되냐고 물어본 거야? 완전 *구질구질*해 보이는 거 알지?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *이런 애*가 좋다고? 우리가 얘네 평화와 안정을 방해했잖아! 우린 민폐덩어리야!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: 그, 그러니까 안 돼도 괜찮아. 난 그냥...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[잠깐, 우리 파티에서 보지 않았어?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[그래, 좋아! 여기 앉아.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[미안, 지금은 좀 혼자 있고 싶어서.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: 맞아, 그 파티 때 소파에 누워 있었잖아!

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: 내가 파티 주최자한테 죽빵날린 그 때 말이야.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: 내가 패닉상태에 빠져서 울면서 뛰쳐나간 그 때 말이야.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: 인간, 잠깐만. 우리가 쟤 불편하게 만드는 걸 수도 있어.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: 앗, 불편하게 하려는 건 아니야!

`publish("act4", ["hong_to_alshire",4]);`

h2: 그냥 익숙한 얼굴이라서 그래.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: 으아아아! 역시! 쟤는 공황에 빠진 위험한 싸이코야!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: 으아아아! 첫 인상이 "트라우마를 목격함"이라니! 우릴 싫어할 게 뻔해!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: 으아아아아! 트라우마를 떠올리게 했어! 우린 존재만 해도 남에게 상처를 줘!
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: 인간, 잠깐만. 우리가 쟤 불편하게 만드는 걸 수도 있어.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: 아, 당연히 강요는 아냐!

`publish("act4", ["hong_to_alshire", 4]);`

h2: 그냥 앉고 싶으면 앉아도 돼.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: 너무 친절하게 대하잖아! 연쇄살인마 테드 번디처럼 말야!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: 그냥 친절한 척하는 거야! 우리랑 진심으로 친하게 지내고 싶어하는 사람은 아무도 없어!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: 아아아아 우린 맨날 남 어색하게 만들어! 우린 이 지구의 더러운 얼룩이야!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: 인간, 잠깐만. 우리가 쟤 불편하게 만드는 걸 수도 있어.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: 아, 무례한 뜻은 없어.

`publish("act4", ["hong_to_alshire", 6]);`

h2: 그냥 내 생각 좀 정리해야 해서 그래. 네가 싫어서 그러는 게 아냐.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: 무슨 뒤틀리고 역겨운 생각을 정리하길래 저러지?! 저 싸이코의 음침한 욕망을 채우는 게 뭐길래?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: 우리가 싫대! 우린 절대 사랑받지 못할 거야!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: 우리가 쟤 생각 정리하는 걸 방해해버렸어! 우리 때문에 영원히 갖고 갈 트라우마가 생기겠지!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: 흠, 이상하네. 무슨 생각을 했길래?

`publish("act4", ["hong_closer", 2]);`

h: 아무튼, 어디까지 했지?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: 어.. 나도 까먹었는데? 무슨 협력하는 거였나?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: 사람들은 감정을 무슨 "전범"인것 마냥 "화해"해야 된다고 해.

`publish("act4", ["bb_closer", 7]);`

b: 하지만 난 화해한 사이보다, *동맹* 관계였으면 좋겠어!

`publish("act4", ["bb_closer", 3]);`

b: 네 생리적 욕구를 알려주는 배고픔과 갈증처럼, 나도 좋은 경비-견이 되고 싶어.

`publish("act4", ["bb_closer", 8]);`

b: 안전해지고자 하는, 소속감을 가지고자 하는, 더 나은 사람이 되고자 하는, *심리적 욕구*를 알려주고 싶어.

`publish("act4", ["bb_closer", 1]);`

b: 하지만... 난 잘 못해. 그래서 네가 날 훈련시켜야 해.

`publish("act4", ["bb_closer", 4]);`

b: 난 "늘 옳은 것"도 아니고, "늘 비합리적"이지도 않아. 단지... 최선을 다하는 것 뿐이야. 그러니 부탁할게.

`publish("act4", ["bb_closer", 30]);`

b: 널 도울 수 있게 날 도와 줘!

`publish("act4", ["bb_closer", 6]);`

b: 물론, 늙은 개에게 새로운 재주를 가르치는 건 *꽤* 걸릴 거야. *몇 년*이 걸릴 수도 있지.

`publish("act4", ["bb_closer", 3]);`

b: 그리고 가끔 재발할지도 몰라. 예전의 습관들이.

`publish("act4", ["bb_closer", 2]);`

b: 그림자를 보고 짖고, 무서운 말을 할 지도 모르고, 심지어 보기 거슬리는 모습을... 보여줄 수도 있어.

`publish("act4", ["bb_closer", 9]);`

b: 정말 미안해! 난 닳고 닳은 유기견이야! 가끔 똥오줌도 못 가리는 똥개!

`publish("act4", ["bb_closer", 4]);`

b: 그래도 인내를 갖고... 나와 함께 있어준다면...

`publish("act4", ["bb_closer", 8]);`

b: 이 늑대를 길들일 수 있을 거야.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[착하지, 우리 강아지.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[착하다, 우리 인간.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: 으아아아아! 또 혼밥하고 있어! 담배 15개피! 으아아아
{{/if}}

{{if _.parasite}}
b: 으아아아 먹는 동안 아직도 비생산적이야! 우린 사회의 기생충이야! 으아아아
{{/if}}

{{if _.whitebread}}
b: 으아아아 '하얀 식빵'을 더 먹고 있잖아 으아아아아
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: 왈 왈 왈 왈 왈 왈

(#credits)
