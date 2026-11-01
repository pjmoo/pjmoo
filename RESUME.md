# 박정민 (pjmoo) | Backend Developer 이력서

> **"사용자 경험과 서비스 운영 안정성을 함께 고민하는 백엔드 개발자입니다."**  
> Spring Boot 기반의 비즈니스 로직 및 인증·보안 아키텍처를 설계하고, 데이터 정합성과 배포 자동화를 검증하며 지속 가능한 서비스를 만듭니다.

---

## 📌 Contact & Channels

- **Email**: [jung17min66@gmail.com](mailto:jung17min66@gmail.com)
- **GitHub**: [github.com/pjmoo](https://github.com/pjmoo)
- **Tech Blog**: [myinfo30840.tistory.com](https://myinfo30840.tistory.com/)
- **Today I Learned (TIL)**: [github.com/pjmoo/PJMOO_TIL](https://github.com/pjmoo/PJMOO_TIL)

---

## 👨‍💻 About Me

- **검증 중심의 백엔드 개발**: 비즈니스 로직의 예외 상황과 데이터 정합성을 JUnit 5·Mockito 테스트 및 Flyway 마이그레이션으로 검증하며 개발합니다.
- **인증 및 보안 아키텍처 구현**: JWT, 쿠키 기반 세션, OAuth2 소셜 로그인, Redis 기반 토큰 블랙리스트 및 무차별 대입 방어(Rate Limit) 등 안전한 서비스 환경을 구축했습니다.
- **배포 및 운영 자동화**: Docker, Docker Compose, GitHub Actions, Nginx Blue/Green 무중단 배포 파이프라인을 직접 구축하고 장애 모니터링 체계를 경험했습니다.
- **문서화와 적극적인 협업**: PR 템플릿, 코드 가이드, 트러블슈팅 문서를 작성하며 팀원 간 브랜치 병합 충돌을 최소화하고 일관된 코드 품질을 유지합니다.

---

## 🛠 Tech Stack

| 분류 | 기술 및 도구 |
| :--- | :--- |
| **Language** | Java 17, JavaScript (ES6+), SQL, HTML5/CSS3 |
| **Backend** | Spring Boot 3/4, Spring Data JPA, Spring Security, Spring Web MVC, Spring AI, OAuth2, JWT, QueryDSL, MyBatis |
| **Database** | PostgreSQL, Redis, Flyway, Supabase |
| **Infra & DevOps** | Docker, Docker Compose, GitHub Actions, GHCR, Nginx (Blue/Green), AWS EC2, Render |
| **Testing & Tools**| JUnit 5, Mockito, Gradle, Git, GitHub, Postman, IntelliJ IDEA, Slack, Notion |

---

## 🎓 Education & Training

### 프로그래머스 데브코스 백엔드 엔지니어링 과정 (AIBE 7기)
**2026.05.13 ~ 2026.11.09** (약 6개월)

- **Java & Spring Boot 핵심 역량 습득**: 객체 지향 원칙(SOLID), Spring Data JPA 영속성 컨텍스트 관리 및 N+1 최적화, Spring Security 기반 인증/인가 체계 학습
- **데이터베이스 모델링 및 트랜잭션 관리**: 정규화, 인덱싱 전략, Flyway를 활용한 점진적 DB 형상 관리 및 데이터 무결성 보장
- **CI/CD 및 인프라 자동화 실습**: Docker 컨테이너화, GitHub Actions 기반 테스트/빌드 자동화, Nginx Blue/Green 무중단 배포 구현
- **실전 팀 프로젝트 3회 수행**: 애자일 스크럼, Git-flow 브랜치 전략, 코드 리뷰 및 협업 충돌 해결을 통한 실무 프로세스 완수

---

## 🚀 Projects

### 1. PastPort (패스트포트) | 전자제품 관리 및 신뢰 기반 중고거래 서비스
> **노트북 구매·관리 이력(여권)과 신뢰 기반 중고거래를 연결하는 플랫폼 (MVP: 노트북)**

- **진행 기간**: 2026.09 ~ 2026.11 (팀 최종 프로젝트, 백엔드 6인)
- **주요 역할**: 인증·보안 아키텍처 구축 및 노트북 MVP 프론트엔드 UI/UX 통합
- **기술 스택**: `Java 17`, `Spring Boot`, `Spring Security`, `JWT`, `PostgreSQL`, `Redis`, `Flyway`, `Docker Compose`, `Vanilla JS`, `CSS3`
- **저장소**: [GitHub (pjmoo/AIBE7_FinalProject_Team1)](https://github.com/pjmoo/AIBE7_FinalProject_Team1)

#### 💡 주요 담당 업무 및 기여
- **보안 및 인증 아키텍처 설계**:
  - `HttpOnly` 쿠키 기반 JWT 인증 체계와 CSRF 방어 구축
  - Redis를 활용한 Refresh Token 관리 및 로그아웃 시 Access Token 블랙리스트 처리
  - 무차별 대입 공격(Brute-force) 방지를 위한 로그인 Rate Limit 적용
- **이메일 인증 및 사용자 라이프사이클 관리**:
  - Supabase Auth 기반 이메일 인증 코드 발송, 재전송 쿨다운 및 미인증 회원 정리 스케줄러 개발
  - `VerificationStatus` 도입으로 인증 조회 실패 시 정상 사용자가 삭제되지 않도록 방어 로직 구현
- **채팅 및 중고거래 UX 강화**:
  - WebSocket 채팅방 나가기 기능 및 사용자 확인 모달 UX 구현
  - 제품 상세 증빙 문서 바로가기 버튼 및 여권 페이지 라우팅 보완
- **MVP 프론트엔드 UI 통합 및 브랜치 병합 조율**:
  - MVP 정책에 맞춰 노트북 외 카테고리(`is-soon`) 비활성화 및 상단 GNB(홈 / 제품 여권 / 중고거래 / 내 거래) 개편
  - 팀원 간 PR 병합 시 발생하는 UI 충돌 및 SecurityConfig 허용 경로 충돌 해결

---

### 2. BaroHae (바로해) | 긴급 업무 매칭 플랫폼
> **실시간 가용성과 신뢰도를 기반으로 24시간 이내 디지털 업무를 프리랜서와 매칭하는 플랫폼**

- **진행 기간**: 2026.08 ~ 2026.09 (팀 2차 프로젝트)
- **주요 역할**: 지원자 비교 및 작업자 매칭, 업무 취소/정산 트랜잭션, OAuth2 소셜 로그인, Render 클라우드 배포
- **기술 스택**: `Java 17`, `Spring Boot`, `Spring Data JPA`, `Spring Security`, `OAuth2`, `PostgreSQL (Supabase)`, `Flyway`, `WebSocket (STOMP)`, `Docker`, `Render`
- **저장소**: [GitHub (pjmoo/2nd_project)](https://github.com/pjmoo/2nd_project)

#### 💡 주요 담당 업무 및 기여
- **지원자 비교 및 작업자 선택 시스템**:
  - 의뢰인 전용 지원자 비교 대시보드 구축 (지원자 기술 스택, 평점, 작업 내역 비교)
  - 등록자 전용 접근 제어 및 작업자 매칭 시 중복 지원 방지 로직 구현
- **업무 상태 전이 및 재화(품) 정산 로직**:
  - 업무 등록 시 재화 예약, 업무 취소/만료 시 예약 재화 자동 반환, 작업 완료 승인 시 정산 트랜잭션 구축
  - 품 거래 원장 보존 및 프로필 내 입출금 이력 추적 기능 구현
- **소셜 로그인 및 보안 연동**:
  - Kakao 및 Google OAuth2 소셜 로그인 연동, 계정 매핑 및 구글 계정 선택 옵션 활성화
- **실시간 채팅 및 첨부 파일 보안**:
  - WebSocket STOMP 메시지 접근 권한 검증
  - 비공개 첨부 파일에 대해 5분 유효 서명 URL 발급 체계 적용
- **클라우드 배포 및 안정화**:
  - Render 환경 배포를 위한 Dockerfile 작성 및 빌드 파이프라인 구성
  - 전역 예외 처리 핸들러 및 복합 조건 검색 목록 쿼리 성능 개선

---

### 3. MOTIPE (모티페) | 지역 축제 기반 AI 여행 추천 플랫폼
> **사용자 성향 진단을 바탕으로 지역 축제와 연계된 여행 일정을 추천하는 커뮤니티 플랫폼**

- **진행 기간**: 2026.05.28 ~ 2026.06.12 (팀 1차 프로젝트)
- **주요 역할**: 커뮤니티·지도 기반 UI 및 사용자 인터랙션 구현, Supabase 데이터 연동
- **기술 스택**: `JavaScript`, `Node.js`, `Express.js`, `Supabase`, `HTML5`, `CSS3`
- **저장소**: [GitHub (pjmoo/AIBE7-Project1-Team01)](https://github.com/pjmoo/AIBE7-Project1-Team01)

#### 💡 주요 담당 업무 및 기여
- **성향 진단 및 맞춤 추천 UI**:
  - 질문지 기반 성향 진단 결과 도출 및 축제 추천 결과 카드 인터랙션 제작
- **지도 및 커뮤니티 화면 연동**:
  - 카카오 지도 API를 활용한 축제 위치 마커 표시 및 축제 연계 일정 뷰 구현
  - 반응형 게시글 카드 컴포넌트 개발 및 Supabase Auth 연동 회원 상태 유지 처리
- **UI 트러블슈팅 및 사용자 경험 개선**:
  - 화면 해상도에 따른 게시글 카드 높이 불균형 및 텍스트 말줄임 CSS 이슈 해결

---

### 4. Spring Boot CI/CD & Blue-Green 무중단 배포 파이프라인
> **GitHub Actions와 Docker Compose를 이용한 백엔드 자동화 및 Nginx 무중단 배포 구축**

- **진행 기간**: 2026.09 (개인 인프라 실습 프로젝트)
- **기술 스택**: `Java 17`, `Spring Boot`, `Docker`, `Docker Compose`, `Nginx`, `GitHub Actions`, `GHCR`, `AWS EC2`, `Slack Webhook`
- **저장소**: [CI 저장소](https://github.com/pjmoo/260917_spring-test-ci) · [CD 저장소](https://github.com/pjmoo/260918_ci-cd)

#### 💡 주요 담당 업무 및 기여
- **자동화 CI 파이프라인**:
  - GitHub Actions에서 Gradle 캐싱을 적용하여 빌드 시간을 단축하고 JUnit 5 단위 테스트 자동 검증
  - 테스트 통과 시 GHCR(GitHub Container Registry)로 도커 이미지 태깅 및 푸시 자동화
- **Nginx 기반 Blue/Green 무중단 배포**:
  - `deploy.sh` 쉘 스크립트를 작성하여 현재 가동 중인 컨테이너(Blue/Green) 확인 후 신규 컨테이너 배포
  - Health check 성공 확인 후 Nginx `service-url.inc` 포트를 교체하고 `nginx -s reload`로 무중단 전환
  - 이전 컨테이너 정리 및 실패 시 롤백 로직 구성
- **알림 자동화**:
  - 배포 성공/실패 여부를 Slack Incoming Webhook으로 즉각 전송하여 배포 가시성 확보

---

### 5. WorryDoll (걱정인형) | Spring AI & RAG 기반 AI 심리 상담 서비스
> **VectorStore 임베딩과 Spring AI를 접목한 개인 맞춤형 AI 상담 챗봇**

- **진행 기간**: 2026.07 ~ 2026.08 (개인 AI 백엔드 프로젝트)
- **기술 스택**: `Java 17`, `Spring Boot`, `Spring AI`, `Google Gemini API`, `RAG`, `Spring Data JPA`, `PostgreSQL`
- **저장소**: [GitHub (pjmoo/260731_worrydoll)](https://github.com/pjmoo/260731_worrydoll)

#### 💡 주요 담당 업무 및 기여
- **Spring AI 및 RAG 파이프라인 구성**:
  - 상담 지침 및 심리 케어 데이터를 임베딩하여 VectorStore에 적재
  - 사용자의 고민 입력 시 관련 문서를 검색(RAG)하여 환각(Hallucination)을 줄인 안정적인 위로·상담 답변 생성
- **대화 이력 및 세션 유지**:
  - `JpaChatMemory`를 설계하여 사용자별 대화 맥락을 데이터베이스에 영속화하고 문맥 기반 멀티턴 대화 지원

---

## 📝 Learning & Growth

- **Today I Learned (TIL)**: 매일 학습한 Spring 내부 동작 원리, SQL 최적화, HTTP 프로토콜, 배포 트러블슈팅 등을 [PJMOO_TIL](https://github.com/pjmoo/PJMOO_TIL)에 정리하고 있습니다.
- **기술 블로그 운영**: 학습한 내용을 정리하여 [Tistory 블로그](https://myinfo30840.tistory.com/)에 기록하며 지식을 체계화하고 있습니다.
