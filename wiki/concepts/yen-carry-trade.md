---
title: "엔 캐리 트레이드 (Yen Carry Trade)"
type: concept
tags: [carry-trade, fx, japan, interest-rate, risk-appetite, portfolio-flow, dollar-cycle, well-established]
created: 2026-04-17
updated: 2026-04-18
sources: ["raw/20240417_B_20210092_852.pdf", "raw/Japan_FX_Capitulation_of_JPY_carry_Only_the_beginning_of_the_end-Japan_FX.pdf", "raw/24809_Significant position unwinding, and what is USDJPYs next move_nomura.pdf", "raw/240829_엔 캐리 트레이드가 실제로 무엇인지에 대해 말하다_신현송박사_원본.pdf", "raw/240816_How can we estimate the size of yen carry trade positions from existing statistics_Nomura.pdf"]
confidence: high
---

## Definition

엔 캐리 트레이드란 저금리 통화인 일본 엔화를 차입(또는 매도)하여 금리가 높은 국가의 자산에 투자함으로써 금리 차이와 환율 변동에서 수익을 추구하는 거래다. 일본은행(BOJ)의 장기 완화 정책으로 엔화가 글로벌 신용 공급 통화(funding currency)로 자리잡았으며, 1990년대 중반부터 본격화됐다.

## How It Works

### FX 스왑을 통한 오프밸런스시트 캐리 메커니즘

[[entities/hyun-song-shin]](BIS, 2024-08-29)은 캐리 트레이드의 주된 실행 경로가 온밸런스시트 차입이 아닌 **FX 스왑 시장**임을 강조:

- 정상적 FX 스왑: 달러를 제공하고 엔화를 수취, 만기에 역방향 정산 → 헤징 목적
- **캐리 전용**: 스왑으로 수취한 엔화를 안전 자산에 보관하지 않고 현물 시장에서 매도 → **무담보 엔화 부채(naked yen obligation)** 발생 → 이것이 오프밸런스시트 캐리 포지션
- 결과적으로 회계상 "차입"이 아니지만 경제적 실질은 엔화를 빌려 달러 자산에 투자하는 것과 동일
- FX 스왑이 통화 간 자금을 대체 가능하게 만들기 때문에, 조달 통화와 투자 통화의 국가 제약이 사라짐

### 수익 구조 (고전적)
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
| **CFTC 비상업적 JPY 선물 순포지션** | 오프밸런스 캐리 최실용 프록시 — 주간 업데이트, 단기 예측에 가장 적합. Aug 6 ≈ $1bn(≈0) |
| **BOJ 인터오피스 대출 ($68bn, May-24)** | 온밸런스 캐리 하단 추정 — 월간, 캐리 외 일반 플로우 포함. GFC 피크 대비 낮음 |
| **BIS 엔화 크로스보더 대출 ($271bn, Mar-24)** | 온밸런스 캐리 상단(최대값) 추정 — 분기, M&A 대출 포함. 신현송 X 포스트: "최대 추정치". GFC 피크 상회 |
| **엔/기타통화 FX 스왑 잔액 (~$14조)** | 오프밸런스 캐리 규모 — 온밸런스의 52배. 실질 캐리의 주된 경로 (신현송·BIS) |
| 달러-엔 FX 스왑 베이시스 | 캐리 방향 탐지: 거의 변동 없으면 달러 쟁탈이 아닌 엔화 반제 동인 시사 |
| JP Morgan Global FX Volatility Index | 환 변동성 모니터링 |
| Barclays/JP Morgan 캐리 트레이드 지수 | 성과 측정 |

**주요 조달 통화(funding currency)**: 엔화, 달러, 스위스 프랑
**주요 투자 통화(target currency)**: 호주 달러, 뉴질랜드 달러, 신흥국 통화, 고금리 국면의 달러·유로
**클래식 캐리 목적지 통화 (2024년 8월 실증)**: 멕시코 페소, 콜롬비아 페소, 남아프리카공화국 랜드 — 2024년 8월 초 가장 크게 하락함으로써 클래식 캐리 청산의 증거로 확인됨 (신현송, BIS)

## 3종 프록시 체계 — 온/오프밸런스 비교

Nomura(2024-08-16)는 진정한 캐리 포지션 규모를 실시간으로 파악하는 것은 불가능하다고 전제하고, 현존 통계에서 추론할 수 있는 세 가지 대체 지표를 제시:

| 출처 | 데이터 | 커버리지 | 최신 값 | 주기 | 특성 |
|------|--------|---------|--------|------|------|
| BOJ | 일본 소재 외국계 은행 인터오피스 대출 | 온밸런스 | $68bn (May-24) | 월간 | 하단 추정. 비캐리 플로우 혼재. GFC 피크 하회 |
| BIS | 비거주 비은행 섹터 엔화 크로스보더 대출 | 온밸런스 | $271bn (Mar-24) | 분기 | 상단(최대) 추정. GFC 피크 상회. M&A 대출 포함 |
| CFTC | 비상업적 트레이더 통화 선물 순매도 | 오프밸런스 | ~$1bn (Aug-6) | 주간 | 단기 예측에 가장 실용적. 리얼머니·기업 미포함 |

**GFC 이후 온밸런스 → 오프밸런스 구조 전환**:
- 국제 은행 레버리지 비율 규제(GFC 이후 도입)로 은행의 온밸런스시트 확대 비용 증가
- 결과: 직접 엔화 차입(온밸런스) 대신 선물/파생상품(오프밸런스) 캐리 포지션이 주류가 됨
- CFTC 주간 데이터가 실용적 추적 도구로 부상한 구조적 이유

**데이터 공백**: 2024년 8월 청산 규모를 BIS 데이터로 확인하려면 2024년 6월 말 데이터(9월 16일 발표) 이후 12월까지 대기 필요.

## 우리다시 채권 — 일본 개인투자자 캐리 채널

우리다시(Uridashi) 채권은 일본 국내에서 일본 개인투자자에게 발행하는 **외화 표시 채권**으로, Mrs. Watanabe 단위 캐리 트레이드의 핵심 수단이다.

- **발행 통화**: AUD, NZD, USD, TRY, BRL, MXN, ZAR — 고금리 통화 중심
- **캐리 메커니즘**: 엔화로 매입 → 고금리 외화 표시 이자 수취 + 환차익(엔화 약세 시) 추구
- **2010년대 후반 구조 변화**: G10(AUD·NZD) 비중 감소 → EM(TRY·BRL·MXN·ZAR) 비중 증가로 캐리 성격 강화
- **2024년 청산 연관**: MXN/JPY TFX 포지션이 ¥121.5bn(7/30) → ¥45.4bn(8/6)으로 급감 — 우리다시·개인 FX 양 경로로 MXN 캐리 청산 동시 진행

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

## 2024년 8월 청산 사례: Citi vs. Nomura 관점 비교

### Citi Research (2024-08-05) 관찰

Citi Research는 2024년 8월 USDJPY ¥20 급락을 분석하며 다음 사항을 확인:
- **포지션 규모**: CitiFX Position Index 기준, 레버리지 투자자뿐 아니라 리얼머니(장기) 투자자 및 기업 섹터까지 대규모 JPY 숏 포지션 누적 (2021년 6월 이후 누적)
- **반등 억제 요인**: NISA 해외 투자 지속, 일본 SME의 USD 헤지 재구축, 일본 기업 크로스보더 M&A 증가 → 단기 JPY 매도 압력 지속
- **조기 청산 요인**: [[concepts/carry-vol-ratio]]가 40% 미만에 도달하기 전에 일본 재무성의 FX 개입 누적 효과로 청산 전환점이 앞당겨짐
- **Citi USDJPY 전망**: ¥145/$(2025) → ¥129/$(2026) → ¥116/$(2027)

### Nomura (2024-08-09) 관찰

Nomura는 동일 이벤트를 CFTC 투기적 포지션 데이터 기반으로 분석:
- **JPY 숏 약 80% 청산 완료**: H1 2024 기간 구축된 포지션의 대부분이 이미 정리됨 → 추가 급격한 엔화 강세 압력 제한적
- **NISA 자금 흐름 약화**: 2024년 7월 말부터 상위 10개 해외 주식 투신 순유입 감소 확인. H2 2024의 JPY 매도 압력은 H1 대비 구조적으로 약화
- **여름 계절성**: 도쿄 USD/JPY 일평균 거래량이 7~8월에 구조적으로 감소 → 충격 증폭 메커니즘
- **GPIF 리밸런싱 방향**: [[entities/gpif]] 포트폴리오 해외주식 비중 저하 → 약 ¥5조엔 규모 해외주식 매수(JPY 매도) 리밸런싱 가능성으로 오히려 단기 엔화 약세 압력
- **Nomura USDJPY 전망**: Q3 2024 = ¥143, Q4 2024 = ¥148, Q1 2025 = ¥146, Q4 2025 = ¥140

> ⚠️ **Citi vs. Nomura 모순**: Citi는 리얼머니·기업 포지션까지 포함해 "다년간 청산 사이클 초입"으로 평가한 반면, Nomura는 CFTC 투기적 포지션 기준 80% 청산 완료로 추가 급등 제한적으로 판단. 측정 대상의 차이(투기적 vs. 전체 포지션)가 결론 차이를 만든 것으로 보임.

## Related Concepts

- [[concepts/carry-trade-unwind]] — 청산 메커니즘·5차 역사 케이스
- [[concepts/carry-vol-ratio]] — 청산 임계값 모니터링 핵심 지표
- [[concepts/fx-hedging]] — 환율 리스크 관리
- [[concepts/dollar-cycle]] — 달러 사이클과 엔화 방향성
- [[concepts/crowded-trade]] — 대규모 누적 포지션의 집중 리스크
- [[concepts/risk-appetite]] — 위험선호 전환이 캐리 청산 촉매
- [[concepts/cross-currency-basis]] — 통화 간 자금 조달 비용

## Sources

- `raw/20240417_B_20210092_852.pdf` — 교보증권 리서치센터, 2024-04-17
- `raw/Japan_FX_Capitulation_of_JPY_carry_Only_the_beginning_of_the_end-Japan_FX.pdf` — Citi Research (Osamu Takashima 외), 2024-08-05
- `raw/24809_Significant position unwinding, and what is USDJPYs next move_nomura.pdf` — Nomura Securities (Yujiro Goto 외), 2024-08-09: **CFTC 기준 JPY 숏 80% 청산, NISA 자금 약화, GPIF 리밸런싱 방향, Citi 전망 대비 덜 강세적 엔화 시나리오**
- `raw/240829_엔 캐리 트레이드가 실제로 무엇인지에 대해 말하다_신현송박사_원본.pdf` — BIS 신현송 박사 (Bloomberg Odd Lots 인터뷰), 2024-08-29: **FX 스왑을 통한 오프밸런스시트 캐리 메커니즘, BIS 규모 추정($270bn vs $14조), 클래식 캐리 목적지 통화(MXN·COP·ZAR) 실증**
- `raw/240816_How can we estimate the size of yen carry trade positions from existing statistics_Nomura.pdf` — Nomura Securities (Yujiro Goto 외), 2024-08-16: **BOJ/BIS/CFTC 3종 프록시 체계, CFTC Aug 6 ≈ 0 확인, 온→오프밸런스 구조 전환 이유(레버리지 규제), 우리다시 채권 데이터, MOF 주간 플로우(Aug 4-10)**
