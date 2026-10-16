<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:667EEA,100:764BA2&height=190&section=header&text=Wonjin%20Kim&fontSize=56&fontColor=ffffff&fontAlignY=34&desc=%EC%93%B0%EB%8B%A4%EA%B0%80%20%EB%B6%88%ED%8E%B8%ED%95%9C%20%EA%B1%B8%20%EB%A7%8C%EB%93%A4%EC%96%B4%EC%84%9C%20%EC%97%86%EC%95%B1%EB%8B%88%EB%8B%A4&descSize=17&descAlignY=56" alt="" />

# 김원진 · Wonjin Kim

**생활 속 불편을 웹 서비스와 브라우저 도구로 해결합니다.**

React·TypeScript를 중심으로 웹 서비스를 만들고, AI·뇌파·로봇 등 다른 시스템과 연결하는 작업에도 참여했습니다. 만든 과정에서 부딪힌 문제와 해결 방법은 블로그에 기록합니다.

[블로그](https://lingard09.github.io) · [이메일](mailto:kinnwonjin@gmail.com) · [프로젝트 전체 목록](https://lingard09.github.io/project/)

## 대표 팀 프로젝트

### 1. 모보까 · 공연 예매 플랫폼

공연 동아리와 관람객을 연결해 예매와 운영자 관리를 제공하는 서비스입니다.

- **담당:** 로그인·인증, 마이페이지·개인정보 수정, 관리자용 공연·행사·모집·예매자 관리 화면.
- **구현:** Google 로그인과 백엔드를 연결하고, 예매 후 송금 안내·모바일 송금 앱 연결·카카오톡 공유를 구현했습니다.
- **문제 해결:** 공유 SDK의 로딩·오류 상태에 따라 버튼을 제어하고, 공유 내용에 공연별 계좌·예금주·금액을 연결했습니다.

**최우수상** · 2025 한동대 SW 페스티벌 SW 전공부문
`React` `Recoil` `Zustand`

[코드](https://github.com/MOBOGGA/MOBOGGA_Front) · [서비스](https://mobogga.netlify.app/) · [관리자·마이페이지 구현](https://github.com/MOBOGGA/MOBOGGA_Front/commit/cd1d13a3e6) · [송금·공유 개선](https://github.com/MOBOGGA/MOBOGGA_Front/commit/abc6b7dd60)

### 2. 여러시 · 위시리스트형 나눔 매칭

기관이 등록한 필요 물품과 개인의 나눔을 사진 인식·품목 매칭으로 연결하는 서비스입니다.

- **담당:** 사진 인식 API 연동, 유통기한 판독·검증, AI 일반명과 문자열 규칙을 결합한 품목 매칭.
- **구현:** 사진 인식을 Gemini에서 OpenAI로 전환하고, 모델의 판독 결과와 서버의 나눔 가능 여부 판정을 분리했습니다.
- **문제 해결:** 날짜를 못 읽은 물품이 ‘기한 없음’으로 통과하던 문제를 판독·없음·미확인 상태로 나눠 처리하고, 미확인 상태에는 추가 입력을 요구했습니다.

`Next.js` `TypeScript` `OpenAI` `Firebase`

[코드](https://github.com/Estherdami-cmd/Sharing) · [서비스](https://sharing-khaki.vercel.app) · [날짜 판독 개선](https://github.com/Estherdami-cmd/Sharing/commit/12678ff6e7) · [품목 매칭 개선](https://github.com/Estherdami-cmd/Sharing/commit/3e8a32df49)

### 3. 잡어드림 · 혼획물 거래 서비스

영상에서 분류한 혼획물 정보를 어민과 기업·연구소의 거래로 연결하는 서비스입니다.

- **담당:** 인증·역할별 홈, 거래 상세·매칭·요청·게시물 수정·프로필 화면과 API 연동.
- **구현:** 어민·공장별 홈과 메뉴를 분리하고, 거래 과정의 확인·취소·오류 모달을 구현했습니다.
- **문제 해결:** 토큰 유무·만료 검사와 로그아웃 처리를 관련 화면에 연결해 인증 예외 상황을 처리했습니다.

**대상** · 구글 후원 AI커리어스쿨 LAUNCH 창업톤
`React` `TypeScript` `styled-components`

[코드](https://github.com/LikeLionHGU/Karina_Front) · [서비스](https://jabeodream.netlify.app/) · [역할별 화면·API 연동](https://github.com/LikeLionHGU/Karina_Front/commit/691438c5ec) · [토큰 만료 처리](https://github.com/LikeLionHGU/Karina_Front/pull/47)

### 4. Bisang · EEG 기반 명상 서비스

뇌파와 자세 정보를 바탕으로 명상 상태를 시각화하고 세션 리포트를 제공하는 서비스입니다.

- **담당:** MindWave 패킷 파서·Web Serial 연결, 실시간 차트, 자세·눈 감음 분석과 세션 리포트 연동.
- **구현:** 장비 연결·해제와 데모 모드를 구성하고, 분석 결과를 세션 상태와 리포트 화면에 연결했습니다.
- **문제 해결:** 고빈도 원시 뇌파 패킷으로 불필요하게 갱신되던 화면을 지표 패킷 중심으로 바꾸고, 차트는 집중·명상 지표 수신 시 갱신하도록 수정했습니다.

`React` `TypeScript` `Web Serial` `MediaPipe` `Zustand`

[코드](https://github.com/EEGMeditation-HCI02/Bisang) · [서비스](https://bi-sang.pages.dev/) · [장비 연결 구현](https://github.com/EEGMeditation-HCI02/Bisang/pull/40) · [차트 갱신 개선](https://github.com/EEGMeditation-HCI02/Bisang/commit/6ebecc9004)

### 5. 물어볼래 · 수질 데이터 분석

질문에서 분석 조건을 추출하고 수질 측정 데이터와 원본 근거를 조회하는 서비스입니다.

- **담당:** 타입 기반 API 클라이언트, 규칙 기반 질문 파서, 인증·세션 연동과 배포 프록시.
- **구현:** 서버에 실제로 존재하는 지점·항목을 기준으로 질문을 해석하고, 추출한 조건을 사용자가 확인·수정하도록 연결했습니다.
- **문제 해결:** 배포 환경에서 API 대신 HTML이 반환되던 문제를 프록시·라우팅 수정과 JSON 응답 검증으로 처리했습니다.

`Vue 3` `TypeScript` `Vercel` `Cloudflare Pages`

[코드](https://github.com/LikeLionHGU/Aewonhaeseo-Front) · [서비스](https://aewonhaeseo-front.vercel.app) · [질문 파서 구현](https://github.com/LikeLionHGU/Aewonhaeseo-Front/commit/34e469bee6) · [배포 API 연동 수정](https://github.com/LikeLionHGU/Aewonhaeseo-Front/pull/7)

### 6. 팜사인 · 사과 출하 의사결정 지원

저장고 센서 데이터와 도매 시세 예측을 활용해 사과 출하 시점을 추천하는 서비스입니다.

- **담당:** 로그인·농가 정보 입력·시장가격 화면과 시세 예측 API 연동.
- **구현:** 시장·품종별 실제 시세와 7일 예측·예측 범위를 실선·점선·음영으로 구분한 차트를 구현했습니다.
- **문제 해결:** 로그인 전 선택에 의존하던 이동 경로를 인증 응답의 신규 회원 여부로 판단하도록 바꿔, 농가 정보 입력과 저장고 현황으로 분기했습니다.

**대상** · 경북 X AI 문제해결 해커톤
`React` `TypeScript` `SVG`

[코드](https://github.com/LikeLionHGU/HipApple_Front) · [서비스](https://hip-apple.vercel.app) · [로그인 후 분기 수정](https://github.com/LikeLionHGU/HipApple_Front/pull/34) · [시세 예측·차트 구현](https://github.com/LikeLionHGU/HipApple_Front/commit/b9b4ddba1d)

## 수상 · 경력

| 수상·선정 | 대회·사업 | 관련 프로젝트 |
| --- | --- | --- |
| 대상 | 구글 후원 AI커리어스쿨 LAUNCH 창업톤 | 잡어드림 |
| 대상 | 경북 X AI 문제해결 해커톤 · 한동대 산학협력단 | 팜사인 |
| 최우수상 | 2025 한동대 SW 페스티벌 · SW 전공부문 | 모보까 |
| 장려상 | 업스테이지 주관 AI Agent 해커톤 | — |
| 선정 | 2026 이노테크 지원사업 | 경제의 숲 |

- **ZCELL 인턴** — 한동대 교수 창업기업 · 풀스택 개발, 호스팅, DNS.
- **멋쟁이사자처럼대학 한동대학교 14기 대표** — 프론트엔드 13기 수료.
- **포항YMCA 지원 학습지원 플랫폼** — 학업위기청소년을 위한 시제품 제작.
- **경제퀴즈플랫폼** — 기획·PM·디자인·퍼블리싱.
- **군 복무** — 28사단 정보통신대대 영상음향장비운용병 만기 전역.

## 연구

### 뇌파 데이터와 비전 AI를 이용한 로봇팔 제어

P300 기반 BCI로 선택한 객체를 YOLO·Depth 카메라의 3차원 좌표와 연결해 로봇팔의 Pick & Place 동작으로 이어가는 시스템입니다.

**담당 — Unity 통합 제어 및 MyCobot 320 연동**

- EEG 모듈의 객체 선택 결과와 비전 모듈의 좌표를 Unity에서 통합했습니다.
- 소켓 통신으로 로봇팔에 좌표를 전달하고 Pick & Place 경로를 생성·실행했습니다.
- P300 시각 자극 인터페이스와 객체별 target 분류 횟수에 따른 최종 대상 판정을 구현했습니다.

| 측정 항목 | 기록된 결과 |
| --- | --- |
| EEG 명령 → Unity 응답 | 평균 8.796 ms |
| 카메라–로봇 좌표 보정 | 대응점 10개 기반 최소자승 아핀 변환 · 평균 오차 9.4 mm |
| P300 분류 | Trial Accuracy 0.917 · AUC 0.747 |

위 수치는 각 측정 구간의 결과이며, 로봇팔의 전체 작업 완료 시간을 의미하지 않습니다.

**2026 한국컴퓨터종합학술대회(KCC) 논문집 공저자** · 과기정통부 SW중심대학사업·한국연구재단 지원

`Unity` `C#` `OpenViBE` `YOLO` `RealSense Depth` `MyCobot 320`

[시연 영상](https://youtu.be/mIUh6lxgHxk)

## 개인 도구 · 기술 글

**[히즈넷 첨부파일 이름 복구](https://github.com/lingard09/HisnetKoreanFileNameFixer)** · `JavaScript` · `Browser Extension`

학교 첨부파일의 깨진 한글 이름을 다운로드 시점에 복구하는 확장입니다. Chromium 계열과 Firefox를 지원합니다. [만든 과정](https://lingard09.github.io/hisnet-filename-fixer/)

**[히즈넷 모바일](https://github.com/lingard09/hisnet-mobile)** · `React`
데스크톱 화면이 축소되어 보이던 학교 공지 목록을 모바일에서 읽기 좋게 바꾸는 북마클릿입니다. [만든 과정](https://lingard09.github.io/hisnet-mobile/)

**[PL2 웹사이트](https://github.com/lingard09/pl2-website)** · `HTML` `CSS` `JavaScript`
빌드 도구 없이 제작한 크리에이티브 스튜디오 정적 웹사이트입니다. [서비스](https://lingard09.github.io/pl2-website/)

**[로지스틱 성장 시각화](https://github.com/lingard09/biomath-logistic-2d)** · `HTML`
로지스틱 성장·수확 모델과 분기를 탐색하는 도구로, 의존성 없는 단일 HTML 파일로 동작합니다. [서비스](https://lingard09.github.io/biomath-logistic-2d/)

| 기술 글 | 다룬 문제 |
| --- | --- |
| [좌충우돌 대용량 영상 배포기](https://lingard09.github.io/video-hosting-detour/) | 134MB 영상 파일의 배포 방법 검토 |
| [히즈넷 모바일 버전 만들기](https://lingard09.github.io/hisnet-mobile/) | 모바일 화면이 없는 학교 시스템 개선 |
| [Floorp 주소창 붙여넣기 문제](https://lingard09.github.io/floorp-double-paste/) | 붙여넣기가 두 번 실행되는 브라우저 문제 조사 |

## 기술

- **주로 사용하는 기술:** JavaScript, TypeScript, React.
- **프로젝트에서 사용한 기술:** Next.js, Vue, Unity, C#, OpenAI, Gemini, Firebase, Cloudflare, Vercel.

<details>
<summary>그 밖에 사용한 언어 · 도구</summary>

기존 프로젝트·학습에서 사용한 기술입니다.

- **언어:** Java, Python, Swift.
- **웹·데이터:** Vite, Electron, Spring Boot, FastAPI, Node.js, PostgreSQL, Supabase.
- **배포·운영:** AWS, Docker, GitHub Actions.
- **AI·자동화:** Claude, OpenAI, Ollama, n8n.
- **연구·디자인:** EEG(DSI-24), MATLAB, SWLDA, ROS2, Figma.

</details>

## 더 만든 것

<details>
<summary>팀 프로젝트 · 기획 프로젝트 더 보기</summary>

| 프로젝트 | 내용 | 기술 · 역할 | 링크 |
| --- | --- | --- | --- |
| 터움 | TourAPI 기반 전통 문화 여행 탐색·AI 맞춤 코스 | Firestore 기반 여정 보관함, TourAPI 프록시·엣지 캐시, AI 추천 설명의 장소 불일치 필터링 | [추천 설명 검증](https://github.com/lingard09/teoum/commit/3e32da1ffc) · [코드](https://github.com/lingard09/teoum) · [서비스](https://teoum.pages.dev) |
| 경제의 숲 | 레벨 테스트·일일 퀴즈·대결·그룹 랭킹을 제공하는 경제 학습 플랫폼 | 기획·PM·디자인·프론트엔드, 정적 다중 페이지 전환, 공용 퀴즈 데이터와 대결 흐름 구현 | [퀴즈·대결 구현](https://github.com/lingard09/ForestOfEconomy-Front/commit/65feabe3d3) · [코드](https://github.com/lingard09/ForestOfEconomy-Front) · [서비스](https://lingard09.github.io/ForestOfEconomy-Front/index.html) |

**[한카 · Hancar](https://github.com/lingard09/HanCar)** — 대학생 카풀 iOS 앱에서 Google·Firebase 인증, 카풀 생성·수정·신청, 내 카풀 목록과 프로필, Firestore·MessageKit 기반 채팅을 구현했습니다. [구현 기록](https://github.com/lingard09/HanCar/commit/ddae792750)

**[BrainRacing](https://github.com/lingard09/BrainRacing)** — 뇌파 입력을 활용하는 Unity 레이싱 게임에 참여했습니다. 맵·씬 구성, 콜라이더·물리 설정, 부스터 작업 기록이 있습니다. [작업 기록](https://github.com/lingard09/BrainRacing/commits?author=lingard09)

[프로젝트 전체 목록](https://lingard09.github.io/project/)

</details>
