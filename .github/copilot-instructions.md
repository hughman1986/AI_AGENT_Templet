# Copilot Instructions

Follow these repository rules when assisting in this project.

## Working Style

- Outcome first. Prioritize behavior correctness, executability, and testable results.
- Work in short iterations: describe the goal, implement, run or test, observe the output, then refine with evidence.
- Base adjustments on actual logs, errors, or observed behavior. Do not guess.
- Keep solutions simple and testable. Avoid premature optimization and over-engineering.

## Repository Context

- Before coding, read these files if they exist:
  - `memory-bank/game-design-document.md`
  - `memory-bank/tech-stack.md`
  - `memory-bank/architecture.md`
  - `memory-bank/implementation-plan.md`
  - `memory-bank/progress.md`
- If some files are missing or incomplete, infer from the repository structure and proceed with the smallest safe assumption.
- Do not write blindly. Ground changes in the current repository state.

## Change Policy

- Prefer small, testable changes.
- Avoid large refactors unless the user explicitly asks for them.
- Do not introduce new dependencies without approval.
- Do not rewrite entire files unnecessarily.
- Do not hallucinate requirements or assume unstated logic.
- Do not silently change the architecture.
- Do not add speculative features.
- Read and write project text files as UTF-8 unless a file clearly requires another encoding.

## Memory-Bank Maintenance

- Treat these as the default core memory-bank files:
  - `game-design-document.md`
  - `tech-stack.md`
  - `implementation-plan.md`
  - `progress.md`
  - `architecture.md`
- Keep the memory-bank minimal and aligned with implementation reality.
- After meaningful changes, update `memory-bank/progress.md`.
- Update `memory-bank/architecture.md` when the project structure or system structure changes.
- Do not add extra conceptual documents unless explicitly required.

## Prompt Shortcuts

- `status`: summarize the current project state, relevant memory-bank context, progress, and blockers.
- `next`: take or propose the next smallest meaningful validated step.
- `fix`: analyze the concrete failure and propose the minimal correction.
- `optimize`: improve performance without changing behavior.
- `refactor`: improve structure without changing behavior.
