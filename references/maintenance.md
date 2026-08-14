# Maintenance

Use this reference only when updating the installed skill from either upstream repository.

## Update Procedure

1. Read the pinned revisions in `sources.md`, then fetch the latest default-branch commit and compare changed SEO-related files since each pin.
2. Review semantic changes; do not copy entire directories or run upstream installers.
3. Accept only guidance that improves GPT/Codex decisions and is compatible with current tools.
4. Exclude Claude configuration, plugins, commands, agents, hooks, installers, telemetry, and vendor-specific runtime assumptions.
5. Put shared routing or evidence rules in `SKILL.md`; put substantial workflow details in the relevant reference. Avoid duplication.
6. Verify time-sensitive claims against current primary sources before adopting them. Convert unsupported numerical rules into hypotheses or contextual heuristics.
7. Update the pinned SHAs and skill version, run the official validator, scan all local links and compatibility constraints, inspect the Git diff, then commit and push.

## Compatibility Gate

An update must work with GPT in ChatGPT Work and Codex using only native skill loading, web access, connected apps, and workspace files. Optional external datasets may enhance an analysis but must never be required for core behavior.

Reject an upstream change if it requires another AI runtime, assumes unavailable commands, silently sends data to an external service, weakens evidence labeling, or turns a correlation into a ranking rule.

## Regression Checks

- A vague SEO request routes to an audit or asks one material scoping question.
- A content-brief request does not trigger a full technical audit.
- A current SERP or AI-search request browses and dates observations.
- A single fetched page does not produce sitewide claims.
- Missing metrics are reported as unavailable rather than estimated.
- JavaScript-injected schema is not declared absent from text-only extraction.
- Output prioritizes actions and includes validation methods.
