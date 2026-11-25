# gguatit

**kalpha** · Web & API Security / Backend

웹/API 보안과 백엔드 엔지니어입니다. OpenAPI 기반 API를 설계하고 공격 시나리오를 분석하며, 재현 가능한 PoC로 검증합니다.

<p align="center">
  <img src="https://img.shields.io/github/followers/gguatit?style=social" alt="GitHub 팔로워" />
  <img src="https://hits.sh/github.com/gguatit.svg?label=Profile%20visitors&color=0e75b6" alt="프로필 방문자" />
  <a href="https://hub.xerj.org/contributors/gguatit"><img src="https://hub.xerj.org/contributors/gguatit/badge.svg" alt="XERJ Corpus Hub 기여자" /></a>
</p>

---

## Profile

웹 보안 / API 보안 / 백엔드 개발 중심으로 활동  
OpenAPI 기반 API 설계 및 공격 시나리오 분석  
재현 가능한 PoC 기반 검증을 기준으로 보안 테스트 수행

---

## Core Focus

- 웹 애플리케이션 보안 (XSS, Injection, 인증 우회)
- API 보안 (스키마 검증, 요청 변조)
- 백엔드 아키텍처 (OpenAPI, RESTful 설계)

---

## Tech Stack

<table>
<tr>
<td width="20%"><b>Backend</b></td>
<td>
Rust<br/>
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
- 실시간 익명 채팅 서비스
- 최소 사용자 식별 아키텍처

**Security**
- 입력 검증 / 출력 인코딩
- XSS·인젝션 방어 설계
- 클라이언트 렌더링 공격 벡터 검증

**위협 모델**

<table>
<tr><td width="20%"><b>공격자</b></td><td>인증되지 않은 외부 사용자</td></tr>
<tr><td><b>목표</b></td><td>인증 우회 / 데이터 접근</td></tr>
<tr><td><b>벡터</b></td><td>XSS / 인젝션 / 요청 변조</td></tr>
</table>

**XERJ Corpus Hub**
- XERJ 선택 커밋: [`e57e898a51`](https://github.com/gguatit/Anonymous_Chat/commit/e57e898a51) — 공지사항을 D1에 영구 저장, Durable Object 저장 한도로 인한 공지 유실 수정
- [기여자 프로필](https://hub.xerj.org/contributors/gguatit) · AGPL-3.0 코퍼스, 라이선스 검토 중 (아직 설치 불가)

---

### XMem
[Xeon-Security/XMem](https://github.com/Xeon-Security/XMem)

**Stack**: Rust · egui · Windows 사용자 모드

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
- API 키 / 관리자 인증 (12h JWT, PBKDF2-SHA256, HMAC-signed httpOnly cookie)
- IP rate limit (60/min), 업로드 크기 제한 (50MB / chunked 250MB)
- UUID v4 파일 ID, attachment + nosniff, CORS allowlist, 만료 검사

---

### Cue
[gguatit/cue](https://github.com/gguatit/cue)

**Stack**: Tauri 2 · Rust · React 19 · Windows

**Overview**
- 포인터 아래 문제를 캡처해 AI에 묻고 답을 눈에 덜 띄게 보여 주는 Windows 시험 도우미
- 단축키 + 마우스 클릭 한 번으로 캡처·요청, 답은 오버레이·트레이·키보드 LED·화면 밝기로 표시

**Security**
- 서버·계정·텔레메트리 없이 로컬에서 동작, API 키는 Windows 자격증명 관리자에만 저장
- 공급자 엔드포인트 고정, 커스텀 URL은 HTTPS/루프백 HTTP만 허용하고 리다이렉트 미추적
- 화면 캡처 보호 적용에 실패하면 답을 숨기는 fail-closed, 서명된 업데이트만 사용

---

## Contact

- GitHub: [github.com/gguatit](https://github.com/gguatit)
- Email: [dev@kalpha.kr](mailto:dev@kalpha.kr)
