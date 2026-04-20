# gguatit

<p align="center">
  <img src="https://img.shields.io/github/followers/gguatit?style=social" />
  <img src="https://komarev.com/ghpvc/?username=gguatit&color=blue" />
</p>

---

## Profile

Web Security / API Security / Backend Development 중심으로 활동  
OpenAPI 기반 API 설계 및 공격 시나리오 분석  
재현 가능한 PoC 기반 검증을 기준으로 보안 테스트 수행

---

## Core Focus

- Web Application Security (XSS, Injection, Auth Bypass)
- API Security (Schema Validation, Request Manipulation)
- Backend Architecture (OpenAPI, RESTful Design)

---

## Tech Stack

<table>
<tr>
<td width="20%"><b>Backend</b></td>
<td>
Node.js (Express)<br/>
TypeScript<br/>
OpenAPI 3.x (Swagger)<br/>
RESTful API Design
</td>
</tr>

<tr>
<td><b>Frontend</b></td>
<td>
React
</td>
</tr>

<tr>
<td><b>Security</b></td>
<td>
Kali Linux (NetHunter)<br/>
Burp Suite (Proxy / Repeater / Intruder)<br/>
Wireshark (Traffic Analysis)
</td>
</tr>

<tr>
<td><b>Infra</b></td>
<td>
Docker<br/>
Git<br/>
Cloudflare
</td>
</tr>
</table>

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

### Web Layer
- XSS (Reflected / Stored) 공격 및 필터 우회 검증
- SQL Injection (Error / Boolean 기반) 테스트
- 인증 우회 및 세션 처리 로직 분석

### API Layer
- OpenAPI 기반 API 구조 분석
- 입력값 검증 우회 (JSON / Query / Header)
- JWT 구조 분석 및 변조 테스트

### Network Layer
- 패킷 캡처 및 트래픽 분석
- HTTP/HTTPS 세션 흐름 분석

---

## Threat Model

<table>
<tr><td width="20%"><b>Attacker</b></td><td>Unauthenticated External User</td></tr>
<tr><td><b>Objective</b></td><td>Authentication Bypass / Data Access</td></tr>
<tr><td><b>Vectors</b></td><td>XSS / Injection / Request Manipulation</td></tr>
</table>

---

## Projects

### Anonymous Chat
https://github.com/gguatit/Anonymous_Chat

**Overview**
- Real-time Anonymous Chat Service
- Minimal User Identification Architecture

**Security**
- Input Validation / Output Encoding 적용
- XSS 및 Injection 방어 구조 설계
- 클라이언트 렌더링 기반 공격 벡터 검증

---

### kalpha-s_api
https://github.com/gguatit/kalpha-s_api

**Overview**
- TypeScript 기반 API 서버
- OpenAPI 3.x 명세 기반 구조 설계

**Security**
- 요청 스키마 검증 기반 입력 제한
- API Request 변조 테스트 수행
- 인증/인가 구조 확장 고려 설계

---

## Contact

dev@kalpha.kr
