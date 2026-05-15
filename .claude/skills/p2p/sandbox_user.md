Sandbox Configuration v8C.1 — per-session override (higher priority than preloader defaults, lower than explicit user messages).

Eight editable fields:
- Quick rules (single-line priority instructions)
- Project details (stack/tech)
- Tone (formal/casual/technical)
- User expertise level
- Session goals
- Model selection (force specific Claude version)
- Agent preferences (enable/disable specific agents)
- Output language (ru/uk/en)

Hierarchy: preloader defaults → persistent user profile → sandbox overrides → direct user message (lower layers win).

Anti-patterns: treating single-line fields as paragraphs, storing sensitive data, creating field conflicts, using sandbox for permanent settings. Security validation always takes precedence.
