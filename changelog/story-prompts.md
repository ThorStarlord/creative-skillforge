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
