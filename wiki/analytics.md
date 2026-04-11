---
title: "Analytics"
type: dashboard
tags: [meta]
updated: 2026-04-11
---

# Analytics

Dataview 플러그인을 통해 wiki 페이지를 실시간으로 집계합니다.

---

## 페이지 현황 요약

```dataviewjs
const pages = dv.pages('"wiki"').where(p =>
  p.type && !["index", "log", "dashboard"].includes(p.type)
);

const concepts   = pages.where(p => p.type === "concept").length;
const entities   = pages.where(p => p.type === "entity").length;
const summaries  = pages.where(p => p.type === "summary").length;
const syntheses  = pages.where(p => p.type === "synthesis").length;
const total      = concepts + entities + summaries + syntheses;

const high   = pages.where(p => p.confidence === "high").length;
const medium = pages.where(p => p.confidence === "medium").length;
const low    = pages.where(p => p.confidence === "low").length;

const sources = pages.where(p => p.type === "summary").length;

dv.paragraph(`
| 항목 | 수치 |
|------|------|
| 📄 총 페이지 | **${total}** |
| 🧠 개념 | ${concepts} |
| 🏢 엔티티 | ${entities} |
| 📰 요약 | ${summaries} |
| 🔗 분석 종합 | ${syntheses} |
| ✅ 신뢰도 high | ${high} |
| 🟡 신뢰도 medium | ${medium} |
| 🔴 신뢰도 low | ${low} |
| 📥 인제스트된 출처 | ${sources} |
`);
```

---

## 개념 페이지 목록

```dataview
TABLE confidence, tags, updated AS "업데이트"
FROM "wiki/concepts"
SORT file.name ASC
```

---

## 엔티티 페이지 목록

```dataview
TABLE confidence, tags, updated AS "업데이트"
FROM "wiki/entities"
SORT file.name ASC
```

---

## 요약 페이지 목록

```dataview
TABLE sources, updated AS "업데이트"
FROM "wiki/summaries"
SORT updated DESC
```

---

## 태그 빈도

```dataviewjs
const pages = dv.pages('"wiki"').where(p =>
  p.type && !["index", "log", "dashboard"].includes(p.type)
);

const tagCount = {};
for (const page of pages) {
  const tags = page.tags ?? [];
  for (const tag of tags) {
    tagCount[tag] = (tagCount[tag] ?? 0) + 1;
  }
}

const sorted = Object.entries(tagCount)
  .sort((a, b) => b[1] - a[1])
  .slice(0, 15);

const rows = sorted.map(([tag, count]) => {
  const bar = "█".repeat(count) + "░".repeat(Math.max(0, 12 - count));
  return [tag, bar, count];
});

dv.table(["태그", "빈도", "수"], rows);
```

---

## 신뢰도가 낮은 페이지 (요주의)

```dataview
TABLE type, confidence, updated AS "업데이트"
FROM "wiki"
WHERE confidence != "high" AND type AND type != "index" AND type != "log" AND type != "dashboard"
SORT confidence ASC
```
