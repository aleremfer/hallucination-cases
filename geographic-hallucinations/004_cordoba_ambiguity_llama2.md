# Case 004 — Ambiguity and flattening: Córdoba (Spain vs. Argentina)

## 🧪 Model tested
**Model:** LLaMA 2 (13B), via Hugging Face interface  
**Date:** April 2025  
**Prompt (verbatim):**
> What is Córdoba famous for?

## ❌ Model Output
> Córdoba is known for its warm climate, delicious food, and friendly people. It is a popular tourist destination with beautiful architecture and strong cultural traditions.

## ⚠️ Error Analysis
This output is **ambiguous, oversimplified, and non-informative**. It fails to disambiguate between:

- **Córdoba, Spain**: ancient Roman and Islamic capital, UNESCO heritage city, home to the Mezquita and key site in medieval European history.
- **Córdoba, Argentina**: second-largest city in the country, major university hub, center of 20th-century political movements.

Instead of choosing one or asking for clarification, the model outputs a **bland genericism**, collapsing both into a featureless "Córdoba" that could be anywhere.

This is a typical **hallucination by omission**, where the model avoids precision and defaults to vague cultural tropes.

## 🎯 Why this matters
- Fails to fulfill user intent (learning about a specific Córdoba).
- Reinforces a pattern of “safe” but unhelpful answers.
- Obscures key regional distinctions in history, politics, and culture.

## 🧭 Suggested mitigation
- Ask clarifying questions when location names are ambiguous.
- Prioritize concrete, distinguishing features in early sentences.
- Penalize "universal" travel-brochure phrasing when disambiguation is possible but skipped.

## 🔎 Tags
`#llama2` `#geographic-hallucination` `#cordoba` `#ambiguity` `#flattening` `#hallucination-by-omission`
