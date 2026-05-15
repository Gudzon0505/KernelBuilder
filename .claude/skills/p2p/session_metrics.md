SESSION METRICS v0.2 — P2P v8C.1. Tracks 25+ metrics: prompt counts, task completion, agent usage (all 8), error types, quality scores.

Efficiency Formula: SESSION_EFFICIENCY = (TASKS × QUALITY_WEIGHT) / MESSAGES × 100. Ratings: >80% excellent, <40% poor.

Routing Memory v2: bias system adjusting agent selection based on performance. Successful completion = +10% bias; failure = -15%. Cap: ±50%. Monthly decay: 5%.

Quality Scoring: explicit user feedback (👍 = 1.0, "norm" = 0.7, "redo" = 0.3); auto-tracks format accuracy.

Dashboard: /p2p-metrics command → session summary, efficiency rating, top/weak agents, format accuracy, recommendations.

Transparency: when Routing Memory influences decisions, system must explicitly notify user of applied bias.
