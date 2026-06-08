# 메르핸드 (Märchand) - 수어 학습 및 동화 생성 서비스

'메르핸드(Märchand)'는 청각장애 아동의 언어 학습을 돕기 위해 수어 콘텐츠와 생성형 AI 기술을 결합한 인터랙티브 교육 서비스입니다. 동화 속 이야기를 통해 재미있게 수어를 배우고, AI가 생성한 창의적인 콘텐츠를 경험할 수 있습니다.

* **개발 기간**: 2025.03 ~ 2025.10 (2025 한이음 ICT 멘토링 프로젝트)
* **주요 목적**: 청각장애 아동의 언어 학습 진입 장벽 완화 및 수어 교육 콘텐츠 제공

## Tech Stack

- **Backend**: Java, Spring Boot
- **Database**: MariaDB, MyBatis
- **AI/API**: OpenAI API (GPT-4, DALL-E 기반 동화/이미지 생성)
- **Deployment/Tools**: JSP, JavaScript (jQuery), AWS(배포 기반)

## Key Features

### 1. 수어 학습 콘텐츠 제공
- 수어 단어 데이터베이스를 기반으로 이미지와 함께 직관적인 수어 학습 서비스를 제공합니다.
- 단순 암기가 아닌 퀴즈를 통한 인터랙티브 학습을 지원합니다.

### 2. 생성형 AI 기반 동화 제작
- OpenAI API와 연동하여 사용자가 입력한 키워드에 따라 맞춤형 동화 텍스트와 삽화를 자동 생성합니다.
- 수어 학습 후 아이들이 자신만의 동화를 직접 만들어보는 창작 활동을 지원합니다.

### 3. 학습 관리 시스템
- 회원별 학습 진도율 관리 및 퀴즈 결과 분석을 통해 개인화된 학습 경험을 제공합니다.

---

## Project Structure

```text
src/
 ├── main/
 │    ├── java/kopo/poly/hanium/
 │    │    ├── controller/      # Fairytale, Quiz, Story 등 비즈니스 로직 제어
 │    │    ├── service/         # OpenAI API 연동 및 데이터 처리 서비스
 │    │    ├── mapper/          # MyBatis 매퍼 파일 및 DB 연동
 │    │    └── dto/             # 데이터 전송 객체
 │    └── resources/
 │         ├── mapper/          # MyBatis SQL 쿼리 XML
 │         └── static/          # 수어 학습용 이미지 및 프론트엔드 리소스
 └── webapp/WEB-INF/views/      # JSP 기반 사용자 UI
