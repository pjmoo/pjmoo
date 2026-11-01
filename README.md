<img width="1900" height="600" alt="Profile Banner" src="https://github.com/user-attachments/assets/35fc4898-04fc-432b-9660-f6db9cf5e053" />

<h1 align="center">Hi 👋, I'm 박정민 (pjmoo)</h1>
<h3 align="center">사용자 경험과 서비스 운영 안정성을 함께 고민하는 백엔드 개발자입니다.</h3>

<p align="center">
  <a href="./RESUME.md">
    <img src="https://img.shields.io/badge/📄%20상세%20이력서(Markdown)%20보기-0969DA?style=for-the-badge&logoColor=white" alt="Resume Badge" />
  </a>
  <a href="./pjmoo_이력서_초안.docx">
    <img src="https://img.shields.io/badge/📥%20이력서(Word%20.docx)%20다운로드-2B579A?style=for-the-badge&logo=microsoftword&logoColor=white" alt="Word Badge" />
  </a>
</p>

---

## 👨‍💻 About Me

- ☕ **Java / Spring Boot** 기반 백엔드 아키텍처와 비즈니스 로직 설계를 깊이 있게 다룹니다.
- 🎓 **프로그래머스 데브코스 백엔드 엔지니어링 과정 (AIBE 7기)** 수료 (`2026.05.13 ~ 2026.11.09`)
- 🔒 인증·보안(JWT, Cookie, Redis Token Blacklist, OAuth2, Rate Limit)과 데이터 정합성을 중요하게 생각합니다.
- 🚀 **Docker, GitHub Actions, Nginx Blue/Green 무중단 배포** 등 인프라 및 CI/CD 자동화 경험을 보유하고 있습니다.
- 🤖 **Spring AI와 RAG**를 접목한 실무형 AI 백엔드 서비스 개발 역량을 키우고 있습니다.
- 📚 매일 배운 기술과 트러블슈팅 경험은 [PJMOO_TIL](https://github.com/pjmoo/PJMOO_TIL)과 [기술 블로그](https://myinfo30840.tistory.com/)에 꾸준히 기록하고 있습니다.

---

## 🛠 Tech Stack

### Languages
<p>
  <img src="https://skillicons.dev/icons?i=java,js,html,css" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
</p>

### Backend
<p>
  <img src="https://skillicons.dev/icons?i=spring,nodejs,express" />
  <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white" />
  <img src="https://img.shields.io/badge/JPA-59666C?style=for-the-badge" />
  <img src="https://img.shields.io/badge/QueryDSL-0769AD?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Flyway-CC0200?style=for-the-badge&logo=flyway&logoColor=white" />
</p>

### Database & Cache
<p>
  <img src="https://skillicons.dev/icons?i=postgres,redis" />
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white" />
</p>

### DevOps & Infra
<p>
  <img src="https://skillicons.dev/icons?i=docker,githubactions,nginx,aws" />
</p>

### AI
<p>
  <img src="https://img.shields.io/badge/Spring%20AI-6DB33F?style=for-the-badge&logo=spring&logoColor=white" />
  <img src="https://img.shields.io/badge/Google%20GenAI-4285F4?style=for-the-badge&logo=google&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenAI%20API-412991?style=for-the-badge&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/RAG-111111?style=for-the-badge" />
</p>

### Tools
<p>
  <img src="https://skillicons.dev/icons?i=git,github,gradle,idea" />
</p>

---

# 🚀 Featured Projects

## 💻 PastPort (패스트포트)
### 3rd Team Project (Final) · 2026.09 ~ 2026.11

**전자제품 관리 및 신뢰 기반 중고거래 서비스 (MVP: 노트북)**

노트북의 영수증, 보증서, 수리 이력 등 제품 여권을 디지털로 관리하고, 신뢰할 수 있는 이력을 바탕으로 안전하게 거래하는 플랫폼입니다.

- **주요 역할**: 인증·보안 아키텍처 구축 및 노트북 MVP 프론트엔드 UI/UX 통합
- **핵심 기여**:
  - `HttpOnly` 쿠키 기반 JWT 인증, Redis 토큰 블랙리스트 & Refresh Token 관리, CSRF 방어
  - 무차별 대입 공격(Brute-force) 방어를 위한 로그인 Rate Limit 적용
  - Supabase Auth 연동 이메일 인증 발송/재전송 및 미인증 계정 자동 정리 스케줄러 구현
  - 채팅방 나가기/퇴장 처리 및 사용자 확인 모달 UX 구현
  - MVP 정책에 맞춘 카테고리 비활성화 및 상단 네비게이션 개편, 팀원 간 브랜치 병합 충돌 조율
- **Tech Stack**: `Java 17`, `Spring Boot`, `Spring Security`, `PostgreSQL`, `Redis`, `Flyway`, `Docker Compose`, `Vanilla JS`

[🔗 Repository](https://github.com/pjmoo/AIBE7_FinalProject_Team1)

---

## ⚡ BaroHae (바로해)
### 2nd Team Project · 2026.08 ~ 2026.09

**실시간 가용성 및 신뢰도 기반 긴급 업무 매칭 플랫폼**

24시간 이내 처리가 필요한 디지털 업무(개발 오류 수정, 문서/디자인 보완 등)를 프리랜서와 신속하게 매칭하는 플랫폼입니다.

- **주요 역할**: 지원자 비교 및 작업자 매칭, 업무 취소/정산 트랜잭션, OAuth2 소셜 로그인, Render 클라우드 배포
- **핵심 기여**:
  - 의뢰인 전용 지원자 비교 대시보드(프로필/평점/기술 비교) 및 작업자 매칭/중복 지원 방어
  - 업무 상태 전이(등록·매칭·완료·취소)에 따른 재화(품) 예약·반환·정산 트랜잭션 구현
  - Kakao & Google OAuth2 소셜 로그인 연동 및 계정 매핑
  - STOMP WebSocket 채팅 권한 검증 및 비공개 첨부 파일 서명 URL(5분 유효) 발급
  - Render 배포용 Dockerfile 작성 및 전역 오류 핸들링/목록 쿼리 성능 개선
- **Tech Stack**: `Java 17`, `Spring Boot`, `Spring Data JPA`, `Spring Security`, `OAuth2`, `PostgreSQL (Supabase)`, `Flyway`, `WebSocket (STOMP)`, `Docker`, `Render`

[🔗 Repository](https://github.com/pjmoo/2nd_project)

---

## ✈️ MOTIPE (모티페)
### 1st Team Project · 2026.06

**지역 축제 기반 AI 맞춤 여행 추천 플랫폼**

사용자의 여행 성향을 분석하여 최적의 지역 축제와 연계 여행 일정을 추천하는 커뮤니티 서비스입니다.

- **주요 역할**: 커뮤니티·지도 UI 인터랙션 구현 및 Supabase 연동
- **핵심 기여**:
  - 여행 성향 진단 인터페이스 및 축제 추천 결과 카드 컴포넌트 개발
  - 카카오 지도 API 연동 및 축제 위치 마커/연계 일정 표시
  - Supabase 기반 회원 인증, 게시글 CRUD 및 마이페이지 연동
- **Tech Stack**: `HTML5`, `CSS3`, `JavaScript`, `Node.js`, `Express.js`, `Supabase`

[🔗 Repository](https://github.com/pjmoo/AIBE7-Project1-Team01)

---

## 🚀 Spring Boot CI/CD & Blue-Green 무중단 배포
### Personal Infra / DevOps Project · 2026.09

**GitHub Actions와 Docker Compose를 활용한 무중단 배포 파이프라인 구축**

- GitHub Actions 기반 빌드 및 JUnit 5 단위 테스트 자동화, GHCR 이미지 빌드 및 푸시
- Docker Compose & Nginx를 활용한 Blue/Green 무중단 배포(Zero-downtime) 스크립트 작성
- 배포 성공/실패 시 Slack Incoming Webhook 실시간 알림 연동
- **Tech Stack**: `Java 17`, `Spring Boot`, `Docker`, `Docker Compose`, `Nginx`, `GitHub Actions`, `GHCR`, `AWS EC2`, `Slack Webhook`

[🔗 CI Repository](https://github.com/pjmoo/260917_spring-test-ci) · [🔗 CD Repository](https://github.com/pjmoo/260918_ci-cd)

---

## 🧠 Spring AI & RAG Study (WorryDoll)
### Personal AI Backend Project · 2026.07 ~ 2026.08

**Spring AI와 VectorStore 임베딩 기반 AI 상담 챗봇 서비스**

- Google Gemini API 및 Spring AI 프레임워크 연동
- VectorStore 기반 RAG(검색 증강 생성)를 구축하여 맞춤형 상담 답변 제공
- `JpaChatMemory`를 구현하여 다중 사용자 세션 및 대화 문맥 보존
- **Tech Stack**: `Java 17`, `Spring Boot`, `Spring AI`, `Google Gemini API`, `RAG`, `Spring Data JPA`, `PostgreSQL`

[🔗 WorryDoll Repository](https://github.com/pjmoo/260731_worrydoll) · [🔗 Spring AI 실습](https://github.com/pjmoo/260728_springai) · [🔗 RAG 실습](https://github.com/pjmoo/260730_rag)

---

## 📚 Today I Learned

매일 학습한 기술 내용, 트러블슈팅, 이론 정리를 꾸준히 기록하고 있습니다.

[📖 PJMOO_TIL 보러가기](https://github.com/pjmoo/PJMOO_TIL)

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-stats-extended.vercel.app/api?username=pjmoo&show_icons=true&hide_border=true&theme=github_dark" height="165" />
  <img src="https://github-stats-extended.vercel.app/api/top-langs/?username=pjmoo&layout=compact&hide_border=true&theme=github_dark" height="165" />
</p>

---

## 📝 Blog & Contact

- **Blog**: [![Tistory](https://img.shields.io/badge/Tistory-FF5A4A?style=for-the-badge&logo=tistory&logoColor=white)](https://myinfo30840.tistory.com/)
- **Email**: [jung17min66@gmail.com](mailto:jung17min66@gmail.com)

---

## 🎮 Interests

🎮 게임 · 🎬 영화 · 📚 독서 · 🍿 애니메이션  
**PS. 프래그마타 재밌어요 😎**
