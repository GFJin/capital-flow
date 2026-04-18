---
title: "캐리/변동성 비율 (Carry/Volatility Ratio)"
type: concept
tags: [carry-trade, fx, japan, interest-rate, risk-appetite, quantitative, cyclical, well-established]
created: 2026-04-18
updated: 2026-04-18
sources: ["raw/Japan_FX_Capitulation_of_JPY_carry_Only_the_beginning_of_the_end-Japan_FX.pdf"]
confidence: high
---

## Definition

캐리/변동성 비율(carry/volatility ratio)은 캐리 트레이드의 수익성을 위험 대비로 측정하는 지표다. 분자는 조달통화와 투자통화 간의 금리차(carry), 분모는 해당 통화쌍의 내재 또는 실현 변동성(volatility)이다. 비율이 높을수록 캐리 트레이드는 매력적이고, 비율이 낮을수록(특히 임계값 이하) 포지션 청산 압력이 강해진다.

## How It Works

- **계산 방식**: `Carry/Vol Ratio = 금리차(%) / 환율 변동성(%)`
  - 예: 3개월 USD-JPY 금리차 5.2%, 3개월 USDJPY 내재 변동성 10.4% → 비율 = 50%
- **해석**: 비율이 높으면 변동성 대비 수익이 충분해 포지션 유지 유인 강함. 비율 하락은 환 변동성 확대 또는 금리차 축소로 인해 캐리 매력도가 감소함을 의미
- **역사적 임계값 (USDJPY 기준)**:

| 이벤트 | 시기 | 비율 수준 |
|--------|------|---------|
| LTCM 쇼크 | 1998 | 40% 미만으로 하락 |
| 닷컴 버블 붕괴 | 2002 | 40% 미만으로 하락 |
| GFC (글로벌 금융위기) | 2007~2008 | 40% 미만으로 하락 |
| 2024년 8월 급락 | 2024-08 | 50% 아래로 하락 (40% 미만 미도달) |

- **2024년 시사점**: Citi Research(2024-08-05)는 비율이 막 50%를 하회했을 때 보고서를 발행. 과거 대세 전환 사례에서는 40% 미만이 조건이었으므로, 현재 청산은 완결되지 않았다고 판단

## Key Parameters

| 변수 | 역할 |
|------|------|
| 미-일 단기금리차 | 비율의 분자. BOJ 금리 인상 또는 Fed 금리 인하 시 분자 감소 |
| USDJPY 내재 변동성 | 비율의 분모. 시장 불확실성 확대 시 분모 증가 → 비율 감소 |
| 기준 임계값 (40%) | 과거 사례 기반 대세 전환 기준. 단, 구조적 변화(FX 개입 등)로 임계값 자체가 이동 가능 |
| 측정 기간 | 주로 3개월 기준 사용. 기간에 따라 비율 수준 상이 |

## When To Use

- USDJPY 캐리 트레이드 포지션의 청산 개시 여부 모니터링
- 과거 대세 전환 사례와 현재 비율 비교로 청산 완결 가능성 판단
- [[concepts/carry-trade-unwind]] 발동 타이밍 사전 경보 지표로 활용
- [[concepts/yen-carry-trade]] 포지션 재구축 여건 평가 (비율 상승 반전 시)

## Risks & Pitfalls

- **구조적 변화에 의한 임계값 이동**: FX 개입 누적, 중앙은행 가이던스 변화 등이 과거 임계값의 유효성을 약화시킬 수 있음. Citi는 2024년 청산이 40% 미도달 시점에 발생한 이유로 일본 정부의 FX 개입 누적 효과를 지목
- **단일 지표의 한계**: 비율만으로 청산 여부를 판단하기 어려움. 금리차 절대 수준, 포지션 규모(CitiFX Position Index 등), 글로벌 위험 지표와 병행 모니터링 필요
- **변동성 측정 방식**: 내재 변동성(옵션 기반)과 실현 변동성 중 어느 것을 사용하느냐에 따라 비율이 달라짐

## Related Concepts

- [[concepts/yen-carry-trade]] — 캐리/변동성 비율이 높을 때 포지션 구축이 활발해지는 전략
- [[concepts/carry-trade-unwind]] — 비율이 임계값 이하로 하락할 때 청산이 가속되는 메커니즘
- [[concepts/crowded-trade]] — 누적 포지션이 클수록 비율 하락 시 충격 더 큼
- [[concepts/dollar-cycle]] — 금리차 방향을 결정하는 달러 사이클

## Sources

- `raw/Japan_FX_Capitulation_of_JPY_carry_Only_the_beginning_of_the_end-Japan_FX.pdf` — Citi Research (Osamu Takashima 외), 2024-08-05
