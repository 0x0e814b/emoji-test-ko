# Emoji-Test-Translate

unicode.org에서 제공하는 [emoji-test.txt](https://www.unicode.org/Public/emoji/16.0/emoji-test.txt) 한글화 파일.
기계번역 및 일부 의역으로 번역이 부정확 할 수 있습니다.

개인 용도로 번역 하였으나 혹시 필요하신 분들 계실까봐 공유합니다.


## CodeFormat

`CodePoint ; status # emoji version description:extra`

## ParseExample (JS)
```js
// codeline = "1F469 1F3FB 200D 1F9B2 ; fully-qualified # 👩🏻‍🦲 E11.0 여성: 밝은 피부톤, 대머리"
const [
  _matched,
  codepoints,  // 1F469 1F3FB 200D 1F9B2
  status, // fully-qualified
  emoji, // 👩🏻‍🦲
  version, // 11.0
  description //  여성: 밝은 피부톤, 대머리
] = codeline.match(/^(.+?)\s+;\s+([\w-]+)\s+#\s+(\S+)\s+E(\S+)\s+(.+)/);
```
