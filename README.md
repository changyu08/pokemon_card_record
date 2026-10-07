# 포켓몬 카드 전적 일지 — PWA

기존 전적 일지 HTML을 기반으로 만든 Progressive Web App 버전입니다.

## 구성
- index.html: 기존 전적 일지 기능 + 모바일 하단 탭 + PWA 등록
- manifest.json: 홈 화면 설치 정보
- sw.js: 오프라인 캐시
- icons/: PWA 아이콘
- pokemon-bw.otf: 기존 폰트가 필요합니다
- pokemonicons-sheet.jpg: 기존 포켓몬 스티커 시트가 필요합니다

## 실행
PWA의 Service Worker는 일반적으로 HTTPS 또는 localhost에서만 동작합니다. 따라서 index.html을 파일 탐색기에서 직접 여는 것보다 웹 서버로 실행하세요.

예: Node.js가 있다면 프로젝트 폴더에서

npx serve .

또는 Python이 있다면

python -m http.server 8000

실행 후 PC에서 http://localhost:8000 으로 접속합니다.

실제 휴대폰에서 설치하려면 HTTPS로 호스팅하는 것이 가장 간단합니다. GitHub Pages, Cloudflare Pages, Netlify 등의 정적 호스팅에 이 폴더를 그대로 배포할 수 있습니다.

## 기존 자산
pokemon-bw.otf와 pokemonicons-sheet.jpg가 현재 폴더에 없으면 기존 웹 프로젝트에서 같은 파일을 복사하세요. 둘 중 하나가 없으면 폰트 또는 포켓몬 스티커가 정상적으로 표시되지 않습니다.
