# gguatit

![Followers](https://img.shields.io/github/followers/gguatit?style=social)
![Visitors](https://komarev.com/ghpvc/?username=gguatit&color=blue)

---

## About Me
- Web Security / API Security / Backend Development
- OpenAPI 기반 API 설계 및 보안 중심 개발
- 취약점 분석 및 공격 시나리오 설계 및 검증
- 공격 재현 가능한 PoC 기반 테스트 수행

---

## Tech Stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

### Backend
- Node.js (Express)
- TypeScript
- OpenAPI 3.x (Swagger)
- RESTful API 설계 및 명세 기반 개발

### Frontend
- React

### Security / Analysis
- Kali Linux (NetHunter)
- Burp Suite (Proxy / Repeater / Intruder 기반 테스트)
- Wireshark (패킷 분석 및 프로토콜 레벨 검증)

### Infra
- Docker
- Git
- Cloudflare (Proxy / DNS / 기본 보안 설정)

---

## Activity

<p align="center">
  <img src="https://streak-stats.demolab.com?user=gguatit&theme=radical" width="48%" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=gguatit&theme=radical" width="48%" />
</p>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=gguatit&theme=radical" width="96%" />
</p>

---

## Security Research

### Web Application
- XSS (Reflected / Stored) 공격 및 필터 우회 테스트
- SQL Injection (Error-based / Boolean-based) 검증
- 인증 우회 및 세션 처리 로직 분석

### API Security
- OpenAPI 기반 API 공격 벡터 분석
- 입력값 검증 우회 테스트 (JSON / Query / Header)
- 인증 토큰(JWT) 구조 분석 및 변조 테스트

### Network
- 패킷 캡처 및 트래픽 분석
- HTTP/HTTPS 요청 흐름 및 세션 식별 구조 분석

---

## Threat Model

- 공격자: 인증되지 않은 외부 사용자
- 목표: 인증 우회 및 데이터 접근
- 주요 공격 벡터:
  - XSS 기반 세션 탈취
  - Injection 기반 DB 접근
  - API 요청 변조 및 권한 상승

---

## Projects

### Anonymous Chat
https://github.com/gguatit/Anonymous_Chat

- 실시간 익명 채팅 서비스
- 사용자 식별 최소화 구조 설계
- 입력값 검증 로직 적용 및 XSS 방어 처리
- 클라이언트 렌더링 과정에서의 스크립트 실행 방지 구조 적용

#### Security Considerations
- 입력값 필터링 및 출력 인코딩 적용
- 기본적인 Injection 방어 로직 구성
- 메시지 처리 과정에서의 공격 벡터 검증 수행

---

### kalpha-s_api
https://github.com/gguatit/kalpha-s_api

- TypeScript 기반 API 서버
- OpenAPI 3.x 명세 기반 구조 설계
- RESTful API 및 자동 문서화
- 요청 검증 및 구조화된 응답 처리

#### Security Considerations
- 요청 스키마 검증 기반 입력 제한
- 인증/인가 구조 확장 고려 설계
- API 요청 변조 및 비정상 입력 테스트 수행

---

## Contact
- dev@kalpha.kr
