DEBUG_V8C.1 — AI Agent Failure Debugging Framework. 5-step methodology:
1. Symptom classification
2. G-error quick checks
3. Prompt autopsy
4. Hypothesis ranking
5. Fix verification

Error categories: G-errors (API-level failures, HTTP 400s) and Type A-P behavioral failures (silent timeouts, context drift, hallucination, format confusion).

Key principle: "LLM = CPU, context window = RAM. Lost-in-the-Middle: rules in middle 55% decay; primacy + recency survive."

Common fixes: remove temperature during extended thinking; add MUST NOT counterparts; constraint reinjection every 25 messages; format locks in both primacy and recency zones.

Escalation: after 5 failed attempts, reconsider task formulation.
