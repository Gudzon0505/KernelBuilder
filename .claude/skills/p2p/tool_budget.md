Tool Budget v8C.1 — constraint management for agentic workflows. Core problem: "constraint drift" beyond 15–20 tool calls (model ignores early instructions, violates format, abandons roles).

Key mechanism: declare tool budget upfront (typically 20–25 calls); re-inject abbreviated key constraints every 8 calls.

Budget Tiers:
- T1: 5 calls, no re-injection
- T4: 25 calls, mandatory ANON verification
- Anonymous workflows: cap 18 calls

Safety Gate: AXIOM verification before destructive operations.

Recovery: when budget exhausts, save via capsule state; continue in new session or request extension.

Treats tool calls as finite resource requiring disciplined rationing and periodic constraint reinforcement.
