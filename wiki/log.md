---
title: "Activity Log"
type: log
---

# Activity Log

Append-only record of all wiki changes.

## Format

Each entry follows this format:
```
### YYYY-MM-DD HH:MM — [Action Type]
- **Source/Trigger**: what initiated the action
- **Pages created**: list of new pages
- **Pages updated**: list of updated pages
- **Notes**: any contradictions flagged, decisions made
```

---

### 2026-04-28 — Ingest: raw/bisbull90.pdf

- **Source/Trigger**: 사용자 명령 `ingest https://www.bis.org/publ/bisbull90.pdf`
- **출처**: BIS Bulletin No. 90, Matteo Aquilina·Marco Lombardi·Andreas Schrimpf·Vladyslav Sushko, 2024-08-27
- **Pages created**:
  - `wiki/summaries/bisbull90.md` — 2024년 8월 시장 격변과 캐리 청산 요약
- **Pages updated**:
  - `wiki/concepts/yen-carry-trade.md` — BIS 5단계 규모 추정 방법론(¥2조~¥80조+), 캐리-리스크 비율 데이터 추가
  - `wiki/concepts/carry-trade-unwind.md` — 6차 청산(2024년 8월) 케이스 추가: TOPIX -12%, VIX 60+, 통화별 절상·절하, CCP 증거금, 모멘텀 전략 기여
  - `wiki/concepts/procyclical-leverage.md` — 2024년 8월 VIX 초과 스파이크, JSCC 증거금 60~80% 인상 실증 추가
  - `wiki/entities/boj.md` — 2024년 7월 금리 인상(매파) 및 FX 개입 루머가 촉발 요인임을 Historical Interventions에 추가
  - `wiki/index.md` — 신규 요약 등록, 통계 업데이트
- **Notes**:
  - 2026-04-17 교보증권 리포트는 "완만한 청산" 전망을 제시했으나, 실제 2024년 8월은 단기간 급진적 특성을 보임 — 두 소스 간 결과 불일치. carry-trade-unwind 페이지에 6차 케이스로 명시.
  - BIS는 ¥40조($2,500억)를 "하향 편의가 있는 중간 추정치"로 제시. 교보증권 리포트에서 인용하는 규모 추정치($200~300억)와 차원이 다름 — 측정 대상(선물 vs. OTC+대출 전체)이 다르기 때문.
  - 오프쇼어 위안화(CNH) 절상이 이례적 사례로 언급됨 — 중국 자본흐름과의 연계 가능성. 향후 별도 탐구 고려.
  - BIS 직접 출처이므로 confidence: high 적용.

---

### 2026-04-17 — Ingest: raw/20240417_B_20210092_852.pdf

- **Source/Trigger**: 사용자 명령 `ingest 20240417_B_20210092_852.pdf`
- **출처**: 교보증권 리서치센터, 2024-04-17, 75페이지 프레젠테이션
- **Pages created**:
  - `wiki/summaries/kyobo-yen-carry-unwind-240417.md` — 요약 페이지
  - `wiki/concepts/yen-carry-trade.md` — 엔 캐리 트레이드 개념 (신규)
  - `wiki/concepts/carry-trade-unwind.md` — 캐리 트레이드 청산 개념·5차 역사 케이스 (신규)
  - `wiki/entities/boj.md` — 일본은행(BOJ) 엔티티 (신규)
- **Pages updated**:
  - `wiki/index.md` — 신규 페이지 4개 등록, 통계 업데이트
- **Notes**:
  - 기존 wiki에 캐리 트레이드 관련 개념 및 BOJ 엔티티 부재. 모두 신규 생성
  - 교보증권은 Trusted Data Source 목록에 없으나, Bloomberg·CEIC·BOJ·IMF 등 신뢰 데이터 출처를 직접 인용하고 있어 confidence: high 부여
  - 2024년 4월 시점 전망이므로 이후 실제 청산 전개(2024년 8월 급격한 엔화 강세 등)와 비교 검토 필요

---

### 2026-04-12 — Ingest: raw/비은행 금융중개의 취약성과 시스템 리스크 관리 방안.md

- **Source/Trigger**: 사용자 명령 `ingest @raw/비은행 금융중개의 취약성과 시스템 리스크 관리 방안.md`
- **출처**: IMF GFSR(2024년 10월·2025년 10월) 및 ECB NBFI 분석 보고서 종합 정리
- **Pages created**:
  - `wiki/summaries/nbfi-systemic-risk.md` — 요약 페이지
  - `wiki/concepts/nbfi.md` — 비은행 금융중개기관(NBFI) 개념 (신규)
  - `wiki/concepts/macro-market-divergence.md` — 거시-시장 괴리 개념 (신규)
  - `wiki/concepts/monetary-policy-transmission.md` — 통화정책 전파 경로 개념 (신규)
  - `wiki/entities/imf.md` — IMF 엔티티 (신뢰 출처 등재, 신규)
  - `wiki/entities/ecb.md` — ECB 엔티티 (신규)
- **Pages updated**:
  - `wiki/concepts/procyclical-leverage.md` — 숨겨진 레버리지(OTC 파생상품) 섹션 추가
  - `wiki/concepts/liquidity-mismatch.md` — LMT(유동성 관리 도구) 선제적 확보 필요성 추가
  - `wiki/index.md` (통계 및 목록 업데이트)
- **Notes**:
  - 핵심 수치: 유로존 NBFI GDP 대비 380%, 미국 330%. 전 세계 금융자산의 50%가 NBFI.
  - 거시-시장 괴리(Macro-Market Divergence)는 IMF의 핵심 경고 프레임워크 — 기존 위키에 없던 신규 개념.
  - NBFI 페이지는 bisbull106에서 BDC·프라이빗 크레딧 맥락으로 이미 등장했으나, 이번에 전용 개념 페이지 신설.
  - ECB·IMF를 신뢰 출처로 등재 → 향후 해당 기관 인용 클레임에 confidence 상향 적용.
  - 모순 없음. 기존 NBFI 관련 페이지(procyclical-leverage, liquidity-mismatch, private-credit)와 일관성 유지.

---

### 2026-04-12 — Ingest: raw/헤지펀드 산업 분석 및 시장 역학 브리핑 보고서.md

- **Source/Trigger**: 사용자 명령 `ingest @raw/헤지펀드 산업 분석 및 시장 역학 브리핑 보고서.md`
- **출처**: Wall Street Prep, 50 South Capital, Khandani & Lo(2007 퀀트 멜트다운 연구) 종합 브리핑
- **Pages created**:
  - `wiki/summaries/hedge-fund-industry-analysis.md` — 요약 페이지
  - `wiki/concepts/hedge-fund.md` — 헤지펀드 구조·전략·수수료·고금리 이점 (신규)
  - `wiki/concepts/quant-meltdown.md` — 2007년 퀀트 멜트다운 (신규)
  - `wiki/concepts/crowded-trade.md` — 과밀 거래(Crowded Trade) (신규)
- **Pages updated**:
  - `wiki/concepts/procyclical-leverage.md` — 퀀트 멜트다운·과밀 거래 연결 추가
  - `wiki/concepts/macro-market-divergence.md` — 과밀 거래·퀀트 멜트다운 연결 추가
  - `wiki/index.md` (통계 및 목록 업데이트)
- **Notes**:
  - 출처가 단일 정리 보고서(Wall Street Prep + 50 South Capital + Khandani & Lo 종합)로, 직접적인 1차 데이터가 아님 → confidence medium 적용.
  - 핵심 수치: HFRI 헤지펀드 연평균 5.9% vs 채권 -1.10% (2019.3 이후), 수수료 전통 2/20→최근 1.5/15.
  - 퀀트 멜트다운은 기존 procyclical-leverage, macro-market-divergence 개념과 연결되는 실증 사례로 양방향 링크 추가.
  - AI 군집 행동(herding)이 새로운 형태의 과밀 거래를 형성할 수 있다는 경고 — nbfi-systemic-risk 보고서의 AI 리스크 경고와 연계.
  - 모순 없음. 기존 NBFI·레버리지 관련 페이지들과 일관성 유지.

---

### 2026-04-12 — Ingest: raw/2026-04-12_report_state-capitalism-financial-repression-napier.md

- **Source/Trigger**: 사용자 명령 — NotebookLM 노트북(9d76d85e-2e62-4efa-8121-a241b044df61) 기반 보고서 정리 및 ingest
- **출처**: 월가아재 YouTube 영상 2편 ("채권은 다 팔아야 합니다" / "미국주식, 앞으로 15년은 지금과 달라질 수 있습니다"), 주요 인물: 러셀 네피어(Russell Napier)
- **Pages created**:
  - `raw/2026-04-12_report_state-capitalism-financial-repression-napier.md` — NotebookLM 정리 보고서 원본
  - `wiki/summaries/state-capitalism-financial-repression-napier.md` — 요약 페이지
  - `wiki/concepts/financial-repression.md` — 금융 억압 개념 (신규)
  - `wiki/concepts/state-capitalism.md` — 국가 자본주의 개념 (신규)
  - `wiki/concepts/capital-nationalism.md` — 자본 민족주의 개념 (신규)
  - `wiki/entities/russell-napier.md` — 러셀 네피어 엔티티 (신규)
- **Pages updated**: `wiki/index.md` (통계 및 목록 업데이트)
- **Notes**:
  - 기존 `entities/gpif`, `entities/japanese-life-insurers` 페이지와 연결 (일본 자본 회수 시나리오)
  - `concepts/dollar-cycle`, `concepts/rollover-risk`와 교차 링크 추가
  - 미국 국가 부채 수치(39조 달러, GDP 122%)는 2026년 3월 기준 — 최신 확인 필요
  - 자본 민족주의 실현 속도는 불확실 — 구조적 방향성 프레임워크로만 활용 권장

---

### 2026-04-12 03:00 — Ingest: raw/2026-02-03_report_private-credit-market-overview.pdf

- **Source/Trigger**: 사용자 명령 `/pdf @raw/2026-02-03_report_private-credit-market-overview.pdf`
- **출처**: KCIF Issue Analysis, "미국 사모대출(private credit) 시장 현황과 위험요인", 김선경·김윤경, 2026년 2월 3일
- **Pages created**:
  - `wiki/summaries/kcif-private-credit-market-overview-260203.md`
  - `wiki/concepts/shadow-default.md` — 그림자 파산 개념 (신규)
  - `wiki/concepts/pik-payment-in-kind.md` — PIK 현물 지급 개념 (신규)
- **Pages updated**:
  - `wiki/concepts/private-credit.md` — 시장 규모·섹터·스프레드 데이터, 그림자 파산·PIK·보험사 연계 리스크 추가
  - `wiki/concepts/business-development-company.md` — 반유동적 BDC 환매 메커니즘 및 2025년 4분기 사례 추가
  - `wiki/index.md`, `wiki/log.md`
- **Notes**:
  - KCIF 신뢰 출처 적용: 모든 클레임 high confidence.
  - 핵심 수치: 글로벌 $2.3조(2025년, Preqin), 미국 70%+, 스프레드 475bp(역사적 저점), 부도율 2.46%(Q4 2025), PIK 비중 10.6% 중 Bad PIK 57.2%.
  - 은행 측: 사모대출 기관 대출 $3,140억 = NBFI 대출의 26%; Fitch 10대 은행 익스포저 자본의 30%.
  - 보험사 측: 생보사 사모대출·PE 보유 $4,604억(2018) → $9,506억(2024); 운용사 계열 생보사 Level III 자산 23.7%.
  - AI 연관: 포트폴리오 25~35%(UBS); Meta·Blue Owl $270억 ABL(부외 부채).
  - 모순 없음. bisbull106(BIS)의 구조적 분석을 KCIF의 시장 데이터와 위험 사례로 구체화함.
  - 핵심 인사이트: 공식 부도율이 낮아 보여도 Bad PIK 비중 급증이 실질 부실 확대를 시사. 서브프라임 유사성 경고(BOE 총재, BofA 설문).

---

### 2026-04-12 02:00 — Synthesis: 아시아 달러 익스포저 전략 비교

- **Source/Trigger**: 사용자 요청 — ingest 후 도출된 인사이트 저장
- **Pages created**: `wiki/syntheses/asia-dollar-exposure-strategies.md`
- **Pages updated**: `wiki/index.md`, `wiki/log.md`
- **Notes**:
  - 핵심 인사이트: 일본·대만은 "달러 자산 축적자"(사후 헤징 위험), 중국은 "달러 자산 매수자"(점진적·구조적). 달러 약세 전환 시 두 그룹이 서로 다른 메커니즘으로 달러 약세를 강화.
  - GPIF는 생보사와 달리 사후 헤징 없이 리밸런싱 경로(채권 시장)로만 작동 — 중요한 구분.
  - 대만의 이중 포지션(사후 헤징 압력 + EM ex-China 수혜) 간 충돌 가능성 첫 명시.

---

### 2026-04-12 01:00 — Ingest: raw/260325-중국+내외국인.pdf

- **Source/Trigger**: 사용자 명령 `ingest raw/260325-중국+내외국인.pdf`
- **출처**: KCIF Issue Analysis, "중국의 내외국인 증권투자 순유출 확대 및 평가", 이은재·신술위, 2026년 3월 25일
- **Pages created**:
  - `wiki/summaries/kcif-china-capital-outflow-260325.md`
  - `wiki/entities/china.md`
  - `wiki/concepts/qdii.md`
  - `wiki/concepts/southbound-trading.md`
  - `wiki/concepts/em-ex-china.md`
- **Pages updated**: `wiki/entities/kcif.md` (새 발간물 추가), `wiki/concepts/dollar-cycle.md` (중국 디커플링 섹션 추가), `wiki/index.md`, `wiki/log.md`
- **Notes**:
  - KCIF 신뢰 출처 적용: 모든 클레임 high confidence.
  - 핵심 수치: 2025년 순유출 3,577억달러(역대 최대), 내국인 해외투자 3,046억달러(역대 최대), 남향자금 HKD 1.4조(최고치), QDII AUM +54%.
  - 모순 없음. 기존 달러 사이클 페이지(bisbull105 기반)에 중국 디커플링 및 위안화 강세 메커니즘을 보완적으로 추가.
  - 새 연결: china → dollar-cycle, rollover-risk(NCD 유출 구조), em-ex-china(한국·대만 수혜 맥락).
  - 주목할 신규 패턴: 중국 본토자금이 홍콩 경유 글로벌 주식 ETF(미국 주식 포함)에 투자하는 우회 경로 확인.

---

### 2026-04-12 00:00 — Ingest: raw/260326-일본+GPIF+포트폴리오+조정+가능성.pdf

- **Source/Trigger**: 사용자 명령 `ingest raw/260326-일본+GPIF+포트폴리오+조정+가능성.pdf`
- **출처**: KCIF Issue Analysis, "일본 GPIF 포트폴리오 조정 가능성 관련 쟁점 점검", 신술위·이은재, 2025년 3월 26일
- **Pages created**:
  - `wiki/summaries/kcif-gpif-portfolio-260326.md`
  - `wiki/entities/gpif.md`
  - `wiki/entities/kcif.md`
- **Pages updated**: `wiki/concepts/hedge-ratio.md` (GPIF 환헤지 비율 1.2% 데이터 추가), `wiki/index.md`, `wiki/log.md`
- **Notes**:
  - KCIF 신뢰 출처 적용: 모든 클레임 high confidence.
  - 핵심 수치: GPIF AUM 293.4조엔, 환헤지 비율 사실상 0%(1.2% → 추가 축소), 해외자산 50.3%(미국 채권 53%, 주식 66%), 목표비중 ±1%p 내 엄격 준수.
  - 기존 `hedge-ratio` 개념 페이지에 GPIF 데이터(일본 생보사 40%와 극명히 대비되는 ~0%) 추가 — 동일 개념을 보강하는 새 증거.
  - 모순 없음. 일본 생보사의 헤지 비율 하락(60→40%)과 GPIF의 구조적 무헤지는 상호 보완적 데이터.
  - 한·미·일 삼각 관계(미 재무부의 GPIF 자금흐름 주시)가 자본흐름 맥락에서 새로운 지정학적 차원을 추가.

---

### 2026-04-11 02:00 — Ingest: raw/bisbull106.pdf

- **Source/Trigger**: 사용자 명령 `ingest raw/bisbull106.pdf`
- **출처**: BIS Bulletin No. 106, "Retail investors in private credit", Aldasoro/Doerr/Todorov, 2025년 7월 9일
- **Pages created**:
  - `wiki/summaries/bisbull106.md`
  - `wiki/concepts/private-credit.md`
  - `wiki/concepts/business-development-company.md`
  - `wiki/concepts/private-credit-etf.md`
  - `wiki/concepts/liquidity-mismatch.md`
  - `wiki/concepts/procyclical-leverage.md`
- **Pages updated**: `wiki/entities/bis.md` (Bulletin No. 106 항목 추가), `wiki/index.md`, `wiki/log.md`
- **Notes**:
  - 기존 위키 내용과 모순 없음. `rollover-risk` 개념이 기존(bisbull105 기반)에 있어 새 출처의 은행-NBFI 연계 맥락으로 연결됨.
  - BIS 신뢰 출처 적용: 주요 수치(AUM 2.2조 달러, BDC D/E 3배 증가, 은행 NBFI 신용공여 2.3조 달러 등) high confidence 처리.
  - `private-credit-etf`는 2025년 초 첫 출시로 스트레스 검증 데이터가 없어 confidence를 medium으로 설정.
  - 핵심 수치: BDC D/E 비율 30%→90%(15년간), 리테일 AUM 비중 0%→13%(280억 달러), 프라이빗 크레딧 ETF 비유동 자산 비중 10~35%, ETF 비용 약 0.7%.

---

### 2026-04-11 01:00 — 한국어 재작성

- **Source/Trigger**: 사용자 요청 — 모든 위키 페이지를 한국어로 재작성
- **Pages created**: 없음
- **Pages updated**: summaries/bisbull105.md, concepts/fx-hedging.md, concepts/ex-post-hedging.md, concepts/cross-currency-basis.md, concepts/hedge-ratio.md, concepts/dollar-cycle.md, concepts/rollover-risk.md, entities/bis.md, entities/japanese-life-insurers.md, entities/taiwanese-life-insurers.md (10개 전체)
- **Notes**: 내용·구조·링크는 그대로 유지; 본문 언어만 영어→한국어로 전환. 향후 모든 위키 작성은 한국어로 진행.

---

### 2026-04-11 00:00 — Ingest: raw/bisbull105.md

- **Source/Trigger**: User command `ingest raw/bisbull105.md`
- **Source**: BIS Bulletin No. 105, "US dollar's slide in April 2025: the role of FX hedging", Shin/Wooldridge/Xia, 20 June 2025
- **Pages created**:
  - `wiki/summaries/bisbull105.md`
  - `wiki/concepts/fx-hedging.md`
  - `wiki/concepts/ex-post-hedging.md`
  - `wiki/concepts/cross-currency-basis.md`
  - `wiki/concepts/hedge-ratio.md`
  - `wiki/concepts/dollar-cycle.md`
  - `wiki/concepts/rollover-risk.md`
  - `wiki/entities/bis.md`
  - `wiki/entities/japanese-life-insurers.md`
  - `wiki/entities/taiwanese-life-insurers.md`
- **Pages updated**: `wiki/index.md`, `wiki/log.md`
- **Notes**:
  - No contradictions with existing wiki content (wiki was empty at time of ingest).
  - BIS is a trusted source per schema; all claims from this bulletin receive elevated confidence (high).
  - Key quantitative claims: Japanese life insurer hedge ratio 60%→40% (2021–2024) per BOJ FSR April 2025; Taiwanese life insurer hedge ratio ~65% near historic lows per BofA Global Research 2025.
  - Intraday FX data and cross-currency basis movements cited as corroborating evidence for ex post hedging thesis (not asset-selling).
  - April 2025 TIC outflow of ~$50bn noted as not exceptional by historical standards.

---

### 2026-04-08 00:00 — Setup

- **Source/Trigger**: Repository initialized
- **Pages created**: index.md, log.md, dashboard.md, analytics.md, flashcards.md
- **Pages updated**: none
- **Notes**: Empty knowledge base ready for first source ingestion
