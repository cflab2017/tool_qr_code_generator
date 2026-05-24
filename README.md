# QR 코드 생성기

텍스트·URL을 QR 코드로 즉시 변환하고 PNG·SVG로 다운로드하는 **단일 HTML** 도구.

🎬 **데모:** [docs/demo.html](./docs/demo.html) — 약 21초 자동 재생 시연 (자막 동기, [WebVTT](./docs/demo.vtt))

## 특징

- 실시간 미리보기 — 입력 즉시 QR 갱신, "생성" 버튼 없음
- PNG(고해상도 래스터) · SVG(벡터) 양쪽 다운로드
- 한글·이모지·일본어 등 UTF-8 텍스트 지원
- 에러 정정 레벨 선택 (L 7% / M 15% / Q 25% / H 30%)
- 전경·배경 색상 커스터마이즈
- 빌드 도구·서버·프레임워크 없음 — `index.html` 한 파일

## 사용법

`index.html`을 브라우저로 열기만 하면 끝.

```bash
# 또는 로컬 서버로 띄우기
npx http-server -p 8080 .
```

## 기술

- QR 엔진: [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) 1.4.4 by Kazuhiko Arase (MIT)
- 폰트: [JetBrains Mono](https://www.jetbrains.com/lp/mono/) + [Gowun Dodum](https://fonts.google.com/specimen/Gowun+Dodum) (Google Fonts, OFL)
- 테마: 앰버 CRT 터미널

## 후원하기

도구가 도움이 됐다면 ☕ [paypal.me/codingnow](https://paypal.me/codingnow)

## 라이선스

[MIT](./LICENSE) © CODINGNOW
