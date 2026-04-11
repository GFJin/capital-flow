---
title: "BDC (Business Development Company, 기업개발회사)"
type: concept
tags: [private-equity, bonds, portfolio-flow, liquidity, interest-rate, us, developed-markets, structural, cyclical, advanced, well-established]
created: 2026-04-11
updated: 2026-04-12
sources: ["raw/bisbull106.pdf", "raw/2026-02-03_report_private-credit-market-overview.pdf"]
confidence: high
---

# BDC (Business Development Company, 기업개발회사)

## 정의

BDC(Business Development Company, 기업개발회사)는 미국 증권거래소에 상장된 폐쇄형 투자 수단으로, 주로 중소기업에 대한 직접대출 및 지분 투자를 통해 프라이빗 크레딧 시장에 참여한다. 기관투자자 전용이던 [[concepts/private-credit]] 시장에 리테일 투자자가 접근할 수 있는 가장 중요한 통로다. 미국 프라이빗 크레딧 시장의 약 **20%**, AUM **3,000억 달러 이상**을 차지한다.

## 작동 방식

**자산 구조**: BDC 자산의 대부분은 만기 4~6년의 비유동 직접대출이다. 사모펀드(PE) 회사의 보통주·우선주 등 지분 투자가 전체 자산의 10% 미만을 차지한다.

**부채 조달 구조**:
- 펀드 매니저가 먼저 자기자본을 조달한 뒤, **은행 변동금리 신용한도(committed credit lines)**를 인출하여 일상적 운영과 신규 대출 재원으로 사용.
- 이후 **무담보 채권(unsecured notes)** 발행을 통해 자금을 추가 조달.
- 평균 BDC의 부채 구성: 은행 신용한도 약 40% + 무담보채 약 50% + 나머지 담보채.

**규제**: 현행 규정상 BDC는 부채/자본 비율(D/E ratio)을 2 이하로 유지해야 하며, 대부분의 BDC는 이 한도 이하에서 운영된다.

**상장 구조의 의미**: BDC 지분은 거래소에서 일별 거래되므로 비상장 폐쇄형 펀드와 달리 유동성이 있다. 그러나 기초 자산(직접대출)은 비유동적이어서, ETF처럼 심각한 유동성 불일치는 없으나 레버리지 리스크가 존재한다.

## 핵심 파라미터

| 파라미터 | 설명 |
|---------|------|
| **AUM** | 3,000억 달러 이상 (미국 프라이빗 크레딧의 약 20%) |
| **D/E 비율 추이** | 30%(2010년경) → 90% 이상(2025년) — 15년간 3배 증가 |
| **규제 한도** | D/E 2.0 이하 |
| **부채 구성** | 은행 신용한도 ~40%, 무담보채 ~50%, 담보채 나머지 |
| **자산 구성** | 직접대출 ~90%+, PE 지분 <10% |
| **조직 형태** | 거래소 상장형(exchange-listed), 비상장 공모형, 사모형의 세 종류 |

## 활용 시점

- **리테일-프라이빗 크레딧 연결고리 분석**: 은행 대출 → 프라이빗 크레딧 → BDC → 리테일 투자자로 이어지는 리스크 전달 경로 파악.
- **은행-NBFI 연계 모니터링**: BDC의 은행 신용한도 의존도가 높아 프라이빗 크레딧 시장 경색이 은행에 전파되는 채널.
- **경기순응적 신용공급 분석**: 경기 하강 시 BDC의 레버리지 축소 → 중소기업 신용 공급 급감 경로.

## 반유동적 BDC (Semi-liquid BDC) 환매 메커니즘

전통적 상장형 BDC 외에 **반유동적(semi-liquid) BDC**가 존재한다. 이는 분기에 한 번 투자자에게 환매 기회를 제공하되, 환매 한도를 순자산가치(NAV)의 5% 내외로 제한하는 구조다.

**2025년 4분기 환매 급증 사례**:
- 사모대출에 대한 투자심리 악화로 환매 요청이 과거 평균(NAV의 ~2%)에서 급증
- 일부 운용사는 5% 한도를 초과하여 환매 요청을 수용
- 2026년 1월 23일: BlackRock BDC(TCP Capital)의 2025년 4분기 NAV 전분기 대비 19% 하락 (Razor·Renovo 투자 손실)
- 2026년 1월 26일: BlackRock TCP Capital 주가 전일 대비 13% 급락
- Apollo는 Perch(브랜드 통합업체) 대출에서 $1.7억 손실(Bloomberg 보도)

## 리스크 및 함정

- **경기순응적 레버리지**: D/E 비율이 자산 가치 변화에 따라 급격히 등락. 경기 하강 시 자산 매각 또는 신규 대출 중단으로 신용 공급을 더욱 위축시킬 수 있다. [[concepts/procyclical-leverage]] 참조.
- **고레버리지의 주가 취약성**: 2025년 4월 "해방의 날" 에피소드에서 고레버리지 BDC가 저레버리지 BDC 대비 더 큰 주가 하락을 기록. 자기자본 잠식·채무 불이행 리스크.
- **반유동적 BDC 환매 리스크**: 분기별 환매 한도(NAV 5%)가 있으나, 투자 심리 급격 악화 시 한도 초과 환매 압력 발생. NAV 급락과 주가 급락이 동시에 일어날 수 있다.
- **가치평가 불투명성**: Renovo 파산 사례처럼 운용사(BlackRock)가 경영난 중에도 원금 100%로 평가. mark-to-model의 한계. [[concepts/shadow-default]] 참조.
- **은행 전염 경로**: BDC의 은행 신용한도 동시 인출이 은행 대차대조표에 직접적인 스트레스를 가할 수 있다. (Berrospide et al. 2025)
- **데이터 불투명성**: 보유 자산, 가치평가 방법, 부채 구조에 대한 조화된 공시 기준 부재.

## 관련 개념

- [[concepts/private-credit]] — 상위 개념: BDC가 참여하는 자산 클래스
- [[concepts/private-credit-etf]] — 2025년 등장한 대안적 리테일 접근 수단
- [[concepts/procyclical-leverage]] — BDC 레버리지의 핵심 특성
- [[concepts/liquidity-mismatch]] — BDC는 폐쇄형으로 유동성 불일치 없으나, ETF와 비교 맥락에서 중요
- [[concepts/rollover-risk]] — 은행 신용한도(변동금리, 단기) 의존에서 비롯된 자금조달 리스크

## 출처

- [[summaries/bisbull106]] — BIS Bulletin No. 106 (2025년 7월): BDC 구조, 레버리지 추이, 은행-NBFI 연계 분석
- [[summaries/kcif-private-credit-market-overview-260203]] — KCIF 2026-02-03: 반유동적 BDC 환매 급증 사례, NAV 하락 데이터
