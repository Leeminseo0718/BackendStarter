# Node.js API Server
Node.js + Express + MongoDB(Mongoose) 기반의 REST API 서버입니다.
회원가입, 로그인 등 기본적인 사용자 인증 기능을 포함하며
데이터 처리 로직은 MVC 패턴에 기반해 모듈화하여 구성했습니다.

------------------------------------------------------------------
### 🚀 Tech Stack
- Node.js / Express
- MongoDB / Mongoose
- SQL 기반 초기 설계 파일(database.sql) 포함
- JavaScript (ES6)

### 📂 Project Structure
```
BackendStarter/
 ├── controller/     # 요청 처리 로직 (Controller)
 ├── data/           # 데이터 스키마 및 모델 관련 파일
 ├── db/             # MongoDB 연결 설정 (Mongoose)
 ├── middleware/     # 인증/검증 등 미들웨어
 ├── public/         # 정적 파일
 ├── router/         # 라우터 (API endpoint)
 ├── app.mjs         # Express 서버 초기 실행 파일
 ├── config.mjs      # 환경 설정 파일
 ├── database.sql    # 초기 SQL 설계안
 └── package.json

```

### ⚙️ Installation & Setup
```
# 1. Clone project
git clone https://github.com/Leeminseo0718/X.git

# 2. Move into folder
cd X

# 3. Install dependencies
npm install

# 4. Start development server
npm run dev
```

### 🔌 Environment Config
- `config.mjs` 또는 `.env` 파일을 통해 환경 설정을 할 수 있습니다.
예시:
```
MONGO_URI=mongodb+srv://your-db-url
PORT=3000
JWT_SECRET=yourSecret
```

### 🧩 주요 기능 (Features)
- 회원가입 / 로그인
  - MongoDB + Mongoose 기반 계정 생성
  - 비밀번호 해싱 처리
  - JWT 인증 흐름 적용

- RESTful Routing
  - router 폴더에서 API endpoint 분리
  - controller에서 비즈니스 로직 처리
    
- Middleware 기반 구조
  - 요청 검증, 인증 처리 분리
  - 유지보수성과 확장성 고려

- DB 구조 설계 파일 제공(database.sql)
  - 기존 SQL 기반 설계를 참고하여 MongoDB 구조로 전환한 흔적 포함


