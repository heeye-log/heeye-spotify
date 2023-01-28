
### Introduction
- 기간 : 2023.01.17 - 2023.01.18
- 스포티파이(KR) 클론 사이트 만들면서 학습하기

### Demo
- 실제 사이트 👉🏻 [Spotify_ko](https://www.spotify.com/kr-ko/)<div>
- 만들어본 Demo 👉🏻 [Spotify](https://heeye-log.github.io/spotify-website/)</div>

### Troubleshooting
- 메인 화면 중 안드로이드/ios 이미지 높이가 CSS 속성값을 넣어도 같은 높이로 위치가 되지 않고 이미지 하나가 꼭 위로 튀어 올라가는 문제가 있었다.
- 따라서 찾아본 결과 img와 텍스트 높이 맞추는 vertical-align 속성에 대해서 알게 되었고 보통은 텍스트와 이미지 높이로 top 속성값을 쓰지만, 내 케이스의 경우 이미지에 대한 사이즈 및 높이 차이 때문에, middle 속성값을 주었더니 일치하는 것을 확인 했다.
---
- 수정 전 CSS
```
.button-icon{
  text-align: auto;
  overflow: hidden;
```
- 수정 후 CSS 
```
.button-icon{
  text-align: auto;
  overflow: hidden;
  vertical-align: middle # 수정
}
```
---
### Retrospect
- 여태까지 기초적인 내용 학습을 할 겸 주어진 사이트 이미지가 아닌 현재 시점에 실제 적용되어 있는 스포티파이 기준으로 클론 제작을 하고 싶어 진행하게 되었다.
- 위와 같이 CSS 속성값을 찾아봐야 하는 케이스도 있었고, 이게 맞는지 고민하면서 메인 사이트 폼을 맞춰갔던 것 같다. 
- 현재 flexbox 및 meta 속성을 넣지 않아, 디바이스 웹에서 봤을 땐 하단 메뉴 한줄 나열 현상 발생하는 것 확인하였다.
