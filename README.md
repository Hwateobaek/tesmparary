# 피카츄 미니게임 ⚡

의존성 없는 단일 HTML 미니게임 모음. 허브(메뉴)에서 게임을 골라 플레이합니다. 피카츄 테마 · 모바일 반응형.

## 플레이

- **온라인 허브:** https://hwateobaek.github.io/Game/
- **로컬:** 루트 `index.html`(허브) 또는 각 게임의 `<slug>/index.html`을 브라우저로 열기

## 구조

```
index.html          # 허브(메뉴) — GAMES 배열로 게임 목록 관리
assets/             # 공용 이미지 (pikachu / pika-happy / pika-angry)
reflex/index.html   # 반사신경 테스트 (완료)
<slug>/index.html   # 게임별 폴더 (memory, whack, rhythm, simon, slide, merge …)
```

게임에서는 이미지를 `../assets/...`, 허브에서는 `assets/...`로 참조합니다.

## 게임 목록

| slug | 게임 | 상태 |
|------|------|------|
| reflex | 🎯 반사신경 테스트 | ✅ 완료 |
| memory | 🃏 기억력 카드 매칭 | 준비 중 |
| whack | 🔨 피카츄 잡기 | 준비 중 |
| rhythm | 🎵 리듬 탭 | 준비 중 |
| simon | 🌈 색깔 순서 기억 | 준비 중 |
| slide | 🧩 슬라이딩 퍼즐 | 준비 중 |
| merge | 🔢 합치기 퍼즐 (2048) | 준비 중 |

## 공통 규칙

Web Audio 실시간 합성 사운드(저작권 프리) + 음소거, localStorage 랭킹, 세션당 1회 인트로,
일시정지/종료, 모바일·태블릿 반응형. 새 게임은 `game-maker` 스킬과 공통 템플릿을 사용해 제작합니다.

© copyright 청주여자고등학교 백승관 선생님
