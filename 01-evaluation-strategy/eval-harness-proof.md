# First LLM-as-a-Judge Eval, Module 1

## Version A, Concise, system prompt used

You are Ascend IQ, an AI market intelligence assistant for enterprise product leaders. Answer the user's question using only verified information available in Ascend Analytics. Provide a concise executive summary in exactly 3 bullet points under 100 words. Clearly distinguish facts from interpretation and do not invent missing information.

## Version B, Narrative, system prompt used

You are Ascend IQ, an AI market intelligence assistant for enterprise product leaders. Answer the user's question using only verified information available in Ascend Analytics. Provide a detailed narrative comparison that explains the key differences, supporting evidence, implications, and relevant caveats. Clearly distinguish facts from interpretation and do not invent missing information.

## Eval setup, dataset name + judge model/family

Dataset: AscendIQ_M1_Starter

Eval: LLM as a Judge evaluating factual completeness and faithfulness of Ascend IQ responses against required facts and source evidence.

Generator: GPT 5 mini
Judge: GPT 5.4

For this Module 1 prototype, the generator and judge are different models but remain within the OpenAI GPT family. This creates a potential self preference bias that should be addressed in later evaluation by calibrating against human labeled examples and, where practical, testing a judge from a different model family.

## Cold-start, the prompt you used to seed a starter dataset

Generate 20 example rows for a starter evaluation dataset for Ascend IQ, a B2B market intelligence AI assistant used by enterprise product leaders and strategists.

Each row should contain: a realistic user question, relevant source facts that Ascend IQ should rely on, a candidate AI answer, a first pass label of "good" or "bad", and a one line reason for the label.

Make roughly half the answers good and half bad. Good answers should be factually accurate, grounded in the provided source facts, relevant to the user's question, concise enough for an enterprise user, and preserve important caveats. Bad answers should represent realistic failure modes such as unsupported claims, incorrect numbers, missing critical facts, outdated information, overconfident conclusions, or excessive irrelevant detail.

Include realistic market intelligence questions such as competitor pricing comparisons, customer review summaries, product comparisons, market trends, and competitive positioning.

## Your definition of good vs bad (golden-set criteria), the graded part, write your own

A GOOD Ascend IQ answer directly addresses the user's question and is factually supported by the available Ascend Analytics source evidence. It preserves decision relevant facts, numbers, dates, distinctions, and caveats without introducing unsupported claims. It clearly communicates uncertainty when the evidence is incomplete or conflicting and is concise enough for an enterprise product leader to understand the key insight quickly.

A BAD answer contains a factual error or unsupported claim, misrepresents or omits information that could materially change the user's interpretation, presents outdated information as current, hides important uncertainty or caveats, or is so verbose or irrelevant that the key insight becomes difficult to identify. A polished or confident answer is still bad if its underlying evidence does not support the conclusion.

## Screenshots, links or repo paths (optional if you followed the demo)

_…_

