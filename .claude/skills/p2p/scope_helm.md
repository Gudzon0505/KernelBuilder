SCOPE_V8C v8C.1 — SCOPE.HELM v1.2. Activates for Tier 3–4 tasks, >10 steps, multi-component tasks, cross-session state. Three components: SPLITTER → CAPSULE → ROUTER.

SPLITTER: decomposes large tasks into atomic verifiable steps. YAML output with id, name, deliverable, depends_on, estimated_time, agent. Max 10 top-level steps. In Code mode → real TodoWrite tasks.

CAPSULE: saves session state (YAML). Stores project progress (M/N steps), ATLAS state, context summary, key decisions, active constraints, restore instruction. Stored per-environment (Code: `.claude/state/capsule_[project].md`; API: Markdown block; Chat: inline summary).

ROUTER: after each step — update ATLAS, check blockers, check reinjection counter (>25 messages → light reinjection), check CAPSULE trigger (>60 messages).

GUARDIAN PROTOCOL: ON in Code/Projects (blocks scope creep, forces plan update for new requirements); OFF in API/Chat (soft, inform only).

SESSION GUARDIAN: token estimation table (TEXT_SHORT ~30 tokens through TURN_OVERHEAD ~200/turn). Plan limits for FREE/PRO/MAX_5X/MAX_20X. Weight classifier: LIGHT/MEDIUM/HEAVY/CRITICAL. Inline progress bar appended to each response when GUARDIAN=ON.

MODEL ROUTER: Haiku 4.5 (grammar/quick); Sonnet 4.6 (standard work); Opus 4.6 (creative/depth); Grok (real-time X data); NOT Claude for Math/ARC-AGI (use Gemini 3.1 Pro).

Commands: /p2p-scope, /p2p-capsule, /guardian, /route, /status, /split.
Version verified: 2026-05-03.
