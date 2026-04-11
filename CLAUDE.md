# Global Capital Flow Knowledge Base — Schema

## Purpose

This is an LLM-maintained knowledge base on global capital flow research and analysis. 글로벌 자본의 이동 패턴, 거시경제 요인, 주요 시장 참여자, 정책 변수 간의 관계를 체계적으로 정리하고 분석한다. The LLM writes and maintains all files under `wiki/`. The human curates raw sources and directs queries. The human never edits wiki files directly.

## Directory Layout

- `raw/` — Immutable source documents (transcripts, articles, notes). Never modify these.
- `wiki/index.md` — Master catalog. Every wiki page must appear here.
- `wiki/log.md` — Append-only activity log.
- `wiki/summaries/` — One summary page per raw source document.
- `wiki/concepts/` — Concept, strategy, and framework pages.
- `wiki/entities/` — Entity pages (people, tools, organizations, products — whatever "things" exist in your domain).
- `wiki/syntheses/` — Comparison tables, decision frameworks, cross-cutting analyses.
- `wiki/journal/` — Research or session journal entries.
- `wiki/presentations/` — Marp slide decks generated from wiki content.

## File Naming

- All lowercase, hyphens for word separation: `concept-name.md`
- No spaces, no special characters, no uppercase
- Name should match the page title slug

## Page Format

Every wiki page uses this frontmatter and structure:

```yaml
---
title: "Page Title"
type: concept | entity | summary | synthesis
tags: [tag1, tag2, tag3]
created: YYYY-MM-DD
updated: YYYY-MM-DD
sources: ["raw/filename.txt"]
confidence: high | medium | low
---
```

### Required Sections by Page Type

**Summary pages** (`wiki/summaries/`):
- `## Key Points` — Bulleted list of main claims/ideas
- `## Relevant Concepts` — Links to concept pages this source touches
- `## Source Metadata` — Type of source, author/speaker, date, URL or identifier

**Concept pages** (`wiki/concepts/`):
- `## Definition` — One-paragraph plain-English definition
- `## How It Works` — Mechanics, process, or structure of the concept
- `## Key Parameters` — Important variables, dimensions, or factors
- `## When To Use` — Situations and contexts where this concept applies
- `## Risks & Pitfalls` — Known failure modes, common mistakes, limitations
- `## Related Concepts` — Wiki links to related pages
- `## Sources` — Which raw sources inform this page

**Entity pages** (`wiki/entities/`):

Entity는 sub-type에 따라 frontmatter의 `type` 필드를 세분화하고, 아래 섹션 구조를 따른다.

*Sub-type: `central-bank`* (예: Fed, ECB, BOJ, BOK, PBoC)
- `## Overview` — 설립 목적, 관할 통화·경제권
- `## Policy Stance` — 현재 금리 수준, QE/QT 상태, 포워드 가이던스
- `## Key Tools` — 사용 가능한 정책 수단 (금리, 자산매입, FX 개입 등)
- `## Historical Interventions` — 주요 정책 전환 이력 및 자본흐름 영향
- `## Related Entities` — 연관 중앙은행, 재무부, 국제기구

*Sub-type: `country-economy`* (예: 미국, 중국, 한국, 신흥국)
- `## Overview` — 경제 규모, 주요 산업, 글로벌 위상
- `## Capital Account Profile` — 자본계정 개방도, FX 레짐, 외환보유액
- `## Flow Drivers` — 자본 유출입을 결정하는 구조적·사이클적 요인
- `## Key Indicators` — 경상수지, GDP 성장률, 물가, 정책금리
- `## Related Entities` — 연관 중앙은행, 주요 교역국, 국제기구

*Sub-type: `market-participant`* (예: SWF, 헤지펀드, 연기금, 보험사)
- `## Overview` — 기관 성격, 설립 배경, 운용 규모(AUM)
- `## Investment Mandate` — 운용 목표, 자산배분 원칙, 투자 제약
- `## Typical Flow Behavior` — 리스크 온/오프 시 행동 패턴, 리밸런싱 주기
- `## Home Bias & Allocation` — 국내외 자산 배분 비중 및 변화 추이
- `## Related Entities` — 연관 기관, 규제기관, 주요 투자 대상국

**Synthesis pages** (`wiki/syntheses/`):
- `## Comparison` — Table or structured comparison
- `## Analysis` — Cross-cutting insights
- `## Recommendations` — When to prefer which approach
- `## Pages Compared` — Links to all pages involved

## Linking Conventions

- Use Obsidian-style wiki links: `[[concepts/concept-name]]`
- Always use relative paths from wiki root
- Every page must link to at least one other page (no orphans)
- When mentioning a concept that has a page, always link it

## Tagging Taxonomy

- **Asset Class**: `equities`, `bonds`, `fx`, `commodities`, `real-estate`, `private-equity`, `crypto`
- **Flow Type**: `portfolio-flow`, `fdi`, `carry-trade`, `hot-money`, `repatriation`, `deleveraging`
- **Geography**: `us`, `china`, `europe`, `japan`, `korea`, `emerging-markets`, `developed-markets`, `latam`, `asia`
- **Macro Factor**: `interest-rate`, `inflation`, `dollar-cycle`, `risk-appetite`, `liquidity`, `central-bank`, `sanctions`
- **Analysis Type**: `quantitative`, `qualitative`, `structural`, `cyclical`
- **Scope**: `foundational`, `advanced`, `experimental`
- **Status**: `well-established`, `emerging`, `speculative`

## Confidence Levels

- **high** — Well-established idea, multiple corroborating sources, demonstrated with concrete examples
- **medium** — Supported by sources but limited examples or single-source
- **low** — Single mention, anecdotal, or speculative

## Trusted Data Sources

아래 출처에서 인용된 클레임은 confidence를 한 단계 올려서 적용한다.

- **KCIF** (국제금융연구센터) — 한국 관점의 국제금융 분석, 자본흐름 보고서
- **BOK** (한국은행) — 국제수지, 외환보유액, 금융안정 데이터
- **FRB** (Federal Reserve Board) — 미국 금융시스템, Z.1 Financial Accounts, 통화정책 보고서
- **Fed** (Federal Reserve) — FOMC 성명, 의사록, 경제전망(SEP)
- **BIS** — 국제결제은행, 글로벌 자본흐름·외환·파생상품 통계
- **IMF** — 국제수지(BOPS), World Economic Outlook, GFSR
- **EPFR Global** — 펀드 플로우 데이터 (주식·채권 자금 이동)
- **US TIC** — 미국 재무부 국제 자본 흐름 데이터
- **World Bank** — 장기 FDI, 송금(remittance) 데이터

## Workflows

### Ingest

When the user says "ingest [source]" or adds a file to `raw/`:

1. Read the raw source completely
2. Create `wiki/summaries/<source-slug>.md` with full summary
3. Identify all concepts, entities, and strategies mentioned
4. For each concept/entity: create the page if it doesn't exist, or update it with new information if it does
5. Add cross-links in both directions between all touched pages
6. Update `wiki/index.md` — add new entries, update summaries of changed pages
7. Append to `wiki/log.md` with timestamp, source name, pages created/updated
8. Flag any contradictions with existing wiki content

### Query

When the user asks a question:

1. Read `wiki/index.md` to find relevant pages
2. Read those pages
3. Synthesize an answer citing specific pages with wiki links
4. If the answer reveals new insight worth preserving:
   - Create a synthesis page in `wiki/syntheses/`
   - Update index and log

### Lint

When the user says "lint" or "health check":

1. Read all wiki pages
2. Check for: orphan pages (no inbound links), stale claims, contradictions between pages, missing cross-links, incomplete sections, low-confidence pages that could be strengthened
3. Fix what can be fixed automatically
4. Report issues that need human judgment
5. Suggest new sources or topics to investigate
6. Update log

## Rules

- Never modify files in `raw/`
- Always update `index.md` and `log.md` after any wiki change
- Prefer updating existing pages over creating duplicates
- When in doubt about a claim, set confidence to "low" and note the uncertainty
- Keep pages focused — one concept per page, split if a page gets too long
- Use plain English — define jargon on first use in each page
- All dates in ISO 8601 format: YYYY-MM-DD
- When a source provides specific examples, include them with concrete details
