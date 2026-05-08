# Creative Skillforge

A versioned library of reusable creative AI skills, meta-prompts, workflows, and stateful systems for ideation, drafting, revision, and long-term project development.

This repository is designed to preserve and evolve repeatable creative processes, especially for AI-assisted storytelling, narrative design, prompt engineering, and workflow automation.

## Core Philosophy: The Bidirectional Engine

Good AI collaboration requires a structured narrative engine that works in two directions:
- **Top-Down Ideation**: Moving from generative causes (**Target Experience**) toward visible execution (**Modulation**).
- **Bottom-Up Diagnosis**: Starting from a symptom in the text and tracing it downward to find the broken root cause.

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

The core of the Creative Skillforge is the three-phase story development system:

1.  **Ideation** (`prompts/story/story-ideation-meta-prompt-v4.md`): Top-down creation from Experience to Modulation.
2.  **Drafting** (`prompts/story/story-drafting-meta-prompt-v2.md`): Execution of scenes within the structural engine.
3.  **Revision** (`prompts/story/story-revision-meta-prompt-v3.md`): Bottom-up diagnosis and refinement.

Use the **State Manager** (`prompts/story/story-state-manager-meta-prompt-v2.md`) to coordinate these phases and maintain the source of truth for your project.
