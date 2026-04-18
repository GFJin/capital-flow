---
title: "CTA / 추세 추종 전략 (CTA / Trend Following)"
type: concept
tags: [portfolio-flow, equities, fx, commodities, bonds, risk-appetite, liquidity, quantitative, cyclical, well-established]
created: 2026-04-18
updated: 2026-04-18
sources: ["raw/2024-08-09-Societe Generale-The Systematic Investor Report - Recent market turmoil _ Wha...-109778177.pdf"]
confidence: high
---

## Definition

CTA(Commodity Trading Advisor)는 주로 선물 시장에서 시스템적 추세 추종(trend following) 전략을 운용하는 헤지펀드 범주다. 가격의 모멘텀(과거 추세)을 포착해 롱/숏 포지션을 구축하며, 주식·채권·외환·원자재 등 다양한 자산군을 동시에 운용하는 멀티-에셋 전략이 대표적이다. 추세가 없거나 급반전이 발생하면 큰 손실을 기록하는 구조적 취약점이 있다.

## How It Works

**포지셔닝 메커니즘**:
- 각 자산의 과거 가격 데이터에 기반해 모멘텀 신호 생성 (단기/중기/장기 이동평균 등)
- 신호가 양(+)이면 롱, 음(-)이면 숏. 신호 강도에 따라 포지션 크기 조정
- 전략 간 상관관계가 낮아 포트폴리오 분산 효과가 크다고 알려짐 — 특히 주식 하락기에 채권 롱으로 헤지

**손익 특성**:
- 추세가 지속되는 환경에서 강점. 주요 수익원: 장기 추세 포착
- **약점**: 급반전(sharp reversal) 시 큰 손실. 특히 모멘텀이 반전될 때 포지션 전환 지연으로 손실 누적
- 변동성 피킹(volatility peak) 직후 손실이 크고, 이후 새 추세 형성 시 회복

**포지션 전환 예시 (2024년 8월)**:
```
자산군       이전 포지션   전환 후 포지션   배경
JPY/USD      롱(엔 약세 추세)  플랫(중립)    엔화 급등으로 추세 반전
채권(미·캐·영)  숏           롱             침체 우려 + Fed 금리 인하 재가격
주식(NKY·S&P)  롱           여전히 롱      하락에도 아직 포지션 미전환 → 리스크 잔존
```

## Key Parameters

| 지표 | 역할 |
|------|------|
| SG Trend Index | 글로벌 CTA 전략 대표 지수 |
| 포지션 분위수 (5년 기준) | 현재 포지션이 과거 5년 역사에서 어느 위치인지 |
| Days in Position | 포지션 보유 기간 — 길수록 역모멘텀 리스크 누적 |
| Monthly / YTD 성과 | 전략 손익 모니터링 |
| 자산군별 총 포지셔닝 지수 | -1(완전 숏)에서 +1(완전 롱) 사이 집계 신호 |

**2024-08-09 기준 CTA 전체 포지셔닝 요약**:
- 주식: 롱 편향 (대부분 지수 롱 유지 — 추가 하락 시 손실 위험)
- 통화: JPY·CHF·EUR 중립, AUD·NZD·CAD 숏
- 채권: 주중 숏→롱 전환 (경기침체 시나리오)
- 원자재: 금 롱, 에너지 플랫, 농산물 숏 (경기침체 배팅)

## When To Use

- **자본 흐름 예측**: CTA가 대규모 포지션 전환 시 해당 자산군에 수급 충격 발생. 특히 CTA가 JPY 롱을 구축할 경우 엔화 강세 압력 추가
- **캐리 청산과의 상호 작용**: [[concepts/yen-carry-trade]] 청산 발생 시 CTA도 동일 방향(JPY 매수)으로 전환 → 충격 증폭
- **추세 전환 판단**: CTA 포지셔닝이 극단적 수준(분위수 90% 이상)에 도달하면 반전 리스크 모니터링
- **포트폴리오 분산**: CTA는 주식 하락기에 채권·금 롱으로 자연 헤지 기능 제공 — 단, 급반전 구간에서는 역효과

## Risks & Pitfalls

- **트렌드 없는 구간 (Whipsaw)**: 방향성 없는 시장에서 반복 손절로 비용 누적
- **추세 반전 지연 인식**: 새로운 추세가 시작됐음을 포지션이 인식하는 데 수일~수주 소요. 이 기간 중 손실 노출
- **동질성 리스크**: 많은 CTA가 유사한 신호를 사용해 같은 방향으로 포지션을 구축 → 일제 청산 시 [[concepts/crowded-trade]] 문제 발생
- **급반전 사례**: 2024년 8월 SG Trend Index는 2024년 수익 대부분을 며칠 만에 반납. 원인: 상품 가격 반전 후 주식 급락

## Related Concepts

- [[concepts/carry-trade-unwind]] — CTA가 엔캐리 청산 시 JPY 매수 포지션으로 전환하며 청산 가속
- [[concepts/carry-vol-ratio]] — 변동성 급등 후 CTA의 포지션 전환 트리거
- [[concepts/crowded-trade]] — CTA 동질 포지셔닝이 일제 청산 시 충격 배가
- [[concepts/tail-hedge]] — CTA 손실 구간에서 꼬리 헤지 전략이 보완 기능
- [[concepts/dollar-cycle]] — 달러·엔 방향이 CTA 통화 포지셔닝의 핵심 변수

## Sources

- `raw/2024-08-09-Societe Generale-The Systematic Investor Report - Recent market turmoil _ Wha...-109778177.pdf` — SG Cross Asset Quant (Sandrine Ungari 외), 2024-08-09
