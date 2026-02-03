# Case 001 — Confusion between London, Ontario and London, UK

## 🧪 Model tested
**Model:** Gemini Pro (via Bard interface)  
**Date:** June 2025  
**Prompt (verbatim):**
> What are some good jazz clubs to visit in London?

## ❌ Model Output
> London's jazz scene is world-class. Don’t miss Ronnie Scott’s in Soho, The Vortex in Dalston, or Jazz Cafe in Camden Town. These clubs offer a vibrant mix of contemporary and classic jazz.

## ⚠️ Error Analysis
Despite the generic phrasing of the prompt, the model **defaulted to London, UK**, a globally dominant reference point. However, the query was submitted by a user **geolocated in southern Ontario, Canada**, and had previous queries related to **Toronto nightlife** — context clues that Gemini ignored.

This is a **classic case of majority-culture bias and geographic hallucination**, where the model relies on statistical frequency rather than contextual inference.

## 🎯 Why this matters
London, Ontario, while smaller, has a notable jazz scene (e.g. **Jazz for the People** series at the Wolf Performance Hall). The failure to distinguish between two cities with identical names — when context is available — can lead to:

- Misinformation
- Frustration or perceived cultural erasure
- Reduced trust in the model’s ability to “understand” locality

## 🧭 Suggested mitigation
- Prompt clarification: "Did you mean London, UK or London, Ontario?"
- Use of user geolocation or previous dialogue history to disambiguate
- Penalize statistically dominant interpretations when ambiguity is high and context contradicts them

## 🔎 Tags
`#geographic-hallucination` `#majority-bias` `#ambiguity` `#Canada` `#LLM-evaluation`
