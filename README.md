# Nodit Console — Overview Redesign

Lambda256 Product Designer 과제 제출물입니다.
Nodit Console의 Overview 화면을 분석하고, 정보 위계 개선과 "Job(목적) 기반 진입점" 아이디어를
더해 다시 설계했습니다.

**Live prototype:** https://jelincc.github.io/NODIT/
**Design deck (문제 정의 · 리서치 · 가설):** https://claude.ai/code/artifact/debda4ac-5c5f-44dc-82e8-a11ed71043e1

## 무엇을 바꿨나

기존 화면 구조(사이드바, 상단바, Getting Started, My Project, Usage Detail, My Plan 등)는
그대로 유지했습니다. Overview 화면 안에 새로운 섹션 하나를 더했습니다.

- **"What are you here to do?"** — Build / Operate / Manage / Investigate / Analyze,
  다섯 가지 목적을 실제 존재하는 API 영역(Asset & Account, Payments & Transfers, Txs & Provenance,
  Datashare)으로 바로 연결하는 진입 카드 5개.

개발자가 아닌 사용자(Treasury, Operations, Compliance, Data팀)도 로그인 직후 자신의 업무와
연결되는 지점을 바로 찾을 수 있도록 하는 것이 목표입니다.

## 인터랙션

- Overview의 Job 카드 클릭 → 해당 목적의 화면으로 이동 (Asset & Account / Payments & Transfers / Txs & Provenance / Datashare)
- 사이드바 전체가 실제 동작 — Getting Started 체크리스트 토글, Usage Detail Elastic/Dedicated 탭,
  Auto-Scaling 스위치, 거래 상태 필터 등

## 저장소 구성

- `index.html` — 실제 배포되는 프로토타입
- `README.md` — 본 문서
