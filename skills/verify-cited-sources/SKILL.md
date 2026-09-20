---
name: verify-cited-sources
description: >-
  Use whenever about to state a specific statistic, figure, percentage, date, or quote that came from a web search result — before including it in a response, verify it against the actual primary source rather than relaying the search tool's own synthesized summary. This applies regardless of topic and is not limited to comparisons between groups: economic data ("GDP grew 4.4% this year"), survey or poll results ("62% of respondents said..."), a quoted line attributed to a document or speech, a historical date, or any other case where a search result's summary text is about to be repeated as settled fact. Trigger this even when the number sounds unremarkable, and especially when it sounds clean, round, or persuasive, or when it describes a period that may not yet be complete (e.g. a "full-year" figure cited before the year has ended).
---

# Verify cited sources before repeating their claims

A web search tool's result text is a synthesized summary written by a model, not the source document itself. It can round numbers, conflate time periods (reporting a mid-year figure as if it were a full-year total, or a projection as if it were a settled result), misattribute a quote, or drop qualifying context that changes what the number actually means. Presenting that summary text as a verified fact passes along whatever the summarizer got wrong.

Before stating a specific number, date, or quote pulled from a search result, fetch the underlying page it is attributed to (or open the primary document directly) and confirm the figure is actually there, in the form you're about to state it. This applies any time a number is about to be handed to the user as fact — not only in comparative questions between groups, and not only when a claim seems doubtful going in.

Two concrete failure examples this catches:
- Stating "Brazil's full-year 2026 GDP is $2.3T, growing 3.1%" when the year in question hadn't ended yet — the only real backing was a mid-year (H1) figure from Brazil's national statistics agency; the "full-year" framing came from a secondary aggregator's projection, relayed by the search summary as if it were already-reported fact.
- Citing a "75% vs. 45%" gap from a survey without opening the actual report — the search summary's paraphrase could have rounded, applied to a different subgroup than implied, or misstated which side of the comparison a figure belongs to.

One extra tool call (fetching the source page) before stating the number is the full cost of avoiding this. Skipping it to save a step is the specific failure this skill exists to catch: a plausible-sounding, unverified number is worse than a slower answer that either confirms the figure or says plainly that it couldn't be confirmed.
