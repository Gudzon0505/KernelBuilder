MEMORY_V8C v8C.1 — Memory Bridge (cross-session memory system). Three tiers:
1. In-session: automatic
2. Cross-session: user-managed CAPSULE format
3. Permanent: project configuration

CAPSULE Protocol (triggered via /p2p-capsule save or [24]): YAML/Markdown format capturing project metadata, progress, key decisions with rationales, active constraints, blockers, context summaries (~10:1 compression: 100 messages → 10 sentences), routing memory biases.

Auto-triggers: after SPLITTER completion phases; every 50 messages; at context limit; on explicit command.

XML-based memory block schema for decisions, failed attempts, domain glossaries, session metrics.

Design principle: "Carry state, not context. State is compressed decisions."
