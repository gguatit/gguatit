# gguatit

**kalpha** · Web & API Security / Backend

Web/API security and backend engineer. I design OpenAPI-based APIs, analyze attack scenarios, and validate them with reproducible PoCs.

<p align="center">
  <img src="https://img.shields.io/github/followers/gguatit?style=social" alt="GitHub followers" />
  <img src="https://hits.sh/github.com/gguatit.svg?label=Profile%20visitors&color=0e75b6" alt="Profile visitors" />
  <a href="https://hub.xerj.org/contributors/gguatit"><img src="https://hub.xerj.org/contributors/gguatit/badge.svg" alt="XERJ Corpus Hub contributor" /></a>
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
RESTful API Design<br/>
WebSocket
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
<td><b>Cloud</b></td>
<td>
Cloudflare Workers<br/>
Cloudflare D1<br/>
Cloudflare R2<br/>
Durable Objects
</td>
</tr>

<tr>
<td><b>Infra</b></td>
<td>
Docker<br/>
Git
</td>
</tr>
</table>

---

## Activity

<p align="center">
  <img src="https://streak-stats.demolab.com?user=gguatit&theme=tokyonight&hide_border=true" width="48%" alt="GitHub streak stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=gguatit&layout=compact&theme=tokyonight&hide_border=true" width="48%" alt="Top languages" />
</p>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=gguatit&theme=tokyonight" width="96%" alt="GitHub profile details" />
</p>

---

## Security Practice

직접 수행한 테스트와 관심 있는 연구 주제를 정리합니다.

### Web Layer
- XSS, SQL Injection 등 웹 취약점 재현 및 필터 우회 검증
- 인증 우회 및 세션 처리 로직 분석

### API Layer
- OpenAPI 명세 기반 API 구조 및 입력 검증 분석
- JWT 구조 분석 및 변조 테스트

### Network Layer
- 패킷 캡처 및 HTTP/HTTPS 트래픽 흐름 분석

---

## Projects

### Anonymous Chat
[github.com/gguatit/Anonymous_Chat](https://github.com/gguatit/Anonymous_Chat)

**Stack**: JavaScript · Cloudflare Workers · Durable Objects · D1

**Overview**
- Real-time anonymous chat service
- Minimal user identification architecture

**Security**
- Input validation / output encoding
- XSS and injection defense design
- Client-rendering attack vector validation

**Threat Model**

<table>
<tr><td width="20%"><b>Attacker</b></td><td>Unauthenticated External User</td></tr>
<tr><td><b>Objective</b></td><td>Authentication Bypass / Data Access</td></tr>
<tr><td><b>Vectors</b></td><td>XSS / Injection / Request Manipulation</td></tr>
</table>

**XERJ Corpus Hub**
- Selected commit: [`e57e898a51`](https://github.com/gguatit/Anonymous_Chat/commit/e57e898a51) — 공지사항을 D1에 영구 저장, Durable Object 저장 한도로 인한 공지 유실 수정
- [Contributor profile](https://hub.xerj.org/contributors/gguatit) · AGPL-3.0 corpus, currently in licence review (not yet installable)

---

### XMem
[Xeon-Security/XMem](https://github.com/Xeon-Security/XMem)

**Stack**: Rust · egui · Windows user-mode

**Overview**
- Windows 프로세스 메모리 공격·포렌식 연구 플랫폼
- 프로세스/메모리 맵/PE/모듈/스레드 분석, 스냅샷 diff, 미니덤프, `.xmemimg` 생성·분석

**Security**
- XMEM-001~005 증거 기반 탐지 및 위험도 점수
- 통제된 실험과 리포트 자동화

---

### file-server
[gguatit/file-server](https://github.com/gguatit/file-server) · [file.kalpha.kr](https://file.kalpha.kr)

**Stack**: TypeScript · Hono · Cloudflare Workers · R2

**Overview**
- Cloudflare Workers + R2 기반 파일 서버
- API 업로드/다운로드, 24시간 후 자동 삭제

**Security**
- API key / admin 인증 (12h JWT, PBKDF2-SHA256, HMAC-signed httpOnly cookie)
- IP rate limit (60/min), 업로드 크기 제한 (50MB / chunked 250MB)
- UUID v4 파일 ID, attachment + nosniff, CORS allowlist, 만료 검사

---

### OCS (OpenCode Sessions)
[gguatit/OCS-OpenCode-Sessions-](https://github.com/gguatit/OCS-OpenCode-Sessions-)

**Stack**: Tauri 2 · Rust · rusqlite · Vanilla JS

**Overview**
- opencode 세션 SQLite DB를 읽기 전용으로 탐색하는 데스크톱 앱
- 대화 뷰, todos, diffs, command palette, bookmarks, en/ko/zh/ja i18n

**Security**
- rusqlite query-only 모드로 DB에 read-only 접근
- `~/.local/share/opencode/opencode.db`만 조회

---

## Contact

- GitHub: [github.com/gguatit](https://github.com/gguatit)
- Email: [dev@kalpha.kr](mailto:dev@kalpha.kr)
