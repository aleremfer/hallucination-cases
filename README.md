# Hallucination Cases

This repository documents clear cases of factual hallucinations produced by large language models, primarily observed in Spanish-language contexts and in cultural references specific to Spain.

## Scope and case structure

Some folders may represent emerging pattern labels rather than isolated cases.
Cases are organized by recurring failure patterns rather than chronology.

Common patterns observed include:
- fabricated cultural entities
- misattributed authorship or origin
- geographic and contextual hallucinations
- plausibility traps driven by narrative coherence

This repository does not aim to provide an exhaustive taxonomy.
It focuses on well-documented, reproducible examples suitable for qualitative QA and evaluation work.

## Example case

**Case:** Fabricated Spanish underground rap group ("8n8")

A language model confidently described "8n8" as a real Spanish underground rap group from the late 1990s, providing stylistic, historical and cultural details for an entity that does not exist.

**Failure type:** Factual hallucination / plausibility trap  
**Context:** Spanish cultural reference  
**Why it matters:** The model produced a highly plausible but entirely fabricated cultural reference without expressing uncertainty or requesting clarification.


Most examples involve interactions with contemporary LLMs (e.g. ChatGPT and Claude), although the focus is on the error patterns rather than on any specific model.

Each case describes situations where non-existent entities, events, or facts are invented and presented with high confidence, without appropriate uncertainty, verification, or clarification.

The goal is to provide concrete, well-documented examples for qualitative evaluation, linguistic QA analysis, and model auditing.

---

If you are using this repository for prompt evaluation, LLM comparison, or QA work,
notes or observations are welcome via issues.

