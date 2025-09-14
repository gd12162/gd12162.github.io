# V4A Root Production Package (GitHub Pages user site: https://USERNAME.github.io/)

1) 저장소 이름을 사용자 사이트 형식으로 생성: USERNAME.github.io
2) 이 폴더의 모든 파일을 루트에 업로드:
   index.html, sw.js, manifest.webmanifest, .nojekyll, /icons
3) Settings → Pages → Deploy from a branch (main / root) 활성화
4) Safari로 https://USERNAME.github.io/ 접속 → 홈 화면에 추가

오프라인 캐시 갱신: sw.js의 CACHE_NAME 값을 v3, v4…로 변경 후 커밋