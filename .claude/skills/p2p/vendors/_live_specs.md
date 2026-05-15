Live Vendor Specs v8C.1 — centralized reference for 10 major providers: Claude (Opus 4.7, Sonnet 4.6), Gemini (3.1 Pro/Flash), Grok (4.3 variants), GPT-5.5, DeepSeek, Qwen, Kimi. Context windows up to 2M tokens.

Routing: Claude for reasoning; Gemini for up to 1M context; Grok for 2M context or real-time X data. Fallback chain: Claude primary → vendor-specific alternatives.

Critical translation rules per vendor:
- Gemini: proper thinking config; no XML in system context
- Grok: standard parameters only
- GPT-5.5: max 7 rule pairs
- DeepSeek: clear reasoning_content in multi-turn; some variants deprecated July 2026
