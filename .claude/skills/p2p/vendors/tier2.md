TIER2_V8C v8C.1 — Balanced-tier vendors.

Claude Sonnet 4.6 (PRIMARY for v8C.1 Tier 2):
- API: claude-sonnet-4-6
- Legacy RETIRE 2026-06-15: claude-sonnet-4-20250514
- Context: 200K | Free tier: yes (default since May 2026)
- Best for: T2-3, production
- G-errors: G7 (temperature + thinking → HTTP 400)

Gemini 3.1 Flash:
- API: gemini-3.1-flash
- Context: 1M | Cost: Budget
- Best for: high-volume batching, long context cheaply
- G-errors: G1 (temp during Deep Think), G2 (XML in system context), G12 (hard 429 rate limit — vs Gemini soft queue)

Verified 2026-05-02; all 7 invariants passed.
