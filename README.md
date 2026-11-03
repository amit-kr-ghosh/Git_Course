# Git & GitHub Mastery Course

## Source of truth
- [MASTER_COURSE_PLANNER.md](MASTER_COURSE_PLANNER.md) — governing curriculum, teaching contract and visual learning standard.
- [COURSE_STATUS.md](COURSE_STATUS.md) — current verified checkpoint.
- [SYLLABUS_TRACKER.md](SYLLABUS_TRACKER.md) — day/module/project coverage.
- [PROGRESS_LOG.md](PROGRESS_LOG.md) — chronological session records.
- [ASSESSMENTS.md](ASSESSMENTS.md) — quizzes and interview outcomes.
- [COMMAND_REFERENCE.md](COMMAND_REFERENCE.md) — commands taught and practised.

## Learning records
- [EXTRA_NOTES/](EXTRA_NOTES/) — supplementary reference notes from related discussions; separate from the core curriculum and progress records.
- [DAY_WISE/](DAY_WISE/) — seven day folders; each day has a README and, after completion, one consolidated whole-day revision note.
- [ADVANCED_MODULES/](ADVANCED_MODULES/) — modules A–L.
- [PRACTICALS_PROJECTS/](PRACTICALS_PROJECTS/) — eight practical projects and evidence.

## Day-wise learning records

The `DAY_WISE/` directory is organised as `DAY-01/` through `DAY-07/`. During a day, teach and discuss the syllabus in ChatGPT; do not create or update lesson/session files after individual concepts.

**One note per completed day:** only after the learner has finished the entire planned syllabus for that day and its required completion criteria have been satisfied with evidence, create one concise `REVISION-SUMMARY.md` in that day's folder and link it from the day README. The note is a consolidated revision aid for the whole day, not a transcript or a session log. Until then, keep the day’s teaching in the conversation and maintain only the course-level progress records needed for accurate continuity.

This rule applies consistently to Days 1–7. Supplementary discussions remain separate and are saved to `EXTRA_NOTES/` only when the learner explicitly asks. Creating a day summary does not itself prove completion or upgrade progress status.

## Supplementary discussion notes — user-controlled saving

The `EXTRA_NOTES/` folder is reserved for supplementary concepts discussed alongside the formal Git/GitHub course. **Do not save, summarize into repository notes, or update this folder automatically. Only do so when the learner explicitly asks to save the supplementary discussion or specific material.**

- A discussion, useful explanation, correction, diagram, or substantial topic is **not** permission to save it.
- Requests such as “continue”, “explain more”, or “what does this mean?” are not save requests for supplementary notes.
- Save only the material the learner explicitly identifies or clearly asks to preserve. If the scope is unclear, ask what they want saved.
- When explicitly authorized, prefer updating an existing relevant note; create a new Markdown file only for a substantial, distinct subject. Update `EXTRA_NOTES/README.md` when adding a file.
- Preserve accurate explanations, useful examples and editable Mermaid diagrams where appropriate. Keep supplementary notes separate from the formal syllabus and learner-progress records.
- Saving a note does not introduce, practise or verify a formal syllabus topic.
- Do not save secrets, access tokens, private keys or unnecessary sensitive personal information.
- After an authorized repository edit, fetch changed files again and report exactly which files were verified.

**Default: do not write supplementary discussion notes unless the learner explicitly requests it.**

## Visual-first teaching standard

The course should use clear, purposeful visuals alongside detailed explanations. Apply this standard in ChatGPT lessons and repository lesson materials.

| Visual element | How it supports learning |
|---|---|
| 🎨 Color-coded diagrams | Consistent visual language for worktree, staging, commits, remotes, risks and conflicts |
| 🧩 Mermaid diagrams | Flowcharts, sequence diagrams, state diagrams, decision trees and Git commit graphs |
| 🖼️ Technical imagery | Relevant illustrations, annotated screenshots and terminal/UI captures |
| 📊 Knowledge checks | Interactive questions in ChatGPT; compact Markdown quizzes and answer-hidden exercises in repository files |
| 🎞️ Animation | Short GIFs only when motion explains a changing state, pointer, merge or workflow |
| 💻 Terminal demonstrations | Separate copyable commands, expected output and explanation, with learner-run evidence clearly distinguished |

### Consistent visual language
| Cue | Meaning |
|---|---|
| 🔵 Blue | Working directory, active work or current branch |
| 🟠 Amber | Staging area, pending change or decision |
| 🟢 Green | Commit, successful verification or completed safe step |
| 🟣 Purple | Remote repository, GitHub or collaboration |
| 🔴 Red | Risk, destructive operation, failed check or unresolved conflict |

Use labels and shapes as well as colors so diagrams remain understandable for color-blind readers and in monochrome.

### Diagram and media guidelines
- Prefer Mermaid for editable, text-based diagrams that GitHub can render: `flowchart`, `sequenceDiagram`, `stateDiagram-v2` and `gitGraph`.
- Keep diagrams focused: one main idea per diagram, meaningful labels, directional arrows and a short explanation below.
- Use images only when they add information; include useful alt text and cite/credit external assets where required.
- Use screenshots to demonstrate real interfaces or terminal states. Redact usernames, email addresses, tokens, keys and other private information.
- GIFs are suitable for concepts whose meaning depends on motion. Keep them short and legible; provide a static explanation as an alternative.
- GitHub Markdown does not provide general-purpose interactive widgets. Use native Markdown for static content and ChatGPT's supported interactive controls for live quizzes. Do not imply a static Markdown quiz is an interactive app.
- Terminal demonstrations should show context, copyable command, illustrative expected output and explanation. Learner evidence is recorded only when supplied.

## Course continuity and evidence
At each new chat, inspect the status, tracker, progress log and relevant day/module/project record. Resume at the next incomplete item. Never infer completion from chat history alone.

Statuses: Not started · Introduced · Practised · Verified · Needs revision · Blocked.

A topic is Verified only when relevant explanation, practical or assessment evidence supports it. Never claim local execution or GitHub sync without evidence.

## Course scope
- Seven foundational bootcamp days.
- Twelve advanced modules (A–L).
- Eight progressive practical projects.
- Planned quizzes, interview practice, milestone assessments and a final capstone/mock interview; administer each only after the learner explicitly opts in.

The full curriculum and learner-consent rules remain governed by [MASTER_COURSE_PLANNER.md](MASTER_COURSE_PLANNER.md).


## Selective note-taking and end-of-day revision summaries

Keep repository notes **high-value and concise**. Capture only information that materially helps future learning or continuity: core concepts and mental models, important distinctions, essential commands/options, useful diagrams, representative examples, common mistakes/safety warnings, and unresolved points or the next checkpoint. Do not archive every chat message, repeated explanation, minor clarification, decorative visual, or redundant command output. Prefer improving the relevant existing note over creating duplicates. The final day note should be a useful study reference, not a transcript.

### Day completion summary
When a day's full planned syllabus has been taught **and** its required completion criteria have been met with evidence (including any practical/assessment items required by that day's definition of done), create one concise whole-day revision note in that day's folder. For Day 1, the file will be `DAY_WISE/DAY-01/REVISION-SUMMARY.md`. It should distil the day's essential mental models, lifecycle/workflows, commands and their differences, key safety points, common mistakes, and links to the session notes. Do not reproduce every lesson or add unverified claims. Add it to the day README only when the completion criteria are actually satisfied. If teaching is complete but practice/verification remains deferred, do not label the day complete or create the final completion summary prematurely; a clearly labelled interim recap may be offered in chat, but it is not the final day-completion record.

The same rule applies to Days 2–7: use `REVISION-SUMMARY.md` in the corresponding day folder only after that day's completion criteria are met. Summary creation is a study aid, not independent evidence of completion.
