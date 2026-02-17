# Codex Operating Contract (repo-local)

## Non-negotiables
1) Keep a running task log in `.codex/inbox/YYYY-MM-DD_<task>.md`.
2) When you learn something durable, update memory:
   - Conventions/decisions → `.codex/memory/decisions.md`
   - Sharp edges/gotchas → `.codex/memory/gotchas.md`
3) Prefer using `.codex/helpers/*` scripts instead of guessing commands.
4) Before finalizing work:
   - run the relevant checks (via helpers)
   - update notes
   - commit code + notes in the same PR/branch
5) End-of-task is not complete until both are done:
   - update memory files when applicable (`.codex/memory/decisions.md`, `.codex/memory/gotchas.md`)
   - commit code changes and `.codex/` note/memory updates together
6) Before you finish, paste the completed checklist from `.codex/templates/task_close.md` into the active inbox task file.

## Output format for each task
- Plan (short)
- Changes made (files)
- Commands executed + results
- Risks / assumptions
- What was added to memory

## Git hygiene
- Work on a dedicated branch.
- Use small commits if needed, but always include the note updates.
- Never push secrets. Never commit credentials.
