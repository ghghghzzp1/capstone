# capstone# Sasang Constitution Backend

사상체질 기반 맞춤형 건강 관리 플랫폼 (백엔드)

---

## 1. 프로젝트 개요
- Node.js (Express) 기반 API 서버
- MySQL 데이터베이스 사용
- 주요 기능: 회원가입 / 로그인 / 설문 응답 저장 등

---

## 2. 초기 세팅

### 2-1. 필수 설치
- Node.js (v20 이상)
- MySQL (8.x 이상)
- VS Code (권장)
- Postman (API 테스트용)

---

### 2-2. 데이터베이스 초기화
1. MySQL Workbench 실행
2. `scripts/init.sql` 열기
3. 번개 버튼 ⚡ 클릭 → DB(`sasang`), 계정(`sasang`/`pass1234`), 테이블(`users`, `survey_answers`) 생성됨

---

### 2-3. 환경변수 설정
- `.env.example`를 복사해서 `.env` 파일 생성
```env
PORT=3000
JWT_SECRET=dev-secret-change-this
DB_HOST=127.0.0.1
DB_PORT=3306
DB_USER=sasang
DB_PASS=pass1234
DB_NAME=sasang
