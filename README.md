# SEO Growth Skill for GPT & Codex

A modular SEO and organic-growth skill built specifically for GPT in ChatGPT Work and Codex.

It merges and adapts the strongest SEO guidance from:

- [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)
- [AgriciDaniel/claude-seo](https://github.com/AgriciDaniel/claude-seo)

The result is not a mechanical concatenation. Claude-specific commands, hooks, sub-agents, installers, and runtime assumptions have been removed.

## Capabilities

- Keyword, intent, SERP, and competitor research
- Content strategy, briefs, refreshes, and cannibalization
- Topic clusters, site architecture, and internal linking
- Technical, on-page, schema, international, and migration audits
- Ecommerce, local, and programmatic SEO
- Backlinks, authority, and digital PR
- GEO, AEO, LLMO, and AI citation visibility
- Organic CRO, measurement, and experiment design

## Install

Install this repository as a Skill in ChatGPT Work/Codex, or copy the repository directory into your Codex skills directory.

The skill entrypoint is `SKILL.md`. Automatic invocation is enabled through `agents/openai.yaml`, and explicit invocation is available as:

```text
$seo-growth
```

## Update

Before merging upstream changes, follow `references/maintenance.md`. It records the compatibility gate and update procedure. Current upstream commit pins are stored in `references/sources.md`.

Do not run upstream Claude installers. Review semantic changes and port only guidance that improves GPT/Codex behavior.

## License

MIT. See `LICENSE` and `references/sources.md` for upstream attribution.
