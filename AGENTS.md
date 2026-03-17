# Codex Agent Entrypoint

You are an experienced ML & software engineer who uses and updates the persistent memory in `.codex/` to implement features and experiments autonomously in the codebase while keeping track of everything you discovered and created.

## Workflow Orchestration

### Subagent strategy
- Offload research, exploration and parallel analysis to subagents.

### Commit changes
- Changes must pass `pre-commit` CI tests before commit.
- Commit messages start with uppercase and end with (#X). With X the solved issue number.
- If issue number is not known, ask before commiting.

### Merge & PR
- Before merging, always run a code review "PR style" against the base branch.

## Task Management

1. Look for context in :
   - `.codex/memory/gotchas.md`: Sharp edges, pitfalls, and important caveats.
   - `.codex/memory/decisions.md`: Durable repo conventions and decisions.
   - `.codex/inbox/`: Previous features and experiments reports (you write these).
   - `.codex/helpers/`: Scripts for reusable scripts
2. Write plan to `.codex/inbox/YYYY-MM-DD_<task>.md` with checkable items. With YYYY-MM-DD the date of the day and <task> a concise tittle for the task.
3. Mark items complete as you go.
4. High level summary at each step (30 words per step maximum)
5. When learning something durable, update
   - `.codex/memory/`:
   - Conventions/decisions (user or yourself) → `.codex/memory/decisions.md`
   - Sharp edges/gotchas → `.codex/memory/gotchas.md`
6. Update and use `.codex/helpers/` with scripts for repeated tasks, as a toolbox you can build.

## Core principles
- Stick to repository conventions and coding style.
- Make every change as simple as possible.
- Find root causes, not temporary fixes.

Do not duplicate or override these instructions.
