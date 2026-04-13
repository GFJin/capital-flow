# Graph Report - ./raw  (2026-04-13)

## Corpus Check
- Corpus is ~32,890 words - fits in a single context window. You may not need a graph.

## Summary
- 68 nodes · 74 edges · 8 communities detected
- Extraction: 73% EXTRACTED · 27% INFERRED · 0% AMBIGUOUS · INFERRED: 20 edges (avg confidence: 0.82)
- Token cost: 12,000 input · 4,500 output

## Community Hubs (Navigation)
- [[_COMMUNITY_State Capitalism & Financial Repression|State Capitalism & Financial Repression]]
- [[_COMMUNITY_Carry Trade & NBFI Risk|Carry Trade & NBFI Risk]]
- [[_COMMUNITY_Private Credit Rate Risk|Private Credit Rate Risk]]
- [[_COMMUNITY_FX Hedging & Dollar Dynamics|FX Hedging & Dollar Dynamics]]
- [[_COMMUNITY_Retail Private Credit & BDCs|Retail Private Credit & BDCs]]
- [[_COMMUNITY_Hedge Fund Market Dynamics|Hedge Fund Market Dynamics]]
- [[_COMMUNITY_Geopolitics & Bond Yields|Geopolitics & Bond Yields]]
- [[_COMMUNITY_China Capital Flows|China Capital Flows]]

## God Nodes (most connected - your core abstractions)
1. `Financial Repression (금융 억압)` - 6 edges
2. `Private Credit Interest Rate Risk (사모대출 금리 위험)` - 6 edges
3. `NBFI Growth (비은행 금융중개기관 성장)` - 6 edges
4. `Foreign Currency Swap (외환 스왑)` - 5 edges
5. `Hedge Fund (헤지펀드)` - 5 edges
6. `Capital Nationalism (자본 민족주의)` - 4 edges
7. `Private Credit Market Overview (사모대출 시장 현황)` - 4 edges
8. `FX Hedging and Dollar Slide April 2025 (BIS Bull 105)` - 4 edges
9. `Retail Investors in Private Credit (BIS Bull 106)` - 4 edges
10. `Russell Napier` - 3 edges

## Surprising Connections (you probably didn't know these)
- `China Capital Outflow (중국 자본 유출)` --semantically_similar_to--> `Capital Nationalism (자본 민족주의)`  [INFERRED] [semantically similar]
  raw/260325-중국+내외국인.pdf → raw/2026-04-12_report_state-capitalism-financial-repression-napier.md
- `US Fiscal Debt Burden (미국 재정 부채 부담)` --semantically_similar_to--> `Sovereign Debt Burden (선진국 부채 위기)`  [INFERRED] [semantically similar]
  raw/2026-04-03_article_economy-debt-rate-burden.pdf → raw/2026-04-12_report_state-capitalism-financial-repression-napier.md
- `GPIF Domestic Reallocation Pressure` --semantically_similar_to--> `Capital Nationalism (자본 민족주의)`  [INFERRED] [semantically similar]
  raw/260326-일본+GPIF+포트폴리오+조정+가능성.pdf → raw/2026-04-12_report_state-capitalism-financial-repression-napier.md
- `Trump Pressure on Fed Independence` --semantically_similar_to--> `Central Bank Independence Erosion (중앙은행 독립성 훼손)`  [INFERRED] [semantically similar]
  raw/260317-미국+제도적+리스크+시장영향.pdf → raw/2026-04-12_report_state-capitalism-financial-repression-napier.md
- `FX Swap and Forward Overlay (헷지 오버레이)` --semantically_similar_to--> `FX Hedge (환헷지)`  [INFERRED] [semantically similar]
  raw/bisbull105.pdf → raw/FX Swaps.md

## Hyperedges (group relationships)
- **Financial Repression — Sovereign Debt — Capital Nationalism Nexus** — napier_financial_repression, napier_sovereign_debt_burden, napier_capital_nationalism, napier_negative_real_rates [EXTRACTED 0.95]
- **Private Credit Systemic Risk Cluster** — bloomberg_private_credit_rate_risk, bloomberg_bank_nbfi_linkage, pc_redemption_surge, bisbull106_retail_private_credit, nbfi_report_liquidity_mismatch [INFERRED 0.87]
- **Dollar Dynamics: FX Hedging + Geopolitics + Safe Haven Demand** — bisbull105_fx_hedging_dollar_slide, bisbull105_triple_decline, mideast_safe_haven_dollar, fxswap_fx_hedge [INFERRED 0.82]

## Communities

### Community 0 - "State Capitalism & Financial Repression"
Cohesion: 0.16
Nodes (14): GPIF Domestic Reallocation Pressure, Japan GPIF Portfolio Adjustment (일본 연금 포트폴리오 조정), Capital Nationalism (자본 민족주의), Central Bank Independence Erosion (중앙은행 독립성 훼손), Financial Repression (금융 억압), Gold as Inflation Hedge (금 투자 전략), Negative Real Interest Rates (마이너스 실질 금리), Reshoring / Supply Chain Realignment (리쇼어링) (+6 more)

### Community 1 - "Carry Trade & NBFI Risk"
Cohesion: 0.15
Nodes (13): Carry Trade Conditions (캐리트레이드 여건), Interest Rate Differential (금리차), Low Volatility Environment (저변동성 환경), European Central Bank (ECB), Hidden Leverage (숨겨진 레버리지), IMF Global Financial Stability Report (GFSR), Macro-Market Divergence (거시-시장 괴리), Monetary Policy Transmission via NBFI (통화정책 전파) (+5 more)

### Community 2 - "Private Credit Rate Risk"
Cohesion: 0.2
Nodes (10): Bank-NBFI Interconnection (은행-비은행 연결 고리), PIK Loans (현물상환 대출, Payment-in-Kind), Private Credit Interest Rate Risk (사모대출 금리 위험), Unitranche Loans (유니트랜치 대출), US Fiscal Debt Burden (미국 재정 부채 부담), CDO/CLO Securitization Risk, Subprime Mortgage GFC Comparison (서브프라임 비교), BlackRock / Apollo Private Credit Losses (+2 more)

### Community 3 - "FX Hedging & Dollar Dynamics"
Cohesion: 0.25
Nodes (9): Asian Investors FX Hedging Activity, FX Hedging and Dollar Slide April 2025 (BIS Bull 105), FX Swap and Forward Overlay (헷지 오버레이), US Triple Decline (Equities + Bonds + Dollar), Counterparty Risk in Swaps, Foreign Currency Swap (외환 스왑), FX Hedge (환헷지), SOFR (Secured Overnight Financing Rate) (+1 more)

### Community 4 - "Retail Private Credit & BDCs"
Cohesion: 0.25
Nodes (9): BDC Leverage and Procyclicality, Liquidity Mismatch in Private Credit ETFs, Private Credit ETF (사모대출 ETF), Retail Investors in Private Credit (BIS Bull 106), Business Development Company (BDC, 사업개발회사), Blue Owl Capital (블루아울 캐피탈), Blue Owl OBDC II Redemption Halt (환매 중단), Liquidity Mismatch in Open-End Funds (유동성 불일치) (+1 more)

### Community 5 - "Hedge Fund Market Dynamics"
Cohesion: 0.4
Nodes (6): 60/40 Portfolio (전통 자산배분), Alpha Generation (알파 수익), Crowded Trade (과밀 거래), Hedge Fund (헤지펀드), Khandani & Lo Research (퀀트 멜트다운 연구), Quant Meltdown 2007 (퀀트 멜트다운)

### Community 6 - "Geopolitics & Bond Yields"
Cohesion: 0.5
Nodes (4): Middle East War Oil Price Inflation, Major Country Bond Yield Rise (주요국 국채금리 상승), Middle East War Dollar Scenarios (중동 전쟁 달러 시나리오), Safe Haven Dollar Demand (안전자산 달러 수요)

### Community 7 - "China Capital Flows"
Cohesion: 0.67
Nodes (3): China Capital Outflow (중국 자본 유출), China QDII (적격 국내 기관투자자), Yuan Appreciation (위안화 강세)

## Knowledge Gaps
- **24 isolated node(s):** `Japan Yield Curve Control (YCC)`, `Reshoring / Supply Chain Realignment (리쇼어링)`, `Gold as Inflation Hedge (금 투자 전략)`, `SOFR (Secured Overnight Financing Rate)`, `Counterparty Risk in Swaps` (+19 more)
  These have ≤1 connection - possible missing edges or undocumented components.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Private Credit Interest Rate Risk (사모대출 금리 위험)` connect `Private Credit Rate Risk` to `Retail Private Credit & BDCs`?**
  _High betweenness centrality (0.683) - this node is a cross-community bridge._
- **Why does `US Fiscal Debt Burden (미국 재정 부채 부담)` connect `Private Credit Rate Risk` to `State Capitalism & Financial Repression`, `Geopolitics & Bond Yields`?**
  _High betweenness centrality (0.504) - this node is a cross-community bridge._
- **Why does `NBFI Growth (비은행 금융중개기관 성장)` connect `Carry Trade & NBFI Risk` to `Private Credit Rate Risk`?**
  _High betweenness centrality (0.451) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `Financial Repression (금융 억압)` (e.g. with `GPIF Domestic Reallocation Pressure` and `Major Country Bond Yield Rise (주요국 국채금리 상승)`) actually correct?**
  _`Financial Repression (금융 억압)` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Japan Yield Curve Control (YCC)`, `Reshoring / Supply Chain Realignment (리쇼어링)`, `Gold as Inflation Hedge (금 투자 전략)` to the rest of the system?**
  _24 weakly-connected nodes found - possible documentation gaps or missing edges._