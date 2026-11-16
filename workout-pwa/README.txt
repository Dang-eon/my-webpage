운동 기록 PWA 설치 방법

1. 이 폴더의 파일 전체를 https 주소로 호스팅합니다. (PWA는 https에서만 설치됩니다)
   - 예: Netlify Drop(app.netlify.com/drop)에 폴더를 끌어다 놓기, GitHub Pages, Cloudflare Pages 등
2. 스마트폰에서 발급된 주소를 엽니다.
   - iPhone(Safari): 공유 버튼 → 홈 화면에 추가
   - Android(Chrome): ⋮ 메뉴 → 앱 설치 또는 홈 화면에 추가
3. 한 번 열면 이후에는 인터넷 없이도 실행되고, 기록은 기기 안(LocalStorage)에 저장됩니다.

파일 구성
- index.html : 앱 본체
- manifest.webmanifest : 앱 이름, 아이콘, 실행 방식 정보
- sw.js : 오프라인 실행을 위한 서비스워커 (앱을 수정해 다시 올릴 때는 VERSION 숫자를 올리세요)
- icon-*.png : 홈 화면 아이콘
