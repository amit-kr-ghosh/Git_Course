# Day-wise Learning Records

The seven bootcamp days are stored in separate folders: `DAY-01/` through `DAY-07/`. Each folder has a `README.md` index and keeps the actual lesson material in sequential session files.

## Day folders
- [Day 1 — Foundations](DAY-01/README.md)
- [Day 2 — File lifecycle and safe undo](DAY-02/README.md)
- [Day 3 — Branching, merging and conflicts](DAY-03/README.md)
- [Day 4 — GitHub collaboration](DAY-04/README.md)
- [Day 5 — Advanced Git and history editing](DAY-05/README.md)
- [Day 6 — Actions, quality and security](DAY-06/README.md)
- [Day 7 — Integrated capstone](DAY-07/README.md)

## Session note structure

Each distinct teaching segment is saved as a separate Markdown file in its day folder:
`SESSION-01-<topic>.md`, `SESSION-02-<topic>.md`, and so on. Session numbering continues across chats for that day. Each session note should contain the substantive material actually taught: explanation, first-principles reasoning, diagrams, Windows Git Bash instructor demonstrations, illustrative expected output, common mistakes, troubleshooting and revision summary as appropriate.

When a learner says “next” or “continue” and a new concept is taught, add a new session file and update that day's README index. Do not overwrite earlier session notes. A clarification of the current concept belongs in the current session note; create another session file when a distinct lesson segment is taught.

The legacy day records were moved into their corresponding day folders without discarding their syllabus or checkpoint content. For Day 1, the existing foundations record is retained as Session 1. For Days 2–7, the existing curriculum templates are retained as `CURRICULUM-AND-SESSION-INDEX.md`; actual lesson sessions will be added as they are taught.

## Visual lesson authoring checklist
- Use focused Mermaid flowcharts, state diagrams, sequence diagrams or commit graphs when they clarify the concept.
- Apply the shared color legend: blue worktree, amber staging, green commits/verification, purple remote/collaboration, red risk/conflict.
- Include relevant technical images or annotated screenshots only when they add information; use alt text and redact private data.
- Use short instructional GIFs only when motion is essential, and include a static alternative.
- Use interactive knowledge checks in ChatGPT only when the learner opts in; static Markdown is not an interactive widget.
- Present terminal demonstrations as context, command, illustrative expected output and explanation.
- Keep learner-run evidence separate from instructor demonstrations.
- Preserve the complete syllabus, practical, troubleshooting, interview and revision requirements; do not mark completion without evidence.

## Screenshot and image storage
- Store useful Day 1–7 captures under `DAY_WISE/assets/`; create this folder only when the first asset is ready.
- Embed images in the relevant session note with a relative path, descriptive alt text and caption.
- Prefer authentic, current Git Bash/GitHub captures for interface-specific teaching; label instructor-created mock-ups and illustrative output honestly.
- Redact personal information, private repository details, tokens, keys and credential-bearing URLs.
- Prefer Mermaid source for editable diagrams; use GIF only when motion is essential.
- A teaching screenshot is not learner practical evidence.
- Verify image paths render on GitHub after the lesson and asset are committed.

See the visual teaching standard in [MASTER_COURSE_PLANNER.md](../MASTER_COURSE_PLANNER.md).
