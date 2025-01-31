# 🔐 Spring Security 기반 로그인 시스템

## 📖 프로젝트 소개
Spring Boot를 기반으로 한 인증 및 권한 관리 시스템입니다. JWT, OAuth2, Redis 등을 활용하여 안전하고 효율적인 인증 시스템을 구현하였습니다.

---

## 🚀 주요 기능
- **회원가입 및 로그인**: 사용자 계정 생성 및 인증.
- **JWT 기반 인증**: 토큰 발급 및 검증.
- **OAuth2 로그인**: Google, Naver, Kakao 소셜 로그인 지원.
- **Redis**: 인증 토큰 캐싱을 통한 성능 향상.
- **Spring Security**: 역할 기반 권한 관리.

---

## 🛠 기술 스택
- **백엔드**: Spring Boot, Spring Security, Spring Data JPA
- **데이터베이스**: MySQL
- **인증**: JWT, OAuth2
- **캐싱**: Redis
- **빌드 도구**: Maven

---

### 1️⃣ 인증 (Authentication)
| 메서드 | 엔드포인트 | 설명 |
|--------|------------|------|
| `POST` | `/api/auth/signup` | 회원가입 |
| `POST` | `/api/auth/login` | 로그인 |
| `POST` | `/api/auth/logout` | 로그아웃 |

**📌 요청 예시 (회원가입)**
```json
{
  "username": "user1",
  "password": "pass1234"
}
```

**📌 응답 예시**
```json
{
  "message": "회원가입 성공"
}
```
