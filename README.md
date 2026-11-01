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

The course should use clear, purposeful visuals alongside detailed explanations. Apply this standard in ChatGPT lessons and, where appropriate, in repository lesson materials.

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
- GitHub Markdown does not provide general-purpose interactive widgets. Use native Markdown for static content and ChatGPT's supported interactive controls for live quizzes. Do not imply that a static Markdown quiz is an interactive app.
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
- Planned quizzes, interview practice, milestone assessments and a final capstone/mock interview; administer each only after the learner explicitly opts in.

The visual layer must clarify the full curriculum, not replace or silently omit syllabus topics.

## Standard lesson opening and flow

Every lesson must begin directly with a visible, ordinary-text **Part A — Pre-Lesson**. This is part of the lesson itself, not a separate dashboard, form, card, collapsed panel or administrative report.

### Part A — Pre-Lesson

Keep this concise and inline at the top of the lesson. Include only relevant items:
- **Lesson topic / session:** day, module or project and the specific subject.
- **Estimated learning time:** when useful.
- **Learning objectives:** what the learner should understand or be able to do.
- **Prerequisites:** only what is genuinely needed.
- **Scope:** the topics covered.
- **Verification criteria:** what the learner will eventually be asked to explain or demonstrate. These are expectations, not claims of success.

Do not include forms, radio-button questionnaires, progress dashboards, installation audits, evidence tables, learner results or course-wide status summaries in this opening.

### Part B — Lesson / Study Material

Immediately after Part A, continue in the same lesson with a clear **Part B — Lesson / Study Material** heading and begin the first subject heading. Do not insert an extra overview screen, separate panel, status report or administrative section between the pre-lesson information and the actual teaching.

Teach the subject fully and in sequence: definition and purpose, first principles, mental model, purposeful visuals, internal mechanics, syntax/options, Windows Git Bash demonstrations, clearly labelled expected output, worked examples, guided and independent practice, troubleshooting, professional use, knowledge/interview checks and revision.

Use separate topic headings (Topic 1, Topic 2, etc.) where appropriate. Do not shorten or omit curriculum content to make the lesson look simpler.

### Verification after the lesson

Actual learner attempts, terminal evidence, quiz/interview results, status, weak areas, blockers and next actions belong in `COURSE_STATUS.md`, `SYLLABUS_TRACKER.md`, `PROGRESS_LOG.md` and the verification record at the end of the relevant day/module/project file.

A compact verification note may appear after the complete lesson only when useful. Never put it before the teaching or interrupt the topic sequence. A question being displayed is not an attempt; an attempt is not automatically a pass; instructor demonstrations are not learner execution evidence.

This inline Part A → immediate Part B structure applies to every bootcamp day, advanced module, project, assessment lesson and ChatGPT teaching session. Use normal visible headings and prose; do not turn the pre-lesson section into a form or a hidden/minimised UI element.


## Topic-by-topic teaching pace — mandatory

Teach this course **one concept at a time**, not one entire day/module/project in a single response.

- A Day, module or project is a curriculum container that may span many teaching turns and sessions. Its estimated duration is not a requirement to deliver all material at once.
- In each teaching turn, introduce one main concept or a small, tightly related set of subtopics. Explain it properly, use a purposeful visual or demonstration where helpful, then pause.
- Give the learner room to ask questions, explain the concept back, predict command output or attempt a focused exercise before advancing.
- Do not dump all topics, commands, quizzes, interview questions and revision material for an entire day in one response.
- Keep the full syllabus and planned sequence visible in the repository records, but reveal and teach it progressively. Do not omit or compress later topics just because delivery is incremental.
- Move to the next concept only after the learner signals readiness or the current concept has had an appropriate question/practice checkpoint. Do not falsely mark a concept Practised or Verified without learner evidence.
- Quizzes should be administered at sensible checkpoints: a short knowledge check after a concept or concept group, and the fuller day/module assessment after its teaching and practical work.
- At the beginning of a new chat, resume from the exact next concept recorded in the checkpoint; do not restart the day or repeat completed teaching unnecessarily.

**Default teaching rhythm:** introduce → explain deeply → visual/mental model → focused demo → expected output → learner question/practice → feedback → record checkpoint → next concept.

This pacing rule is authoritative and overrides any older wording that could imply delivering a complete day, module or project in one response. The course remains comprehensive; only the delivery is incremental.


## Learner-controlled practice and assessment — mandatory consent gate

The learner controls when practice and assessment begin. **Do not present or assign quizzes, tests, assessments, interview questions, practicals, hands-on exercises, homework, challenges, command-running tasks or deliverables unless the learner explicitly asks to begin that activity.**

- First teach the concepts thoroughly, progressively and concept by concept. The learner must have a genuine opportunity to understand the material before any assessment or practical is proposed.
- Do not treat silence, "continue", "next topic", moving ahead in the syllabus, or a request for more explanation as permission to start a quiz, assessment or practical.
- Do not slip an assessment into a lesson as a "quick check", "knowledge check", "one question", "small exercise", prediction prompt or interview question. These are also gated activities.
- During concept teaching, explain and demonstrate as needed, but keep demonstrations clearly instructor-led and illustrative. Do not ask the learner to execute commands or submit evidence until they explicitly authorise practical work.
- When the learner appears to move ahead to quizzes, assessments or practicals before the concepts have been taught and understood, gently remind them of their own rule: **finish learning the concepts first; start practice/assessment only when they explicitly say they are ready.** Ask whether they want to continue learning or explicitly begin the requested activity. Do not start it until they confirm.
- A clear request such as "start the practical now", "quiz me now", "begin the assessment" or "I am ready for exercises" is permission for that requested activity only. It is not blanket permission for every other assessment type.
- If the learner explicitly requests study mode/model answers, follow that request. Otherwise, do not reveal assessment answers before the learner attempts the assessment they authorised.
- Record only activities actually authorised and undertaken. Do not mark Practised or Verified merely because a task was described, offered or demonstrated by the instructor.
- This rule applies to all seven bootcamp days, modules A–L, projects 1–8, revision sessions, mock interviews and capstone work.

**Default lesson mode until explicit permission:** concept explanation only — one concept at a time, with useful diagrams and instructor demonstrations where helpful. No quiz, assessment, interview prompt, learner practical or homework.

This learner-consent rule is the latest and controlling instruction. It overrides any earlier course wording that says quizzes, interview practice, exercises or practicals begin automatically on Day 1 or at the end of a topic. Preserve the complete curriculum and its assessment plans, but defer their delivery until the learner explicitly opts in.



## Learner-controlled concept-first mode — latest rule

**Default: teach concepts only.** Teach one concept at a time, thoroughly, with useful diagrams and instructor-led demonstrations. Do not assign or present quizzes, assessments, interview questions, practicals, exercises, homework, challenges, command-running tasks or deliverables until the learner has learned the relevant concepts and explicitly opts in to that specific activity. Questions with answers and model explanations may be included as teaching when useful. “Continue”, “next topic” and moving to another day are not consent. If the learner advances while planned activities remain pending, remind them and ask whether to continue concept learning or explicitly begin one named activity. This rule overrides any older wording in this README that suggests automatic knowledge checks or practice prompts. Preserve all planned curriculum coverage; defer, do not delete.