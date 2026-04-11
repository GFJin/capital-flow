---
title: "PIK (Payment-in-Kind, 현물 지급)"
type: concept
tags: [private-equity, bonds, liquidity, interest-rate, us, developed-markets, structural, cyclical, advanced, well-established]
created: 2026-04-12
updated: 2026-04-12
sources: ["raw/2026-02-03_report_private-credit-market-overview.pdf"]
confidence: high
---

# PIK (Payment-in-Kind, 현물 지급)

## 정의

PIK(Payment-in-Kind, 현물 지급)란 이자·배당·원금 등을 현금 대신 채권·주식·재고 등 비현금 수단으로 지급하는 방식이다. [[concepts/private-credit|사모대출]] 맥락에서는 차입자가 현금 이자를 지급하는 대신, 그 금액을 원금에 가산하거나(원금 복리 누적) 추가 채권을 발행하는 형태로 이자 지급을 유예한다. 이는 차입자의 단기 현금 흐름 부담을 줄여주는 대신, 만기 시 상환해야 할 원금을 지속적으로 키운다.

## 작동 방식

**설계 시 PIK (Good PIK / Designed PIK)**: 처음부터 PIK 조건으로 설계된 대출. 스타트업, 성장 단계 기업, LBO(차입 매수) 구조에서 초기 현금흐름이 부족할 때 의도적으로 사용한다. 투자자도 높은 최종 수익률(yield-to-maturity)을 기대하고 이를 수용한다.

**전환 PIK (Bad PIK)**: 당초 현금 이자 지급 조건으로 대출을 받았으나, 차입자의 재무 상태 악화로 인해 이자를 현금으로 지급하지 못하게 되어 PIK로 전환된 대출. 이 경우 PIK 전환은 사실상의 [[concepts/shadow-default|그림자 파산]] 신호이며, 상환 불가능성을 내포한다.

**원금 복리 누적 효과**: 이자가 원금에 가산되면 다음 기간의 이자 계산 기준이 늘어나므로(compounding), 시간이 갈수록 부채 총액이 기하급수적으로 증가한다. 만기 시점에 차입자가 갚아야 할 금액은 원래 대출 원금보다 훨씬 커진다.

## 핵심 파라미터

| 지표 | 수치 | 출처·시점 |
|------|------|----------|
| 사모대출 중 PIK 사용 비중 | 10.6% | 2025년 3분기말 (Lincoln International) |
| ↳ 2021년말 PIK 비중 | 7.0% | 비교 기준 (증가세 확인) |
| PIK 중 "Bad PIK" 비중 | 57.2% | 2025년 3분기말 |
| ↳ 2021년말 Bad PIK 비중 | 36.7% | 비교 기준 |

**해석**: 2021→2025년 PIK 비중이 7.0%→10.6%로 증가한 가운데, PIK 중 Bad PIK 비중이 36.7%→57.2%로 더 빠르게 상승. 이는 신규 사모대출 중 전략적 PIK 설계보다 재무 악화로 인한 PIK 전환이 더 빠르게 늘고 있음을 시사한다.

## 활용 시점

- **사모대출 포트폴리오 건전성 점검**: PIK 비중, 특히 Bad PIK 비중은 공식 부도율이 낮게 유지되더라도 실질 신용 질 저하를 감지하는 선행 지표로 활용.
- **수익률 분석**: 이자가 현금으로 유입되지 않으므로 실제 현금수익률(cash yield)과 장부상 수익률(accrual yield)의 차이를 구분해야 한다.
- **LBO/PE 구조 분석**: 차입 매수 거래에서 PIK 채권이 자본 구조의 최열후위(junior most)에 위치하는 경우가 많아, 손실 흡수 순서 파악 시 중요.

## 리스크 및 함정

- **현금흐름 착시**: PIK 이자는 회계상 수익으로 잡히지만 현금으로 수취하지 못하므로, 운용사의 실제 현금흐름을 과대평가하게 만든다.
- **부채 눈덩이(Debt Snowball)**: 이자가 원금에 가산될수록 절대 부채 규모가 빠르게 늘어 만기 상환 부담이 가중된다.
- **가치평가 왜곡**: mark-to-model 환경에서 PIK 대출 자산의 가치는 주관적으로 평가되므로, 손실이 늦게 인식될 수 있다.
- **감독 사각지대**: PIK 전환은 공식 구조조정이나 부도 이벤트로 분류되지 않으므로, 규제 보고서나 부도 통계에서 포착되지 않는다.

## 관련 개념

- [[concepts/shadow-default]] — PIK 전환이 실질 부도를 숨기는 핵심 메커니즘
- [[concepts/private-credit]] — PIK가 구조적으로 가능한 시장 맥락
- [[concepts/business-development-company]] — BDC 포트폴리오에서 PIK 노출이 NAV 변동으로 이어짐
- [[concepts/procyclical-leverage]] — 경기 하강 시 Bad PIK 급증 → 실질 부도 한꺼번에 표면화 → 레버리지 축소 연결

## 출처

- [[summaries/kcif-private-credit-market-overview-260203]] — KCIF 2026-02-03: PIK 정의, PIK·Bad PIK 비중 통계 제공
