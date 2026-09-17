# AI Evaluation Strategy Canvas

> Repo file `ai-evals/01-evaluation-strategy/strategy-canvas.md` (the repo is your submission).
> Becomes the Strategy Canvas slide of the final pitch deck you assemble in Module 6.

## 1. Product Strategy, The Context

**Target user:** VP-level Strategists and Product Leaders at Fortune 500 companies who pay a premium for verified market intelligence.

**Key use case:** Rapidly extracting specific, verified insights (e.g., comparing competitor pricing models or summarizing G2 reviews) without manual data digging.

**Value proposition:** Personalized, instant answers based on verified data, dramatically reducing the time spent finding and synthesizing information for high-stakes decisions and strategic roadmaps.

## 2. Measurements, The Execution

**User promise.** For VP-level Enterprise Strategists, Ascend IQ promises to deliver verified, citation-backed competitive intelligence in under 5 seconds so that they hit their Q4 roadmap decisions without manual data digging.

**Top 3 trust metrics:**
- **Latency**, Response speed (P95 / P99). Slow kills engagement.
- **Hallucination Rate**, % of outputs that are confidently false or fabricated.
- **Fairness**, Quality consistency across user groups, geos, languages.

**Why these three:** • Hallucination: VP level clients pay $50k+ annually for verified intelligence; fabricated information directly undermines the core product promise. 
• Latency: a response under 5 seconds provides a significant speed advantage over manual data digging. 
• Fairness: consistent factual quality across languages and geographies ensures enterprise customers receive comparable answer quality.

## 3. Strategic Trade-Offs, The Cost

### Trade-off 1 · Hallucination Rate ↔ Latency
We prioritize Hallucination Rate over Latency because Ascend IQ serves VP level customers paying $50k+ annually for verified market intelligence. A fabricated competitor statistic directly undermines the product's core promise, whereas modest additional response time is an acceptable cost for higher factual integrity.

---
_Generated from the AI Evaluation Strategy Canvas, M1 lab tool, AI Evals Certification._
