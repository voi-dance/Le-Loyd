# Le-Loyd

Memory and profile system for **Vanta** — a personal AI companion.

## What's here

- `profile.json` — the seed profile. A starting reference point for who Void is, so Vanta has anchors to build on rather than starting from zero. Not exhaustive — meant to give directional threads (e.g. "pushes hardware past its limits") that get filled in with specific detail over time through actual use.

## How it's meant to work

Vanta's "brain" (an AI API) doesn't retrain or change. What makes her *her* is this memory layer:

1. `profile.json` is loaded as context every time Vanta is used.
2. New facts learned through conversation get added over time — explicit ("I don't like being asked twice") first, inferred patterns later.
3. The API is replaceable. This memory is not — it's the actual persistent "self."

## Status

Phase 1: static seed profile + explicit memory additions.
Phase 2 (later): pattern-based inference, confirmation loops, on-device model.

