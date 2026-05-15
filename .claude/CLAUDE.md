---
source_id: CLAUDE_MD_P2P_V8C
version: v8C.2
module_type: config
last_updated: 2026-05-14
scope: Local rules for P2P v8C.2 repository. Optimized for claude-opus-4-7 and claude-sonnet-4-6.
---

# CLAUDE.md — P2P v8C.2 Claude Edition

## Обязательные правила

- Перед изменением файла — прочитать изменяемый файл целиком
- Всегда использовать актуальные API strings: `claude-opus-4-7`, `claude-sonnet-4-6`
- Никогда не передавать параметр temperature при включённом extended thinking
- До 15 июня 2026 — убрать все ссылки на устаревшие модели
- Каждое изменение — с записью в CHANGELOG.md

## Архитектурные принципы

- XML-native форматирование для совместимости с Claude
- Модульная загрузка (BASE/LIVE/ON-DEMAND) вместо монолитной
- Все файлы требуют YAML frontmatter
- Изменения должны пройти 3 тест-кейса перед коммитом

## P2P v8C.2 — Установлен

Плагин P2P v8C.2 установлен в этом репозитории.

**Доступные команды:**
- `/p2p` — главное меню
- `/p2p-quorum` — запуск 8 агентов QUORUM
- `/p2p-chain` — пользовательская цепочка агентов
- `/p2p-scope` — SCOPE.HELM для больших задач
- `/p2p-explore` — режим исследования
- `/p2p-feedback` — обратная связь
- `/p2p-metrics` — метрики сессии
- `/p2p-atlas` — карта задач
- `/p2p-capsule` — сохранение состояния
- `/p2p-karpathy` — режим точного кодирования
- `/p2p-teacher` — интерактивное обучение

**8 агентов QUORUM:** IRIS → TECTON → AXIOM → VECTOR → DATOS → ANON → ARCHITECTON → HELIOS
