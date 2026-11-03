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
- [DAY_WISE/](DAY_WISE/) — seven day-wise records; a day may span multiple sessions.
- [ADVANCED_MODULES/](ADVANCED_MODULES/) — modules A–L.
- [PRACTICALS_PROJECTS/](PRACTICALS_PROJECTS/) — eight practical projects and evidence.

## Supplementary discussion notes — user-controlled saving

The `EXTRA_NOTES/` folder is reserved for supplementary concepts discussed alongside the formal Git/GitHub course. **Do not save, summarize into repository notes, or update this folder automatically. Only do so when the learner explicitly asks to save the supplementary discussion or specific material.**

- A discussion, useful explanation, correction, diagram, or substantial topic is **not** permission to save it.
- Requests such as “continue”, “explain more”, or “what does this mean?” are not save requests.
- Save only the material the learner explicitly identifies or clearly asks to preserve. If the scope is unclear, ask what they want saved.
- When explicitly authorized, prefer updating an existing relevant note; create a new Markdown file only for a substantial, distinct subject. Update `EXTRA_NOTES/README.md` when adding a file.
- Preserve accurate explanations, useful examples and editable Mermaid diagrams where appropriate. Keep supplementary notes separate from the formal syllabus and learner-progress records.
- Saving a note does not introduce, practise or verify a formal syllabus topic.
- Do not save secrets, access tokens, private keys or unnecessary sensitive personal information.
- After an authorized repository edit, fetch changed files again and report exactly which files were verified.

**Default: do not write supplementary discussion notes unless the learner explicitly requests it.**
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

## Screenshot and visual-asset storage standard

Store useful visual assets in the repository when they materially improve a lesson; do not create empty asset folders in advance.

- **Where to store:** keep assets close to the curriculum they support: `DAY_WISE/assets/`, `ADVANCED_MODULES/assets/` or `PRACTICALS_PROJECTS/assets/`. Create these folders only when the first relevant asset is added. Use clear filenames such as `day-01-git-file-states.png`, `module-c-merge-conflict-resolution.png` or `project-03-pull-request-review.png`.
- **Link from the lesson:** embed the image in the relevant Markdown lesson with descriptive alt text and a short caption explaining what the learner should notice. Keep the asset and lesson link together in the same change.
- **Use the right format:** PNG for terminal/UI captures and diagrams with text; JPEG/WebP for photographic illustrations where appropriate; GIF only for short instructional motion. Prefer editable Mermaid for flowcharts and commit graphs rather than taking a screenshot of a diagram that can be rendered from source.
- **Authenticity:** label each visual as an authentic interface capture, instructor-created illustration/mock-up, or illustrative terminal example. Never fabricate a screenshot and present it as a real GitHub screen or learner terminal output. An expected-output capture is not evidence that the learner ran the command.
- **Privacy and attribution:** redact usernames, email addresses, repository details when private, tokens, keys, URLs containing credentials and other personal data. Never commit secrets. Credit external images and respect their licences; prefer original course-created visuals.
- **Quality and accessibility:** crop irrelevant UI, keep text legible at normal zoom, use consistent callouts, provide meaningful alt text, and explain the important area in nearby prose. Avoid duplicate, decorative or oversized screenshots.
- **Maintenance:** use relative Markdown links, verify every asset path and image render after committing, and replace obsolete captures when the interface changes. Do not add an image solely to satisfy a checklist.

Screenshots are instructional media, **not learner evidence** unless the learner supplied the capture and its provenance is clear. Record learner evidence separately in the progress files. GitHub Markdown does not support arbitrary embedded interactive widgets; use supported static visuals here and interactive controls in ChatGPT when appropriate.



## Complete lesson notes and visual documentation

The day-wise files are the actual study notes, not merely topic checklists. When a concept is taught in ChatGPT, add its substantive explanation to the relevant `DAY_WISE/day-XX-*.md` file as part of the normal course record. Do not leave a taught topic as an instruction such as “teach this here” or an empty placeholder.

For each concept actually taught, capture the relevant material:
- Clear definition, purpose and real-world need.
- First-principles explanation and mental model.
- Editable Mermaid diagram, state chart, sequence diagram or commit graph when it improves understanding.
- Color-coded tables/labels using the shared visual legend.
- Syntax/options and Windows Git Bash instructor demonstrations where relevant.
- Clearly labelled illustrative expected output and explanation.
- Common mistakes, troubleshooting and professional use.
- A concise revision summary.

Keep the lesson notes faithful to what was actually taught. Do not fill future topics with invented lessons, and do not mistake an instructor demonstration for learner execution. Add image assets only when a real visual adds value; Mermaid source is preferred for editable diagrams. Verify each changed lesson file after writing.

## Random spaced-revision prompts — learner-authorized

The learner has requested occasional, short revision pop-ups during the course. This is an explicit opt-in to **brief retrieval-practice prompts** drawn at varied, unpredictable points from:
- Previously taught concepts across earlier days and advanced modules.
- Important distinctions, mistakes and examples already covered.
- Supplementary material in `EXTRA_NOTES/` that has actually been saved.

Guidelines:
- Keep a prompt short (normally one to three questions), focused and conversational; vary timing and topic rather than interrupting every lesson.
- Ask about material that has already been taught or saved; never quiz on an untaught topic.
- Mix recall, command choice, interpretation and short troubleshooting scenarios. Do not reveal the answer until the learner responds, unless they request study mode or the answer.
- Give feedback, correct misconceptions and link the explanation back to the relevant lesson/extra note.
- These are revision prompts, not formal day/module assessments. Keep full quizzes, interviews and practicals behind their separate explicit opt-in gates.
- If the learner declines or asks to continue the lesson, respect that and resume teaching without pressure.
- Do not invent a real-time notification or background popup. Present the prompt naturally inside an active ChatGPT conversation when an appropriate opportunity occurs.
- Record meaningful revision outcomes only when the learner actually responds; a prompt being offered is not an attempt or a verified result.
