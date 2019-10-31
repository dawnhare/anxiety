# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: 짠!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *캬아* 그래 바로 이거야.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: 있잖아 꼬맹아...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: 자세히 말하자면 내 좌우편도체에 딱 꽂히네.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: 널 보면 내가 어렸을 적이 생각나. 내 머릿속의 동물한테 휘둘려서 고통받던 때 말야.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: 내 동물을 죽였듯이, 네 동물을 죽이는 걸 도와줄 수 있어서 정말 다행이야.

```
publish("act3",["roofhunter",2]);
```

r: 자, 여기서 진실 혹은 도전--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: 도저언!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: 하하! 좋았어.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: 자, 저기 아래 하늘색 수영장 보이지?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: 6층 아래에 있는 저거?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: 저기로 뛰어들어

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: 잠깐, 뭐라고?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: 네 동물이 또 징징대기 시작했지, 그렇지?

```
publish("act3",["roofhunter",23]);
```

r: *안돼애애애 위험해애애 그러지 마아아아.*

```
publish("act3",["roofhunter",22]);
```

r: 바로 그것 때문에 아슬아슬한 스릴이 필요한 거라고! 파티를 즐겨! 카르페 디엠! 코카인을 코로 먹는 것처럼 즐겨보자고. #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: 그 동물이 뭐라 ^씨부리^던 우린 ^좆도^ 신경 안쓴다는걸 보여주라고! 자, 뛰어.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: 어.. 그치만, 음... 가끔 두려움도 옳을 텐데...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: 미안한데, 너도 그 아프니까 *청춘이라나* 뭐라나 하는 그 쿨병 걸린 유행에 속은 거야?

```
publish("act3",["roofhunter",17]);
```

r: 쾌락은 고통의 반대라고. 그래서 ^씨발,^ 고통을 이겨내기 위해 쾌락을 좀 쓸 수도 있는 거지!

```
publish("act3",["roofhunter",18]);
```

r: 대체 왜 저 실리콘 밸리의 유사 불교도 ^새끼^들은 이걸 이해못하는 거야?

```
publish("act3",["roofhunter",6]);
```

r: 꼬맹이, 그 동물이 우리 같은 사람들을 *아프게* 한다는 거 알고 있어. 우리들을 *고문*하고 있는 거라고.

```
publish("act3",["roofhunter",19]);
```

r: 그딴 건 우리 친구가 아냐. 미친 짐승일 뿐이지. 그말인 즉슨 *마취시켜* 버리던가,

```
publish("act3",["roofhunter",20]);
```

r: 아니면 *대가리에 총알을 박아넣어야지*.

```
publish("act3",["roofhunter",27]);
```

r: 안그러면 걔만 이기게 냅두는 셈이야.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: 그래, 틀렸어.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
    music('battle_dark_loop');
});
```

h2: 그 자식이 이기게 두지 않을 거야.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: ^씨발^ 바로 그거야! 널 믿어, 짜샤! 죽여버리라고! <3

(#act3a)

# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: 안돼 안돼 안돼 안돼

n: 이 챕터에는 두 가지 엔딩이 있습니다. 그중 하나는 *매우, 매우 끔찍한 엔딩*이죠.

b: 안돼 안돼 아니야 이건 아니라고 안돼 안돼 안돼 안돼 안돼

n: 신중하게 선택하고 인간을 보호하세요.

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: 으아아아아아아아아아

`bb({ mouth:"normal" });`

n: 행운을 빕니다.

```
Game.clearText();
bb({ eyes:"start" });
```

[인간, 이러다 정말로 죽을 수도 있어!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[이건 멍청한 짓이야. 너 스스로를 망치는 거라고!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[이 미친 녀석들은 네 진짜 친구도 아니잖아!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: 인ㄱ-

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: 이ㄱ-

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: 이 ㅁ-

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: 있지, 네가 수천만번씩이나 그러지 않았다면... 네 말을 믿었을지도 몰라

h: 넌 양치기-소년 아니, 양치기-늑대일 뿐이야.

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: 그것도 이미 해 본 거잖아.

b: 인간, 제발...

`hong({ eyes:"look_right" });`

h: 하, 이거 참 거대 제약회사들이 내 자가치유법을 인정해주지 않아서 저어엉말 *유감인데* 말야,

h: 잘 봐봐 이 ^개새끼^야, 우리*모두*  널 ^닥치^게 할 방법 하나쯤은 있다고.

`hong({ body:"look_up", eyes:"look_up" });`

h: 누군가는 일에 미친듯이 열중할 테고.

`hong({ body:"look_down", eyes:"look_down" });`

h: 누군가는 ^성관계^나 마약에을 하든가, 아니면 페이스북 피드나 갱신하겠지.

`hong({ body:"normal", eyes:"look_right" });`

h: 누군가는 다른 사람들의 관심 받는 거에 투신할수도 있고. 

`hong({ eyes:"angry" });`

h: 난 자의적으로 저 수영장에 뛰어들 거야.

[넌 지금 취했고 저기는 여긴 6층이란 말이야!](#act3_bad_1_harm)

[젠장, 이딴 게 내 노력에 대한 보답이라고?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[알았어, 인정할게. 내가 다 망쳤어.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: 물에 착지한다고 해도, 표면 장력때문에 *적어도* 갈비뼈 부러지고 뇌진탕에도 걸릴 거라고! 

h: 으.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: 유튜브에서 러시아 사람이 이거 하는 거 본 적 있어.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: 이, 뭐라고? *보다압?*

`bb({ eyes:"angry" });`

b: 이래서 내가 *존재* 하는 거야! 인간은 자기 스스로 지키도록 맡길 수가 없으니까!

b: 그동안 내 일생을 바치면서까지 모자란 너를 지키려고 노력했는데 지금 너는-

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: 허.

`hong({ body:"laugh_2" })``

h: 하하하!

`hong({ body:"laugh_3" })``

h: 으하하하하!

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: 와 진짜, ^씨발^ 고작 그 정도로 다 표현이 안되지!

`hong({ body:"yell_2" });`

h: 그래, 이 썩어가는 핏덩어리같은 ^새끼야!^ 네가 ^존나^ 망쳤고 말고!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: 더 말할말 없어? 대장 "너무 뻔한"

[그렇지만 나한테 복수하는 건 정답이 아니야!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[하지만 이번엔 내가 *정말로* 옳아!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[난 네게 상처를 줬어.](#act3_good_2a)

# act3_good_1_fail_revenge

b: 네 감정과 건강한 관계를 만들어야지, 들리지 않도록 삼켜버릴 게 아니-

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1_fail_harm

b: 부탁이야, 그 병 내려놓고 이제-

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_bad_2

`bb({ eyes:"sad" });`

b: 제발... 이러지 마...

h: 네 HP 정말 낮아 보인다, 늑대야.

h: 나라면 이 다음 할 말을 신중하게 고를 거야.

`bb({ eyes:"normal" });`

[좋아. 널 지켜주는 것도 여기까지야.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[난 줄곧 옳았어.](#act3_bad_2_right)

[미안해.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_2_jump

b: 어디 한번 뛰어봐, 내가 신경 쓰나 봐라.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: 좋아 그럼, 원샷!

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: 잠깐만! 안돼! 방금 그건 반심리학이야! 내가 말한 *반대로*할줄알고 말한-

(#act3_bad_3)

# act3_bad_2_right

`bb({ eyes:"angry" });`

b: 지금 *너는* 스스로를 위험에 빠뜨리고 있어. 그 친구라는 작자들도 널 *이용*하고 있고 너도 걔를 *이용*하는 것일 뿐이잖아.

`bb({ eyes:"sad" });`

b: 인간.... 제발, 왜 내 말은 안믿어 주는 거야?!

h: 네가 *나를* 믿어준 적이 없으니까

(#act3_bad_3)

# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: 다른 '경비-늑대'들의 주인은 참을성있게 우리를 훈련시켜줘, 서로 협력하는 법을 배워간단 말이야.

b: 지켜주려 노력하는 '경비-늑대'를 싫어하는 게 아니라! 근데 왜 너는 그렇게--

`bb({ eyes:"normal" });`

h: 틀렸어 이 ^개새끼^야

(#act3_bad_3)

# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"우리가 가장 두려워할 것은 두려움 그 자체."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"돈 워리, 비 해피!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: 이 시대 지혜로운 사람들은 다 동의하지. 부정적인 감정은 *나쁜* 거라고!

`hong({ eyes:"less_angry" });`

h: 당연하지! 아니면 왜 *부정적인* 감정이라 하겠어?

b: 인간... 제발...

`hong({ eyes:"normal" });`

h: 예전에 내가 말했지. “이 고통에서 자유로워지고 싶다”고

h: 내 소원대로 됐어. 더이상 고통도, 두려움도 불안감도 느껴지지 않아...

h: 그 무엇도, 전혀 느껴지지 않아.

`_.a3_ending = "jump";`

(#act3_end)

# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: 다른 것들이 널 다치지 않도록 하는 데에 집착하느라 *내가* 널 해치고 있다는 걸 몰랐어.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: 아니. 씨^발^.

`hong({ body:"yell_1" });`

h: 그걸 알아차리는데 이렇게나 ^존나^ 오래 걸렸냐?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: 진작에 알았으면 그동안 이렇게까지 힘들지도 않았을 거라고 이 멍청한 ^개새^야. 왜 이제야 그걸 깨달은 거야?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)

# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...*미안*하다고?

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: *뭐가* 그렇게 미안한데?

(#act3_good_2q)

# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}

# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[좋은 보호자가 되어주지 못해서 미안해.](#act3_good_3_protector)

[널 존중해 주지 않아서 미안해.](#act3_good_3_respect)

[미안해.](#act3_good_4)

# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[주인이 끔찍한 사람이라 정말 미안해.](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[널 존중해 주지 않아서 미안해.](#act3_good_3_respect)

[널 아프게 해서 미안해.](#act3_good_3_hurt)

# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: 널 *진짜* 위협으로부터 지키는 게 내 역할인데, 계속 지나가는 차랑과 우체부한테 짖어댄 꼴이었어.

`bb({eyes:"sorry_up"});`

b: 그림자한테 짖고. 너무나도 많이 짖어댔지.

`bb({eyes:"sorry"});`

b: 네가 나한테 입마개를 씌우려 한 게 당연했을 정도야.

`bb({eyes:"sorry_down"});`

b: 미안해.

(#act3_good_4)

# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: 난 *너의* 충직한 경비-견이 되었어야 했는데 마치 네가 *나한테* 복종해야 하는 것마냥 행동했어. 

`bb({eyes:"sorry_up"});`

b: 보호자와 간수 사이에는 큰 차이가 있어. 그리고 난 그 선을 넘어버렸어.

`bb({eyes:"sorry_down"});`

b: 미안해.

(#act3_good_4)

# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: 네가 다치지 않도록 지키는데에 너무 집착한 나머지, *내가* 널 아프게 하고 있었다는 걸 생각하지 못했어.

`bb({eyes:"sorry_up"});`

b: 난 정말 나쁜 개였어.

`bb({eyes:"sorry_down"});`

b: 미안해.

(#act3_good_4)

# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: 그래 뭐 어차피 이건 멍청한 생각이야.

h: 널 망쳐보려고 해본 건데, 뭐, 그렇게 됐네.

h: 이번 판은 무승부로 치자. 어때?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: 좋아.

h: 좋아.

n: *무승부*

`_.a3_ending = "walkaway";`

(#act3_end)

# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}

# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: 아 *쫌*. 그동안 그 동물이 한 짓을 생각해봐. 그냥 이렇게 *포기*한다고?

r: 왜 그래, 꼬맹아? *무섭기라도* 하냐?

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: 그래.

h2: 무서워.

`publish('hong-next')`

h2: 그래도 괜찮아!

`publish('hong-next')`

h2: 무서워해도 괜찮다고.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: 어..? 방금 문 잠근 거 같은데?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)

# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: 제발...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: 그러지 마...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: 안돼!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
