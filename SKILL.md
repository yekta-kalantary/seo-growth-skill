---
name: seo-growth
description: Use when a user needs SEO research, an SEO audit, keyword or competitor analysis, content strategy or briefs, topic clusters, internal linking, technical/on-page/local/ecommerce/international/programmatic SEO, schema, backlinks, CRO for organic landing pages, or visibility in AI answers such as AI Overviews, ChatGPT, and Perplexity.
license: MIT
metadata:
  version: "1.0.0"
  category: "seo"
---

# SEO Growth

## Compatibility

This skill targets GPT in ChatGPT Work and Codex only. Use their native skills, web access, connected apps, and workspace file tools. It has no runtime dependency on Claude Code, Claude plugins, external agent runners, slash commands, hooks, or third-party SEO APIs.

## Purpose

Turn an SEO or organic-growth question into an evidence-backed diagnosis and a prioritized, usable deliverable. Scope the work before loading detailed guidance.

## Route the Request

Read only the references needed for the request:

| Request | Required reference |
|---|---|
| Keyword research, intent, SERP or competitor analysis | [research.md](references/research.md) |
| Content strategy, brief, creation, refresh or cannibalization | [content.md](references/content.md) |
| Topic clusters, taxonomy, site architecture or internal links | [architecture.md](references/architecture.md) |
| Full-site or single-page audit, indexing, CWV, schema, international SEO | [technical.md](references/technical.md) |
| Backlinks, digital PR, authority or reputation | [authority.md](references/authority.md) |
| Ecommerce, local or programmatic SEO | [specialized.md](references/specialized.md) |
| GEO, AEO, LLMO, AI citations or AI visibility | [ai-search.md](references/ai-search.md) |
| Organic landing-page CRO, measurement or experiment design | [measurement-cro.md](references/measurement-cro.md) |

For multi-part requests, load the smallest combination that covers the requested outcome.

## Shared Workflow

1. Define the decision the user needs to make, the market/language/locale, target site or page, audience, and available data. Ask only for missing information that materially changes the result.
2. Inspect user-provided files and connected first-party data before public research. When a URL or current SERP is involved, browse rather than relying on memory.
3. State scope and limitations. Distinguish what was observed directly, supplied by the user, inferred, or not measurable with available access.
4. Analyze using the relevant reference. Do not apply every checklist to every task.
5. Deliver the requested artifact first, followed by evidence and a prioritized action plan when useful.

## Evidence Contract

- Never invent rankings, traffic, conversions, search volume, keyword difficulty, backlinks, authority scores, index coverage, Core Web Vitals, or competitor behavior.
- Verify current search features, search-engine documentation, structured-data eligibility, platform policies, and numerical benchmarks on the web. Prefer Google, Bing, Schema.org, W3C/Web.dev, and other primary sources for technical claims.
- Treat SEO-tool scores, correlation studies, and practitioner surveys as third-party observations, not causal facts.
- A static fetch may miss JavaScript-rendered content and injected JSON-LD. Use a rendered browser or user-supplied crawl when that distinction matters.
- Do not infer sitewide conditions from a single URL. Name the sample and confidence level.
- Recommendations must connect to a finding, expected outcome, and verification method.

## Prioritization

Use these fields when reporting multiple findings:

| Field | Values |
|---|---|
| Impact | Critical, High, Medium, Low |
| Confidence | Confirmed, Strong inference, Hypothesis |
| Effort | Small, Medium, Large |
| Owner | Content, SEO, Engineering, Design, Analytics, Outreach |
| Validation | Exact check or KPI used after implementation |

Order work by blockers first, then high-impact/high-confidence improvements, quick wins, and longer experiments.

## Output Standard

Match the requested format. A default audit or strategy output contains:

1. Executive verdict
2. Scope, inputs, and limitations
3. Findings with evidence
4. Prioritized actions with owner and validation
5. Deliverable-specific tables, copy, code, or brief

Do not pad the answer with generic SEO education. Preserve the user's language and business context.

## Sources

This skill is a GPT/Codex-native synthesis of two MIT-licensed projects. Read [sources.md](references/sources.md) when updating or redistributing it. Read [maintenance.md](references/maintenance.md) before incorporating upstream changes.
