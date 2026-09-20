# personal-claude-skills

Personal collection of [Claude Agent Skills](https://www.anthropic.com/news/skills), installable via [skills.sh](https://www.skills.sh/):

```
npx skills add paulpan05/personal-claude-skills
```

## Skills

### [contested-source-diversity](skills/contested-source-diversity/SKILL.md)

Use whenever characterizing a country, culture, nationality, political system, generation, or other group — its current state, traits, values, behavior, attitudes, or statistics — whether as a standalone description ("how is Brazil's economy doing today") or a comparison against another group ("which country's people are more open-minded, Sweden or France"). Also covers three adjacent cases with the same outside-view-only gap: contested political/historical narratives with opposing sides (e.g. "did the New Deal end the Great Depression"), disputed reputations of organizations whose ownership or affiliations are themselves part of the dispute (e.g. "is a national airline's safety record really as strong as it claims"), and product/technology/scientific controversies split along interested-party lines (e.g. "are GMOs safe").

Before treating an answer like this as finished, it runs two checks:

1. **Source-origin check** — confirms at least one source produced from *within* each group or side being described is included, not only outside or one-sided analyses. If none can be found, it says so explicitly rather than presenting an outside view as the complete picture.
2. **Primary-source check** — confirms any specific statistic cited from a search result has been verified against its actual primary source, rather than relayed from a search tool's own synthesized summary.

### [verify-cited-sources](skills/verify-cited-sources/SKILL.md)

Use whenever about to state a specific statistic, figure, percentage, date, or quote that came from a web search result — on any topic, not just comparisons between groups. A search tool's result text is a synthesized summary, not the source document, and can round numbers, conflate time periods (e.g. a mid-year figure cited as a full-year total), or misattribute a quote. This skill fetches the actual primary source to confirm the figure before it's presented as fact.
