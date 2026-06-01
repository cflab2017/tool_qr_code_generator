# QR 코드 생성기

텍스트·URL·WiFi·vCard를 QR 코드로 즉시 변환하고 PNG·SVG로 다운로드하는 **단일 HTML** 도구. 중앙 로고 임베드와 색상 커스터마이즈까지 한 파일에서.

**🔗 라이브**
- 홈페이지: <https://www.coding-now.com/qrcode>
- GitHub Pages: <https://cflab2017.github.io/tool_qr_code_generator/>

🎬 **데모:** [docs/demo.html](./docs/demo.html) — 약 21초 자동 재생 시연 (자막 동기, [WebVTT](./docs/demo.vtt))

## 특징

- **4가지 모드**
  - **텍스트 / URL** — UTF-8(한글·이모지·일본어) 지원
  - **WiFi 접속** — SSID·암호·암호화·숨김 → 스캔 즉시 "네트워크에 연결" (iOS·Android 기본 카메라)
  - **vCard 명함** — 이름·전화·이메일·회사·직책·URL → 스캔 한 번에 연락처 저장
- **중앙 로고 임베드** — PNG/JPG/SVG 업로드, 10–30% 크기 슬라이더, 자동 H 레벨 잠금으로 스캔 신뢰도 보호
- **PNG · SVG** 양쪽 다운로드 — SVG는 로고까지 base64로 self-contained
- **색상 커스터마이즈** — 전경·배경 자유 선택
- **에러 정정 레벨** L/M/Q/H 선택, 로고 사용 시 자동 H로 잠금
- **프라이버시** — 모든 변환이 브라우저 안에서 끝남, 서버 업로드 없음
- 빌드 도구·서버·프레임워크 없음 — `index.html` 한 파일
- **SEO 리치 스니펫** — `SoftwareApplication` + `FAQPage` JSON-LD 내장

## 이런 곳에 씁니다

- 카페·식당·매장 — 와이파이 안내, 메뉴판, 주문·리뷰 링크
- 명함·이력서·이벤트 부스 — vCard QR
- 전단·포스터·간판 — 홈페이지·예약 페이지로 즉시 이동
- 행사·전시·세미나 — 입장권·체크인·자료 다운로드
- 제품 패키지·매뉴얼 — 사용법 동영상·고객지원 링크
- 브랜드·디자인 — 로고와 색을 입힌 QR

## 사용법

`index.html`을 브라우저로 열기만 하면 끝.

```bash
# 또는 로컬 서버로 띄우기
npx http-server -p 8080 .
```

## 기술

- QR 엔진: [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) 1.4.4 by Kazuhiko Arase (MIT)
- 폰트: [JetBrains Mono](https://www.jetbrains.com/lp/mono/) + [Gowun Dodum](https://fonts.google.com/specimen/Gowun+Dodum) (Google Fonts, OFL)
- 구조화 데이터: schema.org `SoftwareApplication` + `FAQPage` JSON-LD
- 테마: 앰버 CRT 터미널

## 후원하기

도구가 도움이 됐다면 ☕ [paypal.me/codingnow](https://paypal.me/codingnow)

## 라이선스

[MIT](./LICENSE) © CODINGNOW
