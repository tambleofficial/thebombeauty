# THE BOM BEAUTY — Cloudflare Pages 배포

1. 이 폴더 내용을 GitHub 저장소 루트에 올립니다.
2. Cloudflare Pages → Create project → Connect to Git → 저장소 선택
3. Framework preset: None / Build command: (비움) / Build output directory: `/`
4. 배포 후 Custom domains에서 도메인 연결

도메인이 thebombeauty.com 이 아니면 sitemap.xml, rss.xml, robots.txt, index.html(canonical·og:url)의 주소를 바꿔 주세요.

페이지 주소: / · /brand · /program · /correction · /cases · /contact

## 관리자(편집 모드)

- 주소: /edit (비밀번호 로그인). 글자는 눌러서 고치고, 사진은 눌러서 바꾼 뒤 "저장하기".
- 저장하면 content/text.json(문구), content/media.json(사진)과 assets/uploads/ 에 기록되고 1분 안쪽으로 홈페이지에 반영됩니다.
- Cloudflare Pages 환경 변수: GITHUB_TOKEN(이 저장소 Contents 읽기·쓰기), CMS_PASSWORD(편집 비밀번호).

## 구조

- index.html + assets/b/*.html: 페이지 구성 파일(원래 한 파일 번들을 풀어 놓은 것).
- assets/slot-state.js + assets/slots/: 사진 칸 위치·확대 정보와 사진 파일.
- assets/fonts/: Pretendard 글꼴(화면에 쓰인 글자 묶음만 받음).
