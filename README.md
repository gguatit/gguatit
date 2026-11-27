# gguatit

**kalpha** · AI · Server · Security

AI 기능을 만들고, 서버로 운영하고, 보안으로 검증합니다.

---

## Focus

- **AI** — 멀티 프로바이더 하네스, 비전 입력, SSE 스트리밍
- **Server** — Spring Boot 운영, Cloudflare Workers · Durable Objects
- **Security** — HMAC · Turnstile · CSP, fail-closed 설계

---

## Projects

### Cue — AI · Security
[gguatit/cue](https://github.com/gguatit/cue)

- Tauri 2 · Rust · React 19 기반 Windows 데스크톱 앱, 단축키를 누른 채 클릭 한 번으로 캡처부터 AI 응답까지
- OpenAI 호환 · Anthropic · Google을 공통 계약으로 묶은 Rust AI 하네스 (비전 입력, SSE 스트리밍, fallback, 교차 검증)
- API 키는 Windows 자격증명 관리자에만 저장, 캡처 보호 실패 시 응답 숨김, 서명된 업데이트

### STARLOG — Server · Security (팀)
[gguatit/mirae-yumang-team-server](https://github.com/gguatit/mirae-yumang-team-server)

- Spring Boot 3.5 · Java 17 · MySQL 기반 학교 커뮤니티, Cloudflare Tunnel로 배포·운영
- 담당: 서버 구축·운영, 오늘의 운세 AI ([Today's Horoscope](https://github.com/gguatit/Today-s-horoscope))
- OAuth2(GitHub/Google) · Turnstile · BCrypt · IP+계정 5회 실패 시 15분 잠금 · Jsoup XSS 필터 · Path Traversal 방지

### Anonymous Chat — AI · Server · Security
[gguatit/Anonymous_Chat](https://github.com/gguatit/Anonymous_Chat)

- Cloudflare Workers · Durable Objects · D1 기반 익명 실시간 채팅, 12시간 후 메시지 자동 소멸
- HMAC 메시지 서명 · Turnstile 티켓 바인딩 · Origin 검증 fail-closed · CSP/HSTS
- Workers AI(Gemma/Qwen) 대화 요약 4모드, Vitest 657개

### Today's Horoscope — AI
[gguatit/Today-s-horoscope](https://github.com/gguatit/Today-s-horoscope) · [kalpha.c01.kr](https://kalpha.c01.kr)

- STARLOG의 오늘의 운세 기능을 Workers AI(Llama 3.1 8B) · D1 · SSE 스트리밍으로 구현
- JWT(HS256) · PBKDF2 10만 회 · 파라미터 바인딩 · 입력 이스케이프

---

## Tech Stack

| Area | Stack |
|---|---|
| **Backend** | Rust · Java 17 (Spring Boot) · TypeScript · WebSocket |
| **Frontend** | React · Vanilla JS |
| **AI** | Workers AI · OpenAI-compatible · Anthropic · Google · SSE |
| **Cloud / Data** | Cloudflare Workers · D1 · Durable Objects · KV · MySQL |
| **Security** | HMAC · JWT · OAuth2 · Turnstile · CSP · Kali Linux · Burp Suite · Wireshark |
| **Infra** | Cloudflare Tunnel · Docker · Git |

---

## Activity

<p align="center">
  <img src="https://streak-stats.demolab.com?user=gguatit&theme=tokyonight&hide_border=true" width="48%" alt="GitHub streak stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=gguatit&layout=compact&theme=tokyonight&hide_border=true" width="48%" alt="Top languages" />
</p>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=gguatit&theme=tokyonight" width="96%" alt="GitHub profile details" />
</p>
