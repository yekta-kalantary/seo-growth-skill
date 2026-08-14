# Site Architecture and Internal Linking

Use for taxonomy, pillar/cluster planning, navigation, URL structure, orphan pages, and internal linking.

## Architecture Principles

- Organize around user tasks and durable entities, not only keyword lists.
- Each indexable page needs a distinct purpose, canonical URL, and path from crawlable internal links.
- Keep important pages discoverable through meaningful hubs. Click depth is diagnostic, not an absolute ranking rule.
- Facets, filters, tags, pagination, search pages, and parameters require an explicit crawl/index/canonical policy.
- Breadcrumbs should reflect hierarchy and use valid structured data when implemented.

## Cluster Design

For each cluster define:

1. Hub purpose and scope
2. Child topics with non-overlapping intent
3. Commercial or product destinations supported
4. Link directions: hub-to-child, child-to-hub, relevant sibling links, and content-to-conversion links
5. Coverage gaps and pages to merge

Avoid treating every article as a pillar or forcing circular links. Links should help the reader take a logical next step.

## Internal-Link Plan

Provide exact mappings when page content is available:

| Source URL/section | Suggested anchor concept | Target URL | Reader benefit | Priority |
|---|---|---|---|---|

Check orphan pages, broken links, redirecting targets, excessive template links, competing anchors, and important pages with weak contextual support. Do not claim an exact insertion point without inspecting the source content.

## Migration and URL Changes

Inventory existing URLs, traffic, links, canonicals, redirects, and indexation first. Map every retired URL to the closest genuine replacement; avoid redirecting unrelated pages to the homepage. Update internal links, canonicals, hreflang, sitemaps, and analytics annotations, then monitor crawl and index signals.
