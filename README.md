🎮 PC-Cafe Kiosk Project

PC방 키오스크를 웹으로 구현한 미니 프로젝트입니다.
HTML, CSS, JavaScript를 활용하여 메뉴 선택 → 장바구니 → 결제 방식 선택 → 결제 완료까지의 흐름을 구현했습니다.

📌 프로젝트 소개

이 프로젝트는 실제 PC방 키오스크처럼:

메뉴 카테고리 선택

음식/음료 담기

총 금액 자동 계산

카드 / 현금 결제 분기

약관 동의 체크

결제 완료 알림

기능을 구현한 웹 기반 키오스크입니다.

🛠 사용 기술

HTML

CSS

JavaScript (Vanilla JS)

window.open() 을 이용한 결제창 분리

dataset 속성을 이용한 가격 관리

DOM 조작 및 이벤트 처리

📂 프로젝트 구조
PC-cafe/
│
├── PC-cafe.html        # 메인 키오스크 화면
├── receipt1.html       # 카드 결제 페이지
├── receipt2.html       # 현금 결제 페이지
│
└── menu/               # 메뉴 이미지 폴더
    ├── ramen1.jpg
    ├── side1.jpg
    ├── dinner1.jpg
    ├── drink1.jpg
    └── ...


※ menu 폴더 안에 이미지 파일들을 모두 넣어주세요.

🚀 실행 방법

프로젝트를 다운로드 또는 clone 합니다.

git clone https://github.com/your-id/PC-cafe.git


PC-cafe.html 파일을 브라우저에서 실행합니다.

🎯 주요 기능
1️⃣ 메뉴 카테고리 선택

라면류

사이드류

식사류

음료류

버튼 클릭 시 해당 메뉴만 표시됩니다.

2️⃣ 메뉴 선택 기능

메뉴 이미지를 클릭하면 confirm 창이 나타납니다.

확인을 누르면 장바구니에 추가됩니다.

data-value 속성을 이용해 가격을 추출합니다.

총 금액이 자동 계산됩니다.

this.dataset.value

3️⃣ 결제 방식 선택

카드 결제

현금 결제

체크박스 하나만 선택 가능하도록 처리하였습니다.

4️⃣ 카드 결제 페이지 (receipt1.html)

카드사 선택

전체 약관 동의 기능

약관 동의 후 결제 가능

결제 완료 2초 후 알림

5️⃣ 현금 결제 페이지 (receipt2.html)

현금결제 / 계좌이체 선택

약관 동의

현금영수증 발행 여부 체크

결제 완료 알림

💡 구현 포인트
🔹 window 객체를 통한 데이터 전달
let money = window.open("receipt1.html");
money.myvalue = sum.value;


부모창 → 자식창으로 결제 금액을 전달하였습니다.

자식창에서는:

window.myvalue


로 금액을 받아 사용합니다.

🔹 DOM 조작

getElementById

getElementsByClassName

innerHTML

style.display

checked

등을 활용하여 UI를 동적으로 제어했습니다.

📸 프로젝트 화면
🖥 메인 화면

(여기에 메인 화면 스크린샷 삽입)

💳 카드 결제 화면

(여기에 카드 결제 화면 스크린샷 삽입)

💵 현금 결제 화면

(여기에 현금 결제 화면 스크린샷 삽입)

🔮 개선 가능 사항

체크박스를 radio 버튼으로 변경

메뉴 수량 추가 기능

장바구니 삭제 기능

실제 결제 API 연동

반응형 UI 적용

로컬스토리지 활용

결제 완료 후 메인화면 자동 이동

📚 학습 목표

이 프로젝트를 통해:

DOM 구조 이해

이벤트 처리 방식

window 객체 이해

데이터 전달 방식

프론트엔드 기본 구조 설계

를 학습했습니다.

👨‍💻 제작자

이기준
