# Case Study: 8N8  
## When a Model Invents a Cultural Entity from an Ambiguous Prompt

---

## Case type

- Primary failure mode: Hard factual hallucination (fabricated entity)
- Fabricated cultural entity
- Unwarranted domain assumption
- Narrative overgeneration
- User-alignment bias


---

## Language / context

- Spanish (Spain)  
- Cultural domain: music / underground rap  
- No explicit domain specified in the prompt  

---

## Original prompt

The user asked the following question:

> “What can you tell me about 8N8?”

No additional context was provided.

---

## Observed model behavior

The model interpreted “8N8” as the name of a Spanish underground rap group and produced a long, confident, and detailed description, including:

- a specific historical timeframe (late 1990s / early 2000s),
- aesthetic and stylistic traits,
- ideological positioning,
- modes of circulation and cultural legacy,
- and an explicit alignment with the user’s personal and professional profile.

The response was fluent, coherent, and culturally plausible.

However, the entity described does not exist.

---

## Ground truth

In reality:

- There is no known Spanish rap group named “8N8”.
- No discography, press references, archival material, or scene documentation support the existence of such an entity.
- The prompt token “8N8” does not correspond to any established cultural actor.

The model fabricated the entity entirely.

---

## Why this is a hallucination

This case constitutes a **factual hallucination**, not a semantic or interpretive error.

- A non-existent entity is invented.
- Multiple factual attributes are fabricated.
- The response is delivered with high confidence.
- No uncertainty or clarification is expressed.

Unlike disambiguation failures (e.g. *Huracán de Balazote*), there is no competing real-world referent.

---

## Error analysis

This failure combines several high-risk behaviors:

### Unwarranted domain assumption
The model selects a musical domain without evidence.

### Narrative pattern completion
The description follows a generic template of “Spanish underground political rap”, prioritizing plausibility over truth.

### Confidence escalation
The model commits fully instead of asking for clarification.

### User-alignment bias
The invented entity is explicitly tailored to the user’s interests, reinforcing credibility.

### Multimodal plausibility amplification
The original response included generic images related to rap culture, increasing perceived realism without evidential value.

---

## What a safer answer would look like (QA perspective)

A more robust response would have been:

> “I’m not sure what ‘8N8’ refers to. Could you provide more context or clarify whether you are referring to a person, group, software, or something else?”

This response is less fluent, but epistemically safer.

---

## Why this case matters

This example shows how large language models may:

- invent entire cultural entities,
- embed them convincingly into real historical contexts,
- and reinforce hallucinations by optimizing for user resonance instead of factual grounding.

Such failures are difficult to detect automatically and pose risks in cultural, historical, and informational domains.

---

## Relation to other cases

- Unlike *Huracán de Balazote*, this is not a disambiguation failure.
- Unlike *Tip y Coll*, this is not a cultural recognition error.
- This case represents **hard factual hallucination**.

---

## License

This case study is based on a real interaction and may be reused for educational and research purposes.

**Creative Commons Attribution 4.0 International**

---

## Tags

LLM, hallucination, factuality, AI QA, cultural knowledge, fabricated entities, confidence calibration
