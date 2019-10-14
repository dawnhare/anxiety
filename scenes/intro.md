# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

```
_.PLAYED_BEFORE = !!window.localStorage.continueChapter;
```

{{if !_.PLAYED_BEFORE}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if !_.PLAYED_BEFORE}}
[#play1# 시작! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act2"}}
[_이어하기_: 파티](#act2) `publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act3"}}
[_이어하기_: 또 다른 파티](#act3) `publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act4"}}
[_이어하기_: 또 다른 샌드위치](#act4) `publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
[#play1# 다시 시작! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE}}
[챕터 선택](#chapter-select) `Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

[(제작 노트)](#intro-play-button) `Game.OVERRIDE_CHOICE_LINE=true; publish('show_cn');`

# chapter-select

`publish("HACK_chselect");`

[I. 샌드위치](#intro-start) `publish("HACK_chselect_end"); publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

[II. 파티](#act2) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`

{{if window.localStorage.act3}}
[III. 또 다른 파티](#act3) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act3}}
[III. 또 다른 파티]()
{{/if}}

{{if window.localStorage.act4}}
[IV. 또 다른 샌드위치](#act4) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act4}}
[III. 또 다른 샌드위치]()
{{/if}}

{{if window.localStorage.credits}}
[V. 크레딧](#to-credits) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.credits}}
[V. 크레딧]()
{{/if}}

[(메인 메뉴)](#intro-play-button) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`

# to-credits

`stopAllSounds();`

(...101)

(#credits)

# intro-start

(...500)

`clearText()`

n3: 환영합니다! 사실 이건 "게임"이라기보다는 대화 형식의 이야기에요. 글 읽기 좋아했으면 좋겠네요, '멍충'씨!

n3: 시작하기 전에 어떻게 *읽는 걸* 좋아하시나요?

`publish("show_options_bottom")`

# intro-start-2

n3: 좋아요! 참고: 아래 ⚙ 아이콘을 누르면 언제든지 설정을 바꿀 수 있어요. 그리고 매 챕터마다 자동 저장된답니다!

n3: 그럼, 이야기를 시작하죠...

`clearText()`

(...1000)

`publish("intro-to-game-2")`

n2: 이것은 인간입니다.

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`
