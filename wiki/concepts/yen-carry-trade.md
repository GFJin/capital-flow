---
title: "엔 캐리 트레이드 (Yen Carry Trade)"
type: concept
tags: [carry-trade, fx, japan, interest-rate, risk-appetite, portfolio-flow, dollar-cycle, well-established]
created: 2026-04-17
updated: 2026-04-17
sources: ["raw/20240417_B_20210092_852.pdf"]
confidence: high
---

## Definition

엔 캐리 트레이드란 저금리 통화인 일본 엔화를 차입(또는 매도)하여 금리가 높은 국가의 자산에 투자함으로써 금리 차이와 환율 변동에서 수익을 추구하는 거래다. 일본은행(BOJ)의 장기 완화 정책으로 엔화가 글로벌 신용 공급 통화(funding currency)로 자리잡았으며, 1990년대 중반부터 본격화됐다.

## How It Works

**수익 구조**:
- 수익 = 금리 효과 + 환율 효과
- 달러-엔 캐리 지수 공식: `Carry_t = Long_t − Short_t`
  - `Long_t = (1 + USD3m[t]/26000) × (USDJPY[t] / USDJPY[t-1])`
  - `Short_t = (1 + JPY3m[t]/26000)`
- 달러/엔 환율이 캐리 지수 성과의 대부분을 결정. 환율 변동성이 낮을 때 금리차만으로도 안정적 수익 가능

**투자자 B/S 변화**:
- 최초: 일본에서 저금리 차입 → 외환시장에서 엔화 매도·투자통화 매수 → 고금리 자산 투자
- 청산 시: 해외 투자자산 매각 → 투자통화 매도·엔화 매수 → 엔화 차입 상환

**포지션 구축 조건** (5가지 모두 충족 시 활발):
1. BOJ 저금리 유지 + 엔화 약세 지속 기대
2. 일본 내 풍부한 유동성
3. 고수익 해외 투자처 존재
4. 제한적 환 변동성
5. 위험자산 선호 심리 우세

## Key Parameters

| 변수 | 역할 |
|------|------|
| 미-일 금리차 | 캐리 수익의 금리 효과 결정 |
| USDJPY·EURJPY 환율 변동성 | 실질 청산 촉발 요인 |
| 엔화 투기적 포지션(CME) | 포지션 누적·청산 규모 추정 |
| 일본 소재 외국계 은행 본점 송금액 | 글로벌 자금 흐름 대체지표 |
| 해외 엔화 신용 차입 잔액 | 캐리 규모 추정 |
| JP Morgan Global FX Volatility Index | 환 변동성 모니터링 |
| Barclays/JP Morgan 캐리 트레이드 지수 | 성과 측정 |

**주요 조달 통화(funding currency)**: 엔화, 달러, 스위스 프랑
**주요 투자 통화(target currency)**: 호주 달러, 뉴질랜드 달러, 신흥국 통화, 고금리 국면의 달러·유로

## When To Use

- 달러/엔 환율 방향성 분석 시 기준 프레임워크
- 글로벌 위험선호 심리 변화의 선행지표로 활용
- 한국·신흥국 증시에 대한 외국인 수급 방향 예측
- BOJ 통화정책 전환의 글로벌 파급 효과 분석

## Risks & Pitfalls

- **비대칭성**: 포지션 구축은 점진적이나 청산은 급격. 차입통화 강세 → 성과 악화 → 추가 청산의 자기강화 루프
- **환차손 리스크**: 투자통화 절하 시 금리 수익을 초과하는 손실 발생 가능
- **규모 측정 어려움**: 엔캐리 트레이드의 정확한 시점·규모·자금 흐름 추적 불가. 대체변수로만 추정
- **USD·EUR 캐리의 비동조화**: 달러-엔과 유로-엔 캐리지수는 시기에 따라 다른 흐름. 구분 분석 필요

## Related Concepts

- [[concepts/carry-trade-unwind]] — 청산 메커니즘·5차 역사 케이스
- [[concepts/fx-hedging]] — 환율 리스크 관리
- [[concepts/dollar-cycle]] — 달러 사이클과 엔화 방향성
- [[concepts/crowded-trade]] — 대규모 누적 포지션의 집중 리스크
- [[concepts/risk-appetite]] — 위험선호 전환이 캐리 청산 촉매
- [[concepts/cross-currency-basis]] — 통화 간 자금 조달 비용

## Sources

- `raw/20240417_B_20210092_852.pdf` — 교보증권 리서치센터, 2024-04-17
