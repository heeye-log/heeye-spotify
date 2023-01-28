
### Introduction
- 기간 : 2023.01.17 - 2023.01.18
- 스포티파이(KR) 클론 사이트 만들면서 학습하기

### Demo
- 실제 사이트 👉🏻 [Spotify_ko](https://www.spotify.com/kr-ko/)<div>
- 만들어본 Demo 👉🏻 [Spotify](https://heeye-log.github.io/spotify-website/)</div>

### Troubleshooting
- 메인 화면 중 안드로이드/ios 이미지 높이 CSS 속성값을 넣어도 같은 높이로 위치가 되지 않고 이미지 하나가 꼭 위로 튀어 올라가는 문제가 있었다.
- 따라서 찾아본 결과 img와 텍스트 높이 맞추는 vertical-align 속성을 걸어주니 높이가 일치하게 적용 되었다.
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

### Retrospect
- 
