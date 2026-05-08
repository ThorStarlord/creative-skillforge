# Creative Skillforge

A versioned library of reusable creative AI skills, meta-prompts, workflows, and stateful systems for ideation, drafting, revision, and long-term project development.

This repository is designed to preserve and evolve repeatable creative processes, especially for AI-assisted storytelling, narrative design, prompt engineering, and workflow automation.

## Core Philosophy

Good AI collaboration requires:
- **Clear Scope**: Understanding exactly what is being asked and what the boundaries are.
- **Preserved State**: Keeping track of decisions, canon, and progress over time.
- **Explicit Constraints**: Working within defined rules to ensure consistency and creative friction.
- **Reusable Workflows**: Standardizing processes so they can be improved and repeated.
- **Controlled Invention**: Balancing AI creativity with authorial intent and established facts.
- **Clean Handoffs**: Ensuring a smooth transition between different phases of work.

## Repository Structure

- **`prompts/`**: Raw meta-prompts for copy/paste use.
- **`skills/`**: Packaged instructions for specific AI capabilities.
- **`templates/`**: Reusable ledgers, logs, and handoff formats.
- **`examples/`**: Demonstrations of the system in use.
- **`changelog/`**: Tracking evolution and improvements.

## Getting Started

The core of the Creative Skillforge is the three-phase story development system:

1.  **Ideation** (`prompts/story/story-ideation-meta-prompt-v3.md`): Top-down creation from Feeling to Scene.
2.  **Drafting** (`prompts/story/story-drafting-meta-prompt-v1.md`): Execution of scenes within the structural engine.
3.  **Revision** (`prompts/story/story-revision-meta-prompt-v2.md`): Bottom-up diagnosis and refinement.

Use the **State Manager** (`prompts/story/story-state-manager-meta-prompt-v1.md`) to coordinate these phases and maintain the source of truth for your project.
