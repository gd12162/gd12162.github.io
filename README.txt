
# V4A Root Production Package (UMD build)

**대상:** GitHub Pages 사용자 사이트 루트 (https://USERNAME.github.io/)

## 배포
1) 저장소 이름을 USERNAME.github.io 로 생성
2) 이 폴더의 모든 파일을 루트에 업로드:
   - index.html, sw.js, manifest.webmanifest, .nojekyll, /icons
3) Settings → Pages → Deploy from a branch (main / root) 활성화
4) Safari로 https://USERNAME.github.io/ 접속 → 홈 화면에 추가

## 업데이트(캐시 무효화)
- `sw.js`의 `CACHE_NAME`을 v2, v3… 으로 변경 후 커밋
