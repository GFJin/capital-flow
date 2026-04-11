---
title: "그림자 파산 (Shadow Default)"
type: concept
tags: [private-equity, bonds, liquidity, interest-rate, us, developed-markets, structural, cyclical, advanced, well-established]
created: 2026-04-12
updated: 2026-04-12
sources: ["raw/2026-02-03_report_private-credit-market-overview.pdf"]
confidence: high
---

# 그림자 파산 (Shadow Default)

## 정의

그림자 파산(Shadow Default)이란 [[concepts/private-credit|사모대출]] 시장에서 차입 기업이 사실상 채무불이행 상태에 있음에도 불구하고, 공식 부도 처리 대신 대출 만기 연장·조건 변경·[[concepts/pik-payment-in-kind|PIK]] 옵션 전환 등을 통해 그 사실이 표면적 통계에 나타나지 않는 현상을 말한다. 실제 신용 손실이 숨겨진 채 누적되는 구조적 왜곡이다.

## 작동 방식

사모대출은 2차 시장이 없고 대출자와 차입자 간 직접 협상이 가능하므로, 차입자가 상환 불능에 처했을 때 공개 시장에서 자동으로 가격이 반영되지 않는다. 대신 아래 세 가지 우회 경로가 부도를 숨긴다.

**1. 만기 연장(Maturity Extension)**: 차입자가 원금을 상환할 수 없는 상황에서 대출자가 만기일을 연장해 디폴트 이벤트를 미룬다. 공식 통계상 부도로 잡히지 않는다.

**2. 계약 조건 조정(Covenant Amendment / Amend-and-Extend)**: 당초 대출 약정에 명시된 재무 비율(leverage ratio, interest coverage ratio 등)을 하향 조정하거나, 위반 시 페널티를 면제하는 방식으로 사실상의 구제를 제공한다.

**3. PIK 전환(Bad PIK)**: 현금 이자를 지급할 능력이 없는 차입자가 이자 대신 원금에 가산하거나 추가 채권 발행(PIK; Payment-in-Kind)으로 지급을 미룬다. 특히 대출 설계 시부터 PIK가 아니었음에도 재무 악화 이후 PIK로 전환된 "Bad PIK"가 증가하면, 실질적인 부실이 누적되고 있음을 시사한다.

## 핵심 파라미터

| 지표 | 수치 | 출처·시점 |
|------|------|----------|
| 미국 사모대출 공식 부도율 | 2.46% | 2025년 4분기 (Proskauer Rose LLP) |
| 사모대출 중 PIK 사용 비중 | 10.6% | 2025년 3분기말 (Lincoln International) |
| ↳ 2021년말 PIK 비중 | 7.0% | 비교 기준 |
| PIK 중 "Bad PIK" 비중 | 57.2% | 2025년 3분기말 |
| ↳ 2021년말 Bad PIK 비중 | 36.7% | 비교 기준 |

**해석**: 공식 부도율 2.46%는 낮아 보이나, Bad PIK 비중이 36.7%→57.2%로 상승했다는 것은 PIK 전환의 절반 이상이 "이자를 지급하지 못해 전환"된 사실상의 부도임을 의미한다.

## 활용 시점

- **사모대출 포트폴리오 리스크 평가**: 공식 부도율만 보면 안전해 보이는 사모대출 시장의 실질 건전성을 평가할 때.
- **신용 사이클 분석**: 피크 이후 신용 질 저하가 공식 통계보다 빠르게 진행될 수 있음을 감안할 때.
- **감독·규제 논의**: FSB, 연준, 법무부 등의 투명성 강화 요구의 배경을 이해할 때.

## 리스크 및 함정

- **데이터 제약**: 사모대출의 폐쇄적 특성상 데이터 제공업체 표본이 제한적이어서 시장 전체의 부실 규모를 온전히 파악하기 어렵다.
- **후행성**: 리사 쿡 연준 이사 지적처럼 부도율은 후행 지표(lagging indicator)이므로, 문제가 가시화될 때는 이미 손실이 상당 규모에 달해 있을 수 있다.
- **숨겨진 레버리지**: 기업이 PIK를 통해 부채를 계속 쌓으면 총 레버리지가 가파르게 상승하여 최종 손실이 설계 시점 예상을 크게 초과할 수 있다.
- **전염 리스크**: 그림자 파산이 일정 시점에 한꺼번에 표면화될 경우 사모대출 시장 전반의 신뢰 붕괴로 이어질 수 있다.

## 관련 개념

- [[concepts/pik-payment-in-kind]] — 그림자 파산의 핵심 도구; Bad PIK 전환 메커니즘
- [[concepts/private-credit]] — 그림자 파산이 발생하는 시장 맥락
- [[concepts/business-development-company]] — BDC 가치평가에 직접 영향
- [[concepts/procyclical-leverage]] — 부실이 누적된 후 한꺼번에 드러날 때 경기순응적 레버리지 축소와 맞물림

## 출처

- [[summaries/kcif-private-credit-market-overview-260203]] — KCIF 2026-02-03: 그림자 파산 개념화, PIK 통계 제공
