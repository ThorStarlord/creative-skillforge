# Story Prompts Changelog

## [1.0.0] - 2024-05-22
### Added
- **Story Ideation Meta-Prompt v3**: Top-down architecture from Feeling to Scene.
- **Story Drafting Meta-Prompt v1**: Scene execution with intensity control.
- **Story Revision Meta-Prompt v2**: Layered diagnosis and revision.
- **Story State Manager Meta-Prompt v1**: Coordination and ledger maintenance.
- **Initial Templates**: State Ledger, Decisions Log, and Revision Handoff.
- **Skill Documentation**: SKILL.md files for all major phases.
- **Workflow Demo**: "The Clockwork Heart" example.

---
*Note: This repository follows semantic versioning for its meta-prompts.*

## 2026-05-08 — Story Recovery v1
### Added
- Recovery / Narrative Reverse Engineering bridge workflow (`prompts/story/story-recovery-meta-prompt-v1.md`).
- Depth modes: `SCAN` (minimum viable recovery), `MAP` (full 9-layer recovery), `FORK` (2–3 variants), `HANDOFF` (prepared input for State Update).

### Changed
- Clarified default RECOVERY DEPTH behavior: prefer `SCAN` for fragments or very long/low-context material, use `MAP` for short-to-medium material or explicit full recovery requests.
- Story State Manager now preserves Recovery metadata during ingestion and added `CONFIRM RECOVERY [LAYERS]` command to mark accepted recovered layers.

### Fixed
- README: Fixed a Markdown typo in the Bridge Workflow entry and added a brief usage example.

## 2026-05-08 — Revision & Recovery Scope System
### Added
- Engine/Chapter/Prose scopes added to the Revision meta-prompt (`prompts/story/story-revision-meta-prompt-v3.md`).
- `RECOVERY SCOPE` options formalized in Recovery (`prompts/story/story-recovery-meta-prompt-v1.md`) with `ENGINE` default.
- Scope-specific Revision supplements: Engine Layer Map, Chapter Function, and Prose Modulation.
- `PREPARE PHASE` command made scope-aware and State Manager now supports optional `[SCOPE]` parameter.
- Templates: `templates/recovery-handoff.md`, `templates/revision-scope-handoff.md`.
- Examples: `examples/revision-prose-example.md`, `examples/recovery-scan-example.md`.

### Changed
- Tightened Revision `ENGINE` wording and added an `ENGINE` alignment-audit path when no symptom is provided.
- Reinforced `PROSE` no-rewrite rule in Revision.
- README: Documented Revision/Recovery scopes and added quick examples.

### Notes
- Scopes are implemented as options within existing prompts; no split into separate prompts yet. Monitor `PROSE` usage for possible future specialization.
