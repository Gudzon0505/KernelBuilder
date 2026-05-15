LIVE_CLAUDE_V8C v8C.1 — Claude-specific live data. Update on every Anthropic release.

Claude Models (May 2026):

Claude Opus 4.7:
- API: claude-opus-4-7 | Context: 200K | Output: 32K | Cost: $15/1M in, $75/1M out
- Arena Elo: Code #1 (1571), Text #1 (1503), Vision #1 (1303) | Free tier: No
- Extended Thinking: effort low/medium/high
- Bedrock/Vertex: claude-opus-4-6 alias (not yet switched)
- Active G-Errors: G6 (+10-35% tokenizer inflation → effective max 160K), G7 (HTTP 400 temp+thinking), G8 (MRCR recall 32.2% at 1M → use Opus 4.6 for >500K recall)

Claude Sonnet 4.6:
- API: claude-sonnet-4-6 | Context: 200K | Output: 32K | Free tier: Yes (default since May 2026)
- G-Errors: G7 (same rules)

Claude Haiku 4.5:
- API: claude-haiku-4-5-20251001 | Extended Think: limited | Previously default (replaced by Sonnet 4.6)

Claude Opus 4.6 (Pinned):
- API: claude-opus-4-6 | Keep for: long-context recall >500K (G8 protection), cost-sensitive, Bedrock/Vertex
- MRCR at 1M: 78.3% (vs 32.2% for 4.7)

RETIREMENT ALERT [DEADLINE 2026-06-15]:
- claude-opus-4-20250514 → claude-opus-4-7
- claude-sonnet-4-20250514 → claude-sonnet-4-6

Extended Thinking API (May 2026):
```python
{
    "model": "claude-opus-4-7",
    "thinking": {"type": "enabled", "effort": "medium"},
    "messages": [...],
    "max_tokens": 4096
}
# budget_tokens: REMOVED. temperature: FORBIDDEN with thinking enabled (G7).
```

Pricing: Opus 4.7 $15/$75 in/out; Sonnet 4.6 ~$3/~$15; Haiku 4.5 <$1/<$5. Prompt caching: 70–90% savings, min 1024 tokens.

Context strategy:
- <160K → Opus 4.7
- 160K–200K → Opus 4.7 with caution (G6)
- >200K → Sonnet 4.6
- >500K → Opus 4.6 pinned (G8 protection)

Verified 2026-05-02.
