
# V4A Root Production Package (UMD + IndexedDB + Image Compression)

**대상:** GitHub Pages 사용자 사이트 루트 (https://USERNAME.github.io/)

## 배포
1) 저장소 이름을 USERNAME.github.io 로 생성
2) 이 폴더의 모든 파일을 루트에 업로드:
   - index.html, sw.js, manifest.webmanifest, .nojekyll, /icons
3) Settings → Pages → Deploy from a branch (main / root) 활성화
4) Safari로 https://USERNAME.github.io/ 접속 → 홈 화면에 추가

## 주요 개선
- 상태 저장을 IndexedDB 우선(로컬스토리지 폴백)으로 변경 → 큰 이미지도 안전
- 업로드 이미지를 1280px로 축소 후 JPEG로 저장 → 용량 절감
- iOS 카메라 빠른 접근을 위해 <input capture="environment"> 추가
- 간단한 토스트 메시지/에러 처리

## 업데이트(캐시 무효화)
- `sw.js`의 `CACHE_NAME`을 v3, v4… 으로 변경 후 커밋
