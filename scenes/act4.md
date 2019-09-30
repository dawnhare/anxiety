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

n3: (game auto-saved)

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

h: 그래서 도대체 이 이야기의 교훈은 뭐냐?

`hong({body:"one_up", eyes:"annoyed"})`

h: 배운 게 있기나 해? 난 멍청하게 굴었고 내 "친구들"은 날 이용해먹기나 하고, 거의 *죽을* 뻔 했잖아.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[그래, 병원비는 말할 것도 없지.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[그래, 간 손상은 말할 것도 없지.](#act4a_liver)
{{/if}}

[그래, 그게  최악의 시나리오*였*어.](#act4a_worst)

[그래, 내가 옳았어.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: 그러게. 내 건강보험이 내가 "멍청한 ^새끼^"인 거 까지 보장해주진 않을 거 같은데.

`hong({eyes:"annoyed", mouth:"normal"});`

b: 그래도... 살았잖아!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: 분명 기대수명을 몇년 정도 갉아 먹긴 했지만...

`bb({eyes:"surprise"});`

b: 기대 수명이 *남아있기라도* 하잖아! 살았다고!

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

b: 그런데... 네 말도 맞았어.

`hong({eyes:"surprise"});`

h: 응?

`bb({eyes:"normal"});`

b: 네 말대로 난 양치기 늑대였어. 그래서 *진짜* 위협이 왔을 때, 네가 내 말을 믿지 않을만 한 거지.

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
h: 진짜 거의 죽을 뻔한 경험이었는데 너 꽤 침착하다?
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: 뭐, 덕분인지 다른 것들은 비교적 덜 무서워 보이네. 그래서 생각해봤는데,

`bb({eyes:"normal", mouth:"normal"});`

b: 너랑 싸우는 게 널 지켜주지 못해서 별로라면 말야...

//If me fighting you sucks, because it doesn't protect you...

h: 근데 너랑 싸우는 것도 마찬가지인걸, 네가 더 시끄럽게 소리치게만 만드니까...

//But me fighting you *also* sucks, because it just makes you yell louder...

`bb({eyes:"normal_r"})`

b: 그럼 어쩌면...

`bb({eyes:"normal"})`

h: 어쩌면 싸울 필요도 없던 거야.

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

b: 난 사악한 늑대가 아냐. 그렇지만 경비 늑대도 아닌 걸.

`bb({eyes:"sad_d"})`

b: 그저 상처받은 떠돌이 개일 뿐이지.

`bb({eyes:"sad"})`

b: 힘든 일을 겪었지. 어쩌면 홀대 받거나 트라우마가 있을지도 몰라. 그래서 가끔 내가 과하게 반응하면서 짖어대는 거지

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

b: 그치만 겁쟁이 개가 되는 건 *싫어*! 널 지켜주고 싶단 말이야! 착한 개가 되고 싶다구!

`bb({eyes:"sad", mouth:"normal"});`

b: 인간... 이 늑대를 길들여줄 수 있겠어?
//Human... will you help tame this wolf?

`hong({eyes:"sad"})`

h: 어... 해볼게.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: 좋아. 감정과 건강한 관계. 관계에는 소통이 필요하지. 좋아, 서로 소통해보자.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: 앞으로 5분 동안은 정말 오글거리긴야 하겠는데, 그냥 될때 까지 그려러니 하라고.

//The next five minutes are going to sound super cheesy, but let's fake it 'til we make it.

```
hong({body:"hands_2", mouth:"normal"});
```

h: 자 내 안의 늑대에게... *네* 마음은 좀 어때?

n2: 사용된 공포:

n2: *해를 입음* {{_.attack_harm_total}}, *사랑받지 않음* {{_.attack_alone_total}}, *나쁜 사람* {{_.attack_bad_total}}

n2: 어떤 공포에 대해 먼저 다뤄보고 싶으신가요? (다른 것들도 나중에 다룰 수 있습니다.)

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

b: 네 신체적으로 안전하다고 느끼도록 지켜주고 싶어.

//I want to protect your need for physical safety, 직역하기 어렵군요;;

`bb({eyes:"sad_d"})`

b: 그렇지만 온 *세상*이 위험해 보인단 말야. 온갖 비극과 사악함으로 점철되어 있잖아.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: 모르겠네, *내가* 할 말 고르는 건 이쯤하자고. *넌* 어때, 인간?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: 다시, 네 차례야. 네 생각은 어때?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: 더 생각나는 거 없어, 인간?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[네 말이 맞아. 그니까 서로 지켜주자구.](#act4_harm_skills)

[그럼 *더 많은* 위험에 노출되어 보자구.](#act4_harm_exposure)

//Let's expose ourselves to *more* danger.

[고마워.](#act4_thanks) `_.thanks_for = "신체의 안전";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: 그치만... 어떻게? 난 송곳니랑 발톱도 있지만... 이건 그냥 비유잖아.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: 호신술 배워보는 건 어때? 아님 서로 보호해주는 공동체에 들어간다던가? 우리 전반적인 건강이나 개인적인 경계선을 개선시켜볼 수도 있고.

//We could learn self-defense? Join a community that protects each other? Improve our general health & personal boundaries?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: 어쩌면, 근데...

[대체 어디서부터 시작해야 해?](#act4_harm_skills_start)

[그래도 안 통한다면?](#act4_harm_skills_work)

["안전함"에 너무 과하게 나가 버린다면?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: 할 게 너무나도 많아. 스스로 고칠 점이 너무나도 많다고. 대체 어디서부터 *시작해야*해?

`hong({ body:"shrug", eyes:"surprise" })`

h: 지금 시작하고 있잖아.

`bb({ eyes:"normal", mouth:"narrow" })`

b: 뭐?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: 서로 올바른 소통을 연습하고 있잖아. 그러면 위험을 더 잘 감지하게 되겠지. 과잉반응도 적어질 테고

`hong({ eyes:"surprise" });`

h: 그러면 *그게* 우릴 위험으로부터 지키는데 도움이 될 거야!

`hong({ eyes:"normal", mouth:"normal" });`

h: 따라서 이건: 일종의 호신술 훈련인 *셈*이지.

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

h: 그래, 우릴 100% 지킬 방법은 없겠지...

`hong({ body:"one_up" });`

h: 그래도 1%의 향상이라도 분명 의미는 있잖아 그치? 

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: 유리잔이 99% 비어있는 것 보다 1% 차있는 거로 보겠다고? 

`bb({ eyes:"normal" });`

h: 그래도 의미있는 것이지. 네가 사막에 조난당해 있다면 말이야.

`bb({ eyes:"closed" });`

b: 그렇다면 뭐, 원샷!

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: 내 말은, 네가 내 경고를 무시한 것도 *내가* 과하게 나가서 그런 거잖아!

`bb({ body:"normal", eyes:"normal" })`

h: 그러네, 네 말이 맞아. 적절하게 안전해야지. 모든 걸 적절히 해가면서

`bb({ eyes:"suspect" })`

b: 잠깐, *모든* 걸 적절하도록 손 보겠다고?

`hong({ eyes:"annoyed" })`

h: *적절한 정도의 것들만* 적절히 유지해야 겠지.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: 네 말을 반복적으로 스스로 일관되게 해줘서 정말 고마워.

(#act4_something_else)

# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *뭐라고*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: 내 말은, 예를 들어 천둥을 무서워하는 개가 있다 보자.

`hong({ body:"hands_1" });`

h: 훈련사들이 쓰는 기법중에 이게 있는데, 천둥 소리를 녹음하고 이걸 작게 틀어, 그리고 개가 침착하게 있으면 보상을 주는 거야.

`hong({ body:"hands_2" });`

h: 수 일간, 훈련사는 볼륨을 조금씩 크게 키우지, 개가 천둥소리에 대한 두려움을 극복할 때 까지.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: 노출 치료라고도 한다고!

`hong({ body:"point", eyes:"normal" });`

h: 너도 개니까, 네게도 통하겠지, 그치? 모든 포유류는 똑같은 투쟁-도피 반응이 있으니까. 

`hong({ body:"normal" });`

[만약 *너무* 무덤덤해지면 어떡하지?](#act4_harm_exposure_overboard)

[만약 우리가*진짜* 위험에 노출되면은??](#act4_harm_exposure_hurt)

[난 늑대야, 개가 아니라고.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: 그럼 네가 귀여운 강아지로 길들여질 때 까지 내 친절함과 참을성을 보여주겠어.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: 아이궁.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: 공포를 차단하면 어떻게 되는지 *방금*  봤었잖아. 너 스스로를 *정말로* 위험한 상황에 처하게  될지도 모른다고. 

`bb({ eyes:"angry_r", body:"one_up" })`

b: 더군다나 *너무* 무덤덤해지다가 싸이코패쓰가 되면 어떻게 해?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: 이러다가 스너프물 야동보면서 보상 받으려 할지도 모른다고!

`hong({ eyes:"annoyed" })`

h: 그... 거랑 천둥소리 가운데에 선이 있을 거 같은데

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: 그치만 정확히 *어디에*? 인간? *어디냐구*?!

`hong({ eyes:"surprise", body:"one_up" })`

h: 나도 그건 모르겠어. 그치만 *네가* 도와주면 돼!

`hong({ eyes:"normal", body:"normal" })`

h: 너랑 협력하고 상의해가면서 선을 그을 수 있을 거야.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: 좋아. 근데 난 늑대라서 손가락 못 쓰니까 선 긋는 건 네가 해야 해.

//Okay. But I've got no opposable thumbs, so you have to do the drawing.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: 예를 들자면, *지붕* 위에서 뛰어 내렸잖아!
{{/if}}

{{if !_.INJURED}}
b: 예를 들자면, *지붕*위에서 서의 떨어질 뻔 했잖아!
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: 그래, 맞아. 어쩌면 너무 멀리 갈 *수*도 있지

`hong({ eyes:"normal" });`

h: 근데 그 덕분에 노출 치료를 하면은 조금씩 위로 한 발짝씩 올라갈 수 있는 거야.

h: *진짜* 위험에 다다르기 전에 멈추는 거지.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: 그래 뭐, 천둥 소리 듣는 거랑 폭풍속에서 뾰족한 모자 쓰고 나가는 거 사이에 선 그을 수 있지.

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

b: 잠깐, 내가 느끼는 거에 대해 할 말이나 반박할 거 없어? 그냥... 고마운 게 다야?

`hong({ eyes:"surprise", body:"shrug" })`

h: 그래! 내 {{_.thanks_for}}에 대한 네 걱정을 알려줘서 고마워.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: 괜찮아?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: 내게 *고맙다고*한 적은 이번이 처음이야.

`hong({ mouth:"smile" });`

h: 어이구 이 털복숭이 겁쟁이 늑대야.

//Aw you big fuzzy-wuzzy panic-wolf.

(#act4_something_else)

# act4_thanks_2

h: 네가 과잉반응 할지라도, 내 {{_.thanks_for}}을 돌봐주려 해서 고마워.

`bb({ eyes:"annoyed" })`

b: 잠시만... 이런 두려움에 대해서 다루기 싫어서 그냥 "고맙다고"만 반복하고 그냥 넘어가려는 건 아니지?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: 글쎄, 여러모로 좀 복잡해서. 그리고 항상 대답이 준비된 것도 아니고.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: 인생이 무슨 대답을 3지선다에서 고르는 것도 아니잖아.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: 그치만 지금으로서는, 적어도 고맙다고 말하는 거 정도는 할 수 있지.

b: 뭐, 그럼 나도 고마워. 내 말을 침착하게 들어 줘서.

`bb({ eyes:"closed" });`

b: 이 털 없는 작은 포유류야.

(#act4_something_else)

# act4_thanks_3

h: 네 울음소리가 날 무섭게 하긴 해도 넌 단지 내{{_.thanks_for}}을 보호하려는 거잖아.

`bb({ eyes:"smile_r" });`

b: 잠깐, 계속 날 이렇게 칭찬하다가는 인터넷에서 우릴 이상하게 보겠어.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: 에이, 난 그냥 연약한 대학생 꼬맹이고 넌 크고 무서운 늑대인데 그게 뭐-

`hong({ eyes:"normal", body:"point" });`

h: 아냐, 말하지 않아도 돼.

(#act4_something_else)

# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: 난 네가 그 깊고 인간다운 소속감을 충족시킬 수 있도록 하고 싶어...

`bb({ eyes:"sad_u" });`

b: 그치만 만약 누구라도 우릴 알게 된다면, 우리의 *진짜* 모습을 말야, 겁먹고 달아날까봐 두려워.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: 모르겠네, *내가* 할 말 고르는 건 이쯤하자고. *넌* 어때, 인간?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: 다시, 네 차례야. 네 생각은 어때?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: 더 생각나는 거 없어, 인간?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[동의해. 우리 사회적 생활에도 좀 손을 써보자.](#act4_alone_skills)

[사람들이 나 좋아할 거 같은데. 한번 알아볼까?](#act4_alone_experiment)

[고마워.](#act4_thanks) `_.thanks_for = "사회적 소속감";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: 질문하거나 경청하고 공감하고 마음을 여는 것처럼 사회성 기술을 연습해 볼 수 있지 않을까?

`hong({ eyes:"normal_l" });`

h: 아니면 사회성있는 습관을 기른다던가, 친구들과 약속도 잡고 아님 동아리같은데 정기적으로 참여한다던지?

//Or make better social habits, like scheduling time with friends or regularly going to meetups?

`hong({ body:"one_up" });`

h: 거절당하는 거에 편해지는 법을 배울 수도 있고.

//Could also learn to get more comfortable with rejection.

`hong({ eyes:"normal" });`

h: 아니면 사람들이 우릴 기피하는 게 *아닐* 때에 대한 것도 알 수 있을 테고. 사실은 그냥 피곤하다거나 낮짝이 원래 ^좆같다^거나 

//Or learn to know when people *aren't* rejecting us, they're just tired or have Resting ^Bitch^ Face.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: 그거 참 선택지도 많다. 근데, 사회성 기술 배우는 거 말야...

[그거 사람들을 우리 입맛대로 *조작하는* 거 아냐? ](#act4_alone_skills_manipulative)

[우리가 다른 사람들 마음대로*휘둘리게* 놔두는 건 아닐까?](#act4_alone_skills_manipulated)

[그래도 실패한다면?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: 피해자의 감정을 잘 읽는 연쇄살인마도 사실상 굉장한 "공감능력"을 가진 거 아냐?

`bb({ eyes:"annoyed" });`

b: 유명한 연쇄살인마들 중에 친구가 많다거나 영향력있는 사람인 경우도 많잖아? 

`hong({ eyes:"annoyed", body:"chin" });`

h: 그래, 네가 맞아.

h: "사회성 기술"은 우리가 다른 사람들을 *위해서* 배려해주는 게 아니면 아무 의미 없지.

`hong({ body:"normal" });`

h: 기본적으로, ^좆^같이 굴지 않으면 돼.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: 오 동기 유발 표어감으로 딱인데?

`hong({ body:"shrug", mouth:"narrow" });`

h: “^좆^같이 굴지 마세요™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: 발닦개처럼 되어서 생글생글 웃으면서 사람들은 우릴 짓밟고 문지르게 될 거라고!

//We'll become a Welcome doormat, saying Please and Thank You as people wipe their feet on us!

`bb({ mouth:"scream", eyes:"scream" })`

b: 하도 빨아대서 갈색 립스틱이라도 바르게 된 거처럼 보일 거야!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: 그래, 네가 맞아. "사회적 기술"은 남들한테 잘 대해주는 게 다는 아니지. *선을 긋는 것*도 사회적 기술이야.

`hong( body:"one_up" });`

h: 우리 집을 잡아줄 벽이 없으면 남을 우리 집으로 초대할 수 없는 법이잖아?

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: 그리고... ㄴ립스틱 뭐? *드러워*.

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: 실패할지도 사실, 실패하게 *될 거야*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: 그래도 괜찮아! 누구나 처음엔 실패하면서 배우는 거잖아!

`hong({ body:"normal", eyes:"normal" });`

h: 그니까 같이 실패하면서 전진해 보자고, 어때?

`bb({ eyes:"normal_r" });`

b: 그래 뭐... 최악의 상황이면 그냥 여기서 빠져나가서 새 정체성을 가지면 되지.

`bb({ eyes:"normal" });`

h: 그래 그거 요즘에 한 2 비트코인이면 된다더라.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: 실험해 볼 수 있지!

`hong({ body:"chin" });`

h: 친구한테 같이 어울리자고 먼저 톡 내볼 수도 있고, 오랜 친구와 다시 연락한다던가, 아니면 그냥 카페 바리스타랑 얘기 나눌 수도 있는 거고.

`hong({ body:"normal" });`

h: 우린 우리가 생각하는 거 보다 좀 더 호감가는 사람일 지도 모르잖아.

`bb({ eyes:"annoyed" });`

[만약 이게 그저 작고 얉은 "성공"이라면 어떻게 해?](#act4_alone_experiment_cheap)

//What if these are small, cheap "wins"

[남에게 민폐끼치는 거라면 어떡해?](#act4_alone_experiment_burden)

[그치만 이런 담소는 우리의 *진짜*모습이 아니잖아!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: 얉은 미소만 짓고 있으면 다른 사람과 진정으로 이어지지 못할 거야.

`bb({ eyes:"super_sad" });`

b: *그치만*  본모습을 보이면 다른 사람들 모두 우리의 망가진 속모습을 보게 될 테고!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: 굴러.

b: 뭐.

`hong({body:"hands_1"})`

h: 개들이 사랑과 신뢰를 보여줄 때, 배를 보여줌으로써 위험에 노출시키잖아.

//When dogs want to show love and trust, they make themselves vulnerable by exposing their belly.

`hong({body:"one_up"})`

h: 어쩌면 우린 아직 그 정도 까지 안심할 수 있는 단계는 아니지만, 계속된 훈련으로

`hong({body:"normal", eyes:"surprise"})`

h: 언젠가 사람들에게 우리 본모습을 보여줄 수 있을 수도 있지. -망가졌어도 인간적인 본 모습을.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: 간식 주면 구를게.

`bb({ eyes:"normal", mouth:"normal" });`

h: 안돼.

(#act4_something_else)

# act4_alone_experiment_cheap

b: 바리스타한테 인사하는 게 인싸-올림픽 금메달감은 아니잖아.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: *우리* 자신을 위한 거지!

`hong({ body:"one_up", eyes:"annoyed" });`

h: 인싸 체육관에서 우리 체급은 페더급도 안될껄? 아마... 몰라, 쿼크급은 되려나?

`hong({ body:"normal", eyes:"normal" });`

h: 그런 얉은 성공이라도 뭐 어때. 1000번째 발걸음을 위해서는 첫 번째 발걸음이 필요한 법이잖아.

b: 그래! 인사하고 난 다음에 더 나아갈 수도 있지. 예를 들면...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"잘 지내시나요?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"별일 없어요!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: 바리스타는 그냥 커피나 만들고 싶어하는데 우리가 사회성이 얼마나 떨어지는지 *실험*하는 건 민폐 아닐까?

//Maybe the barista just wants to make some dang coffee, not be an *experiment* to see if our social skills suck.

`bb({ eyes:"annoyed" })`

h: 뭐, 정말로 우리가 *민폐*라면...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: 그래도 알게 돼서 좋은 거지!

`hong({ eyes:"normal" });`

h: 사전에 다른 사람에게 민폐될만한 건 뭔지 물어본다거나 다른 사람들의 선을 존중해주는 법도 배워갈 수 있는 거잖아.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: 왜 있잖아, 심리상담가들 책자에 써있는 "대인관계 기술"인가 뭔가 

//Y'know, all that "inter-personal skills" ^crap^ we see in counselor brochures.

(#act4_something_else)

# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: 네 도덕적 욕구를 채워주고 싶어 네가 더 좋은 사람이 될 수 있도록...

`bb({ eyes:"sad_d" })`

b: 근데 그저 우리 속 깊은 곳이... 근본적으로 망가져 있는 것 같아.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: 그리고 망가진 게 *아니*라고 할 생각 마. *옥상*에서 뛰어내렸잖아.
{{/if}}

{{if !_.INJURED}}
b: 그리고 망가진 게 *아니*라고 할 생각 마. *옥상*에서 뛰어내릴 뻔 했잖아.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: 모르겠네, *내가* 할 말 고르는 건 이쯤하자고. *넌* 어때, 인간?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: 다시, 네 차례야. 네 생각은 어때?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: 더 생각나는 거 없어, 인간?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[그래 망가져있네. 한번 고쳐보자.](#act4_bad_fix)

[그래 망가져있네. 받아들여보자.](#act4_bad_accept)

[고마.](#act4_thanks) `_.thanks_for = "도덕적 건강";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: 조금씩 좋은 습관을 기를 수도 있고, 우리가 가치있게 여기는 것과 우리 삶을 일치시켜 볼 수 있지.

`hong({body:"one_up"});`

h: 필요하다면 전문적인 도움도 얻어볼 수 있어 - 정신과 치료나 심리상담 같은 거.

`hong({body:"normal"});`

h: 우릴 고칠 방법은 있다구.

[하지만 우릴 전혀 고칠 수 없다면은?](#act4_bad_fix_cant)

[하지만 우릴 *너무* 고쳐 버린다면은?](#act4_bad_fix_too_much)

[전문적인 치료받을 돈도 없잖아.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: 그래, 네 말이 맞을지도 몰라.

h: 다 못고칠지도 모르지.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: 으아아 이럴 줄 알았어. 우린 망가져 있다고!

`hong({eyes:"surprise"});`

h: 그래도 뭐, 적어도 *덜* 망가져있을 수 있지.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: 상처는 시간이 지나면 나아지지만 흉터는 그대로 남지. 그래도 괜찮아.

//Scars heal with time, but they never go away. And that's okay.

`bb({eyes:"annoyed_r"});`

b: 그래 뭐, 게다가

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: 흉터는 *섹시*하다구.

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: 아 쫌 제발.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: 인정하기 구역질나지만... 내 일부는 이런 엉망을 *원하는* 거 같아.

`bb({ eyes:"angry" })`

b: 내 말은, 그거 없이는 *지루하지* 않겠어?

`bb({ eyes:"sad_r", body:"one_up" })`

b: 우리가 완벽하다면 우리의 예술은 밋밋하고 재미없게 되지 않을까?

//Without the disorder, won't our art become stale and bland?

`bb({ eyes:"sad_u", body:"two_up" })`

b: 우리가 정말 완전무결하다면 , 흠결 있는 우리 친구들과 이어지지 못하는 거 아닐까?

//Without the disorder, won't we be unable to connect with our friends who have the disorder?

`bb({ eyes:"sad", body:"chest" })`

b: 완벽한 우리 삶에 영원히 안주해버리면, 대단한 일을 하기 위한 노력을 그만두게 되는 거 아닐까?

`hong({ MOUTH_LOCK:true })`

h: ...

h: 만약 "두려울게 없어지는" 게 두렵다면...

h: 두려울 게 없어질 일은 없을 거 같은데.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: 오, 좋아! 휴! 다행이야!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "의사 선생님, 댁이 *그게 본인에게 어떤 기분이 들게 했나요?* 같은 질문이나 듣는데 시간당 몇만원씩 들어가서 게 불안해요"

//Doc, I'm anxious that I'm paying $100/hr just to hear you ask *how does that make you feel?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "으흠, 그래서 그게 본인에게 어떤 기분이 들게 하나요?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: 맞아, 합리적인 걱정거리지.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: 그리고 정신과 치료비를 누구나 감당할 수 있는 것도 아니라 참 별로야.

`hong({ eyes:"normal", mouth:"normal" });`

h: 그래도, 가격이 덜하거나 무료인 선택지도 있어:

`hong({ body:"chin" })`

h: 협력 단체라던가, 온라인 상담이라던가, 또래상담이나 비영리 보건소라던가...

`hong({ body:"hands_1" })`

h: 명상이나, 제때 잠드는 거라던가, 친구들과 규칙적으로 담소를 나누거나 새로운 걸 배우는 것 처럼 좋은 습관을 들여볼 수도 있고...

`hong({ body:"hands_2" })`

h: 도서관에 가서 검증된 심리치료법에 관한 책도 빌려 볼 수 있지...

`hong({ body:"one_up" })`

h: 이 게임 끝에 그런 정보들의 리스트가 쭉 있다고!

//There's a full list of resources at the end of this game!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: 음, 방금 *그* 제4의 벽은 오래 안 갔네

//Well *that* fourth wall didn't last long.

`hong({ body:"point" });`

h: 가끔은 서술적 관습보다 더 중요한게 있다구. 정신 건강 처럼 말이야.

(#act4_something_else)

# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: 내 말은, 그게 상담가들이 하는 말이잖아, 네 감정을 모두 받아들여라. 부정적인 감정들 까지. 그치?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: 잠깐.

["받아들인다는" 게 *포기한다는* 의미로?](#act4_bad_accept_give_up)

[""받아들인다는" 게 *괜찮다는* 의미로?](#act4_bad_accept_approve)

["받아들인다는" 게 *말 그대로*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: 마틴 루터 킹이 "어이구 버스 앞자리에 못앉는구먼, 그냥 받아들이지 뭐"라고 했을 거 같아?

`bb({ eyes:"angry_r", body:"two_up" });`

b: 왜 자립적 산업-복합체는 무슨 백기를 흔드는 게 심오한 지혜라도 되는 줄 아는 거람?

//Why does the Self-Help Industrial Complex think waving the white flag is some *profound wisdom?*

`bb({ eyes:"annoyed", body:"normal" });`

h: 내 생각에는 "받아들인다"는 게 문제 있다는 걸 직시하고 해결하기 쉽지 않다는 걸 인정한다는 의미에서 같아.

h: 하지만 바뀔수 있다는 의지를 포기할 필요는 없는 선에서

//But not necessarily giving up a commitment to change.

`bb({ eyes:"suspect" });`

b: 그럼 상담사들은 그런걸 *인정한다*고 해야지 *받아들인다*가 아니라.

`hong({ body:"chin", eyes:"annoyed" });`

h: 그래, 생각해보니 "받아들인다"는 용어는 좀 헷갈리네.

`bb({ eyes:"closed", mouth:"narrow" });`

b: 뭐, 그건 *인정*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: 우리가 망가져 있는 게 *괜찮은* 거라고? 싫어!

`bb({ eyes:"angry_r", body:"one_up" });`

b: 망할 헐리웃 극작가들이 무슨 정신병 있는 걸 미화시키는데 다 거짓부렁이야!

`bb({ eyes:"angry", body:"two_up" });`

b: 정신적 장애가 있는 건 정말 *별로*라고! 사람들의 *삶*을 앗아가는데! 그런걸 왜 "받아들여야" 해?!

`bb({ body:"normal" });`

h: 내 생각엔 "받아들인다는" 게 참을성 있게 보라는 거 같아.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: 왜 뻘밭에 빠졌을 떄 더 움직이면 더 깊숙히 빠지잖아, 가만히 누워있어야 빠져나올 수 있고.

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: 너, 내 공포와 싸우는 것은 결국 날 옥상에서 뛰어내리게 했지.
{{/if}}

{{if !_.INJURED}}
h: 너, 내 공포와 싸우는 것은 결국 날 옥상에서 뛰어내릴뻔 하게 했지.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: 대신에, 해결방안은 우리가 지금 하는 이거야. 싸우지 말고 침착하게 함께 있기.

//Instead, the solution is to do what we're doing now – not to fight, but to patiently be with each other.

`bb({ eyes:"annoyed" });`

b: 그럼 "받아들인다"같은 문제있는 용어가 아니라 *그렇게* 말했어야지.

`hong({ body:"chin", eyes:"annoyed" });`

h: 생각해보니 그러네. "받아들인다"는 좀 그렇다.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: "받아들인다"니, 받아드릴 수 없어!.

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: 그치만 날 말 그대로 대해선 안된다는 거 우리 모두 *알잖아*! 

`bb({ eyes:"sad_u", body:"two_up" });`

b: 애초에 이 모든 *문제*가, 나는 널 돕고 싶은데 내가 그걸 제대로 전달하는 데 젬병이라서 그런 거라구!

//The whole *problem* is that I want to help you, but I suck at using words to do so!

`bb({ eyes:"sad", body:"normal" });`

h: 내 생각엔 상담가들이 말하는 "받아들인다"는 게 감정과 싸우지도, 무시하지도 말라는 의미에서 같아.

`hong({ eyes:"surprise", body:"one_up" });`

h: 네 말을 듣고, 너와 협력하는 것. 그렇지만 네 말을 100% 곧이 곧대로 알아듣지는 말고.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: 그럼 상담가들은 *그렇게* 말할 것이지. 무슨 애매모호한 "받아들인다"같은 말 말고 말이야.

`hong({ body:"chin", eyes:"annoyed" });`

h: 상담가들도 전달하는 데는 영 젬병인가보지 뭐.

(#act4_something_else)

# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: 어쨌든, 더 할 말은 없고?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: 그래서, 이제 가슴에서 털어낼 건 더 없어? 
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

[아냐, 이제 좀 괜찮아.](#act4c_prelude)

# act4_something_else_2

h: 좋아, 우리가 가진 공포에 대해서 다 다뤄봤네.

b: 그래. 딱 세 가지 공포지

h: 맞아, 딱 세 가지.

b: 편하구만.

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

b: 이건 무슨 *게임*같은 게 아닌 거 알지?

`bb({eyes:"angry_d", body:"one_up"})`

b: 네 감정과 건강한 관계를 맺는 건 컴퓨터 화면에 마우스나 딸깍거리는 것 마냥 간단한 게 아니라고.

`bb({eyes:"sad", body:"normal"})`

b: 정말 우리가 잘 어울릴 수 있을까?

b: 정말 우리가 한 팀으로서 협력할 수 있을까?

`hong({eyes:"sad", body:"one_up"})`

h: 글쎄,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: 저, 저기...

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

a: 옆에서 같이 좀 먹어도 괜찮을까?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *얘*한테 반해 있는 거라고? 왜 뭔 싸이코 킬러마냥 앉아있는 거래?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: 네가 반한 애한테 같이 앉아도 되냐고? 완전 *구질구질*해 보이는 거 알아?!

//Asking your crush if you can sit with them? Do you know how *needy* we sound?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *얘*한테 반해있다고? 가만히 있는데 괜히 방해했잖아! 우린 정말 민폐덩어리야!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: 그, 그게- 안괜찮다면 뭐, 그저...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[잠깐 우리 파티에서 보지 않았나?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[그래, 좋아! 여기 앉아.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[미안해, 지금은 좀 혼자 있고 싶어서.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: 맞아 처음 간 파티때 소파에 있었잖아!

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: 내가 파티 호스트한테 죽빵날린 그 때 말이야.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: 내가 패닉상태에 빠져서 울면서 뛰쳐나간 그 때 말이야.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: 인간, 잠시만. 우리가 쟤 불편하게 하는 거 같은데.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: 앗, 불편하게 하려는 건 아니었어!

`publish("act4", ["hong_to_alshire",4]);`

h2: 그냥 익숙한 얼굴이길래. 그게 다야.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: 으아아아! 이럴 줄 알았어! 쟤는 위험한 패닉에 빠지는 싸이코라고!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: 으아아아! 첫 인상이 "트라우마를 목격함"이라니! 우릴 싫어할 게 뻔하잖아!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: 으아아아아! 트라우마를 떠올리게 했어. 우리 존재만으로도 상처가 된다고.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: 인간, 잠시만. 쟤 좀 불편해 보이는데.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: 아, 물론 강요하는 건 아니야!

`publish("act4", ["hong_to_alshire", 4]);`

h2: 그냥 여기 원한다면 앉아도 된다고.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: 너무 친절하게 대하잖아! 연쇄살인마일지도 몰라!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: 그냥 친절한 척하는 거야! 우리랑 *진정* 가까이 지내고 싶은 사람은 없다고!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: 아아아아 우린 맨날 남 어색하게만 만들어! 우린 이 지구의 더러운 얼룩이라고!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: 인간, 잠시만. 우리가 쟤 불편하게 하는 건 아닐까?

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: 아, 무례하게 말하려던 건 아냐!

`publish("act4", ["hong_to_alshire", 6]);`

h2: 그냥 내 생각 좀 정리해야 해서 그래. 네가 싫어서 그랬다고 생각하진 말아줘.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: 대체 무슨 뒤틀리고 역겨운 생각을 정리해야하길래?! 저 싸이코의 음침한 욕망을 채우는 게 뭐길래?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: 우리가 싫대! 우린 절대 사랑받지 못할 거야!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: 우리가 쟤 생각 정리하는 걸 방해해버렸어! 이제 트라우마가 남을 거고 이건 전부 우리 탓이야!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐 도망쳐

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

h: 흠, 그거 이상하네. 대체 무슨 생각이 오가고 있던 걸까나.

//Huh. That was weird. I wonder what was going on in their head.

`publish("act4", ["hong_closer", 2]);`

h: 어쨌든 어디까지 했지?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: 어 까먹었어. 무슨 팀이랑 협력에 관한 거였는데?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: 사람들 말로는 자기 감정과 "화해"해야한다는데... 마치 무슨 감정을 *전쟁 범죄자*마냥 말이야

`publish("act4", ["bb_closer", 7]);`

b: 그치만 난 화해하는 것 보다 더 바란다고! 우리가 *동맹*이었으면 좋겠어!

`publish("act4", ["bb_closer", 3]);`

b: 좋은 경비견이 되고 싶어. 마치 배고픔이나 목마름이 네 생리적 욕구에 대한 알람인 것처럼,

`publish("act4", ["bb_closer", 8]);`

b: 나도 네 심리적인 욕구에 대한 알람이 되고 싶다고. 안전해지고 싶은 욕구, 소속되고 싶은 욕구, 더 나은 사람이 되고 싶은 욕구

//I want to be the alarm for your *psychological* needs – your needs for safety, belonging, goodness.

`publish("act4", ["bb_closer", 1]);`

b: 근데... 난 내 일을 잘 못해, 그래서 네가 날 훈련시켜줘야 해.

`publish("act4", ["bb_closer", 4]);`

b: 난 "항상 타당"하지도, "항상 비합리적"이지도 않아. 난 단지 최선을 다하는 것 뿐이야. 그니까, 부탁이야,

`publish("act4", ["bb_closer", 30]);`

b: 널 도울 수 있게 날 도와줘!

`publish("act4", ["bb_closer", 6]);`

b: 다만, 나이 든 개에게 새 재주를 가르쳐 주는 건 분명 *꽤* 걸릴 거야. *몇년*이 걸릴 지도 몰라.

`publish("act4", ["bb_closer", 3]);`

b: 그리고 가끔은 예전으로 되돌아가겠지, 예전 습관이 나와 버릴지도 몰라.

`publish("act4", ["bb_closer", 2]);`

b: 그림자한테 짖어대고. 말로써 네게 겁줄 지도 몰라. 어쩌면 보기... 거슬리는 이미지를 보여줄수도 있고. 

`publish("act4", ["bb_closer", 9]);`

b: 미안해! 난 상처 받은 떠돌이 개야! 가끔 네 침대에 똥싸대는 똥개!

`publish("act4", ["bb_closer", 4]);`

b: 그치만 날 침착하게 대해준다면... 그리고 나랑 함께 있어 준다면...

`publish("act4", ["bb_closer", 8]);`

b: 어쩌면 이 늑대를 길들일 수도 있지.

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
b: 으아아아 흰빵 더 먹고 있잖아 으아아아아
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
