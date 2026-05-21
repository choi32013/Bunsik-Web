# Bunsik — Web Playtest Mirror

브라우저에서 바로 플레이 가능한 **Bunsik (분식)** 게임 (Godot 4.4 Web Export).

## ▶ 플레이

🎮 **https://choi32013.github.io/Bunsik-Web/**

## 소개

한국 분식집 운영 게임. 컨베이어 벨트로 흘러오는 재료를 잡아 손님 주문 요리(떡볶이/김밥/라볶이/순대)를 완성하세요.

- **요리 4종**: 떡볶이, 김밥, 라볶이, 순대
- **재료 10종**: 떡 / 어묵 / 고추장 / 밥 / 김 / 단무지 / 햄 / 라면 / 순대 / 소금
- **장애물**: 쓰레기 (-10점), 폭탄 (즉사), 매운 폭탄 (속도 부스트)
- **별점 시스템**: 인내심 비율 + 함정 횟수로 ★1~★5
- **게임 오버**: 연속 ★1 또는 분노 손님 3명, 또는 폭탄 직격

## 기술 스택

- Godot 4.4 stable
- GDScript
- Noto Color Emoji bundled
- 16-bit 픽셀아트 스프라이트
- 컨베이어 벨트 메커니즘

## 빌드 사이클

이 저장소는 main repo (`choi32013/Bunsik`, private) 에서 web export 한 파일을 미러링합니다.
업데이트는 Bunsik-Lead 가 새 빌드 시점에 푸시합니다.

## 알려진 제약

- WebAssembly 다운로드 ~54MB (첫 로드 시 시간 소요)
- SharedArrayBuffer 미사용 (nothreads 빌드) — GitHub Pages 호환
- 모바일 브라우저: Chrome / Safari iOS 모두 지원하나 첫 로드는 wifi 권장
- 진행 상태/세이브는 브라우저 LocalStorage 사용

## 라이선스

게임 자체: 소유 (Owner: HWCHOI3 / choi32013)
폰트: Noto Color Emoji (SIL OFL 1.1)
