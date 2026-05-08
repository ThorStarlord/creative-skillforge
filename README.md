# Creative Skillforge

A versioned library of reusable creative AI skills, meta-prompts, workflows, and stateful systems for ideation, drafting, revision, and long-term project development.

This repository is designed to preserve and evolve repeatable creative processes, especially for AI-assisted storytelling, narrative design, prompt engineering, and workflow automation.

## Core Philosophy: The Bidirectional Engine

Good AI collaboration requires a structured narrative engine that supports three complementary movements:
- **Top-Down Ideation**: Moving from generative causes (**Target Experience**) toward visible execution (**Modulation**).
- **Bottom-Up Diagnosis**: Starting from a symptom in the text and tracing it downward to find the broken root cause.
- **Bottom-Up Recovery**: Starting from unfinished material and extracting the implied engine before returning to Ideation, Drafting, or Revision.

### The 9 Layers of Story
1.  **Target Experience**: Audience feeling and emotional promise.
2.  **Promise / Constraints**: Genre, mode, and medium constraints.
3.  **Scope / Scale**: Story length and subplot capacity.
4.  **Structural Forces**: Want, resistance, conflict, stakes, and change.
5.  **Threads / Modules**: Main plot and subplots.
6.  **Carriers**: Character, setting, and world systems.
7.  **Representation**: Events, scenes, and reveals.
8.  **Modulation**: POV, pacing, tone, and style.
9.  **Resonance / Coherence Check**: Alignment across all layers.

## Repository Structure

- **`prompts/`**: Raw meta-prompts for copy/paste use.
- **`skills/`**: Packaged instructions for specific AI capabilities.
- **`templates/`**: Reusable ledgers, logs, and handoff formats.
- **`examples/`**: Demonstrations of the system in use.
- **`changelog/`**: Tracking evolution and improvements.

## Getting Started

The core of the Creative Skillforge is a three-phase story development cycle supported by a Recovery bridge workflow:

### Core Cycle
1.  **Ideation** (`prompts/story/story-ideation-meta-prompt-v4.md`): Top-down creation from Experience to Modulation.
2.  **Drafting** (`prompts/story/story-drafting-meta-prompt-v2.md`): Execution of scenes within the structural engine.
3.  **Revision** (`prompts/story/story-revision-meta-prompt-v3.md`): Bottom-up diagnosis and refinement.

### Bridge Workflow
- **Recovery / Narrative Reverse Engineering** (`prompts/story/story-recovery-meta-prompt-v1.md`): A bridge workflow for unfinished drafts. It extracts the implied story engine from existing material and returns the project to Ideation, Drafting, or Revision.
	- Depth modes: `SCAN` (minimum viable recovery), `MAP` (full 9-layer recovery for short-to-medium material), `FORK` (2–3 variants), `HANDOFF` (prepared input for State Update).

Example (brief):

RECOVERY DEPTH: SCAN
TEXT: [messy scene / abandoned fragment]
ORIGINAL INTENT: I thought this was a revenge story.
RECOVERY QUESTION: What is this actually trying to become?

The **State Manager** coordinates Ideation, Drafting, Revision, and the Recovery bridge workflow. Recovery is used when existing draft material must be reverse-engineered into a recovered story engine before returning to Ideation, Drafting, or Revision.

Use the **State Manager** (`prompts/story/story-state-manager-meta-prompt-v2.md`) to coordinate these phases and maintain the source of truth for your project. When handoff requires updating the ledger, the recommended next-workflow label `State Update` indicates the ledger should be updated before choosing the next creative phase.
