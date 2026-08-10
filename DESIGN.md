# Nodit Console — Overview 개선 설계 노트

전체 리서치 과정(문제 정의 → 제안 방향 → Persona/Job 정리 → 정보 구조 → 가설과 검증)은
아래 디자인 덱에 정리했습니다.

**Design deck:** https://jelincc.github.io/NODIT/design/
**Live prototype:** https://jelincc.github.io/NODIT/

## 요약

- **문제**: Overview 화면이 로그인 목적(내 프로젝트·사용량 확인)보다 프로모션·광고를 먼저
  보여주고, 핵심 정보는 스크롤해야 나타납니다. 신규 가입자는 빈 그래프만 보고, 업그레이드
  버튼은 세 군데에 흩어져 있습니다.
- **제안**: 기존 화면 구조(사이드바, Getting Started, My Project, Usage Detail, My Plan)는
  유지하면서, Overview 안에 "What are you here to do?" 섹션을 추가했습니다. Build / Operate /
  Manage / Investigate / Analyze 다섯 가지 목적을 실제 API 영역(Asset & Account, Payments &
  Transfers, Txs & Provenance, Datashare)으로 바로 연결합니다.
- **근거**: Nodit을 쓰는 사람은 개발자만이 아닙니다. Treasury, Operations, Compliance, Data팀도
  같은 콘솔을 씁니다. 다섯 가지 목적 모두 결국 Wallet · Transaction · Transfer · Asset이라는
  같은 데이터를 참조하기 때문에, 화면을 나누지 않고 하나의 Overview 안에 진입점만 추가했습니다.

자세한 내용, 가설과 검증 계획, Persona/Job Matrix, 정보 구조 다이어그램은 디자인 덱을
참고해 주세요.
