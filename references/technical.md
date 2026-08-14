# Technical and On-Page SEO

Use for site audits, single-page reviews, indexation, crawling, rendering, performance, schema, sitemaps, migrations, and international SEO.

## Audit Order

1. Access and rendering: status codes, robots controls, authentication/CDN blocks, JavaScript dependencies
2. Indexability: robots meta/header, canonical, duplicates, soft 404s, redirects, index status evidence
3. Discovery: internal links, sitemaps, navigation, orphan pages, crawl traps
4. Page signals: title, main heading, content/intent alignment, media, internal/external links
5. Experience: field Core Web Vitals when available, then lab diagnostics
6. Structured data and international annotations

## Evidence Collection

Record URL, timestamp, method, status, final URL, canonical, robots directives, rendered/static distinction, and sample size. Search Console exports, server logs, crawls, analytics, and field performance data are stronger for sitewide conclusions than isolated fetches.

Do not report absent schema from a text-only fetch when scripts were stripped. Render the page or inspect raw HTML/JSON-LD. Validate syntax and eligibility separately; valid schema does not guarantee a rich result.

## On-Page Review

Check uniqueness and intent alignment of title/H1, descriptive hierarchy, substantive main content, media alternatives, canonical/robots consistency, sharing metadata when useful, and contextual links. Character counts are display heuristics, not quality rules; preview likely truncation rather than declaring a fixed pass/fail.

## Performance

Prefer field data for LCP, INP, and CLS. Use lab tools to diagnose likely causes: server latency, render-blocking resources, oversized media, long main-thread tasks, third-party scripts, missing dimensions, and late content injection. Verify current thresholds from Web.dev or Search Console before quoting them.

## International SEO

- Each language/region URL normally self-canonicalizes.
- Hreflang sets require valid codes, reciprocal relationships, and indexable canonical targets; include `x-default` when a genuine fallback exists.
- Do not use IP or language-based redirects that prevent crawling alternatives.
- Translate the substantive page, not only interface chrome.
- Keep canonical, hreflang, sitemap, protocol, host, and URL formats consistent.

## Schema

Choose types supported by actual visible content and current search-engine eligibility. Produce JSON-LD only after required facts are known. Never invent ratings, prices, availability, authors, addresses, dates, or FAQs. Validate with Schema.org tooling and the relevant search-engine rich-result test.

## Finding Format

For every issue: evidence, affected scope, impact, confidence, fix, owner, effort, and exact validation. Separate confirmed blockers from hypotheses requiring crawl, log, browser, Search Console, or CMS access.
