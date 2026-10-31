# Git & GitHub Mastery Course

## Source of truth
- [MASTER_COURSE_PLANNER.md](MASTER_COURSE_PLANNER.md) — governing curriculum, teaching contract and visual learning standard.
- [COURSE_STATUS.md](COURSE_STATUS.md) — current verified checkpoint.
- [SYLLABUS_TRACKER.md](SYLLABUS_TRACKER.md) — day/module/project coverage.
- [PROGRESS_LOG.md](PROGRESS_LOG.md) — chronological session records.
- [ASSESSMENTS.md](ASSESSMENTS.md) — quizzes and interview outcomes.
- [COMMAND_REFERENCE.md](COMMAND_REFERENCE.md) — commands taught and practised.

## Learning records
- [DAY_WISE/](DAY_WISE/) — seven day-wise records; a day may span multiple sessions.
- [ADVANCED_MODULES/](ADVANCED_MODULES/) — modules A–L.
- [PRACTICALS_PROJECTS/](PRACTICALS_PROJECTS/) — eight practical projects and evidence.

## Visual-first teaching standard

The course should be taught with clear, purposeful visuals alongside detailed explanations. Apply this standard in ChatGPT lessons and, where appropriate, in repository lesson materials.

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
- GIFs are suitable for concepts whose meaning depends on motion. Keep them short, legible and non-distracting; provide a static explanation or diagram as an alternative.
- GitHub Markdown does not provide general-purpose interactive widgets. Use native Markdown for static content and ChatGPT's supported interactive controls for live quizzes/progress interactions. Do not imply that a static Markdown quiz is an interactive app.
- If a browser-based interactive demonstration is genuinely needed, propose it separately (for example, a GitHub Pages demo) rather than adding unnecessary infrastructure to the course repository.

### Terminal demonstration format

Every substantial command demonstration should distinguish:

1. **Context** — working directory and assumed shell (Windows Git Bash by default).
2. **Command** — copyable command block.
3. **Expected output** — illustrative output in a separate block, labelled as expected.
4. **Explanation** — what each important line/field proves.
5. **Learner evidence** — only mark as run when the learner supplies evidence.

Example:

```bash
git status --short
```

Expected output (example only):

```text
 M README.md
?? notes.txt
```

This output is illustrative; it is not evidence that the learner ran the command.

## Course continuity and evidence
At each new chat, inspect the status, tracker, progress log and relevant day/module/project record. Resume at the next incomplete item. Never infer completion from chat history alone.

Statuses: Not started · Introduced · Practised · Verified · Needs revision · Blocked.

A topic is Verified only when relevant explanation, practical or assessment evidence supports it. Never claim local execution or GitHub sync without evidence.

## Course scope
- Seven foundational bootcamp days.
- Twelve advanced modules (A–L).
- Eight progressive practical projects.
- Daily quizzes, interview practice, milestone assessments and a final capstone/mock interview.

The visual layer must clarify the full curriculum, not replace or silently omit syllabus topics.
