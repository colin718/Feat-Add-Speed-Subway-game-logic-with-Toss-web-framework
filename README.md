# Speed Subway (스피드 서브웨이)

### 프로젝트 소개
서울/수도권 지하철 노선도를 암기하고 순발력을 테스트하는 **반응형 웹 게임**입니다.
(금융 앱) **토스(Toss) 챌린지** 참여를 위해 개발되었으며, 별도의 라이브러리 없이 **Vanilla JavaScript**로 게임 로직을 구현하고 **Toss Web Framework**를 연동하여 실제 앱 환경과 유사한 경험을 제공합니다.

### 주요 기능 (Features)
* **두 가지 게임 모드:**
    * **타임어택:** 1분 제한 시간 동안 최대한 많은 역을 맞추는 모드
    * **목적지 도달:** 출발역에서 환승을 포함해 목적지까지 도달하는 길찾기 모드
* **인터랙티브 UI/UX:**
    * 실제 지하철 전광판을 모티브로 한 디자인
    * 지하철 진입/출발 애니메이션 (`CSS Keyframes`) 구현
    * 성공/실패 시 청각적 피드백 제공 (`Web Audio API`)
* **데이터 연동:**
    * `JSON` 기반의 수도권 지하철 데이터 파싱 및 구조화
    * `LocalStorage`를 활용한 기기별 최고 기록 저장

### 기술 스택
* **Core:** HTML5, CSS3, JavaScript (ES6+)
* **Framework:** Apps-in-Toss Web Framework (리더보드 및 앱 환경 연동)
* **Design:** Flexbox/Grid Layout, Responsive Web Design (Mobile First)

### 개발 포인트 (Highlights)
1.  **플랫폼 SDK 연동:** `@apps-in-toss/web-framework`를 활용하여 모바일 앱 내 안전 영역(Safe Area) 패딩 처리 및 리더보드 스코어 전송 로직 구현
2.  **알고리즘 구현:**
    * BFS/DFS 개념을 응용한 노선 연결 및 환승 유효성 검증 로직
    * 순환선(2호선)의 특수성을 고려한 인덱스 계산 처리
3.  **최적화:** 외부 이미지 리소스 로딩 전 로딩 오버레이 구현으로 사용자 경험(UX) 개선

### 실행 화면
<img width="974" height="829" alt="스크린샷 2025-12-17 14 21 41" src="https://github.com/user-attachments/assets/cb635e81-e0ec-4595-8039-c152c02662b5" />

<img width="976" height="820" alt="스크린샷 2025-12-17 14 21 54" src="https://github.com/user-attachments/assets/c74ecc63-d433-4966-8de0-16cb2ec2b322" />

