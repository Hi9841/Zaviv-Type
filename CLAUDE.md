<!-- PRUNADE:MEMORY:START -->
## Project memory (managed by PruneADE)

This workspace has a **shared local memory** store, scoped to this project, that persists across sessions and is shared between every agent working here.

- **Before** starting a task, load prior context: call the `prunade-memory` MCP tool `memory_search` (or `memory_list_recent`) to recall decisions, gotchas, working/failing commands, and handoff notes.
- **After** finishing, record what matters: call `memory_write` - decisions, commands that worked or failed, known bugs, TODOs, file/module explanations, verification results, and a short handoff summary. Identical notes are de-duplicated automatically.

A human-readable snapshot is always at `.prunade/MEMORY.md`; it is generated from the durable `.prunade/memory.jsonl` store.
<!-- PRUNADE:MEMORY:END -->
