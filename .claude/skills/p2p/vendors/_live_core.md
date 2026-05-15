LIVE_CORE_V8C v8C.1 — Session state baseline. Resets each new session, auto-populates during operation.

Tracks: session ID, timestamp, environment (Code/API/Projects/Chat), total prompts, corrections, agent calls.

ATLAS State: empty at start; activates after first /p2p-atlas or Tier ≥2 task.

Routing Memory: bias deltas for all 8 agents; history of recent routing decisions.

Constraint Management: reinjection cycles at messages 25, 50, 75; active constraint tracking.

Model config: primary claude-opus-4-7; fallback claude-sonnet-4-6; optional thinking levels and temperature.

Verified 2026-05-02; all 7 invariants passed.
