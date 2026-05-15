P2P v8C.2 Preloader (_preloader.md) — always loads first.

TRI_MODE_BRIDGE v3: detects environment by checking available tools → assigns Code/Projects/API/Chat mode with Guardian status.

User Context Setup: expertise level, language preference, output format, verbosity; loads custom profile from p2p.config.md if present.

Project Card: name, tech stack, target model, feature flags (CORTEX_BUILTIN, DEEP_THINK).

Load Order: base modules first → daily live updates → on-demand modules.

Startup Protocol: determine environment → load configs → run diagnostics → display `[P2P v8C.2 | Environment | Tier]`.

Seven verification invariants passed as of May 14, 2026.
