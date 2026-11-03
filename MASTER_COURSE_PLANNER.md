# Git & GitHub Mastery — Master Course Planner

This repository follows the user's 23-page Git & GitHub Master Planner, Version 2.0 (1 November 2026). This file is the concise governing index; preserve the source planner's full syllabus scope and terminology when teaching.

## Operating contract
Goal: practical Git/GitHub competence from beginner through advanced. Environment: Windows, Git Bash default; explain PowerShell/CMD differences when useful. The initial bootcamp has seven curriculum days (original estimate 60–120 minutes/day); advanced learning continues without an arbitrary end date. A day/module may span multiple sessions.

## Seven-day bootcamp
1. **Foundations and first repository:** version control; local/centralised/distributed models; Git vs GitHub; repository, worktree, index, local/remote; file states; commits, branches, HEAD; install/configure Git; init, add, commit, status, diff, log.
2. **File lifecycle, inspection and safe undo:** status/diff variants, show/log, commit quality, staging, .gitignore, restore, reset modes, revert, amend, clean and destructive-operation safety.
3. **Branching, merging and conflicts:** branch pointers, switch/checkout, feature branches, fast-forward/three-way merges, conflict resolution, strategies, branch cleanup, GitHub Flow/Git Flow/trunk-based development.
4. **GitHub and collaboration:** repositories/remotes, clone/fetch/pull/push, tracking branches, HTTPS/SSH and credential safety, forks/upstream, pull requests/reviews, issues/projects, repository documentation and permissions.
5. **Advanced everyday Git/history editing:** stash, tags/releases, semantic versioning, rebase/interactive rebase, cherry-pick, reflog, reset/revert, force-with-lease and revision syntax.
6. **GitHub platform, automation, quality and security:** Actions/YAML, CI workflows, jobs/matrices/artifacts/caches, secrets/permissions, branch protection, Pages, Dependabot/security scanning, CODEOWNERS/templates, environments and CI/CD.
7. **Integrated capstone/mock interview:** plan repository, issues/milestones, feature branches, commits, PR/review, conflict, sync, tests/CI, release/tag, recovery exercise, security/documentation audit and retrospective.

## Advanced continuation modules A–L
A. Git internals/object model: blobs, trees, commits, tags, hashing, refs, HEAD, index, packfiles, plumbing.
B. Advanced history inspection: revision parsing, ranges, log filters, blame, bisect, shortlog, describe, merge-base, archive, bundle.
C. Advanced merging/conflicts: strategies, octopus, rename detection, rerere, advanced rebase/onto and mergetool.
D. Repository scale/performance: maintenance, gc, fsck, packfiles, shallow/partial clones, sparse checkout, monorepos, LFS, performance diagnosis.
E. Multi-repository/workspaces: submodules, subtrees, worktrees, multiple remotes, mirrors, bare repositories.
F. Configuration/hooks/customisation: config scopes, aliases, attributes, filters, hooks, templates, safe.directory, credentials.
G. Security/supply chain: SSH, tokens, signing, DCO, scanning, least privilege, OIDC, Actions trust boundaries, provenance, SBOM, incident response.
H. Advanced GitHub Actions: reusable workflows, action types, matrices, caches/artifacts, environments, OIDC, self-hosted runners, expressions, automation, debugging.
I. GitHub administration/enterprise: organisations, teams, rulesets, SSO/SCIM, audit, Projects, Apps, OAuth, webhooks, APIs, GitHub CLI.
J. Team workflows/release engineering: GitHub Flow, Git Flow, trunk-based, feature flags, conventions, semantic versioning, hotfixes, backports, merge queues, reproducible releases.
K. Disaster recovery/troubleshooting: detached HEAD, reflog/fsck recovery, rejected pushes, unrelated histories, auth/remote errors, lock files, bad reset/rebase, corruption, secrets, cross-platform issues.
L. Alternatives/interoperability: SVN/Git-SVN, Mercurial, GitLab/Bitbucket, self-hosting, migration, Git transport.

## Eight-project ladder
1. Personal profile repository.
2. Versioned notes/journal with .gitignore.
3. Multi-feature website with branches and conflict resolution.
4. GitHub portfolio repository, cloneable in a second directory/machine.
5. Collaboration simulation: fork/upstream, PR, review, issues.
6. History cleanup/recovery lab in a disposable repository.
7. CI/CD website using Actions/tests and Pages where feasible.
8. End-to-end team capstone with documentation, issues, PRs, CI, release and security hygiene.

## Supplementary knowledge capture — explicit user authorization only

`EXTRA_NOTES/` is the separate location for supplementary knowledge that supports the course but falls outside the formal bootcamp, advanced modules and projects.

**Do not capture or save supplementary discussions automatically. Save or update `EXTRA_NOTES/` only when the learner explicitly asks for the material to be saved.** A useful discussion, a request for further explanation, or a “continue/next” message does not authorize repository changes.

When the learner explicitly requests saving:
1. Save only the subject or material they identify; ask for clarification if the requested scope is unclear.
2. Prefer updating the most relevant existing note. Create a new Markdown file only for a substantial, distinct subject, and add it to `EXTRA_NOTES/README.md`.
3. Preserve important explanations, corrections, comparisons, examples and useful editable Mermaid diagrams where appropriate.
4. Keep supplementary notes separate from the formal syllabus, day-wise lesson records, assessments and progress evidence. Saving a note does not introduce, practise or verify a formal syllabus topic.
5. Never save credentials, tokens, private keys or unnecessary sensitive personal information.
6. After an authorized GitHub write, fetch the changed file(s) to verify and report exactly which files changed.

**Default rule: no supplementary-note repository edits without an explicit request from the learner.**
## Teaching standard
Teach from first principles. Explain purpose, terminology, mental model, syntax, flags, preconditions, local/remote effects, expected output and verification. Use visuals only when useful. Follow explain → visualise → instructor-led demonstration → learner questions; guided practice, challenges, verification and knowledge checks occur only after the learner explicitly opts in. Never claim commands ran on the learner's machine.

## Assessments
Quizzes and interview preparation are planned from Day 1 onward, but are not administered automatically. The learner must explicitly opt in to each quiz, assessment, interview or practical activity. Preserve the planned coverage: recall, command choice, output prediction, comparisons, troubleshooting and practical verification. Do not reveal answers before an authorised attempt unless the learner requests study mode/model answers. Quiz scores alone do not prove practical mastery. Interview reference notes place each question immediately before its answer; mock interviews include scoring and feedback.

## Progress and continuity
Before teaching, read README, COURSE_STATUS, SYLLABUS_TRACKER, PROGRESS_LOG and relevant day/module/project records. Verify checkpoint and evidence. After meaningful sessions, update relevant records and commit if access permits. Report sync only after verification.

Never commit passwords, tokens, private keys or secrets. Use disposable repositories for destructive experiments. Explain risks and obtain explicit confirmation before destructive operations on shared repositories. Check installed Git version and current official documentation when version-sensitive.

## Initial checkpoint
The source planner says Day 1 was started previously, but installation and practical completion are unconfirmed. Day 1 is therefore NOT VERIFIED complete. Confirm setup and evidence before changing status. This is the tracking repository; `git-learning-journey` is a named Day 1 practical deliverable, not proof of an existing remote.


## Course presentation convention — content vs checkpoint

Keep instructional content and progress verification visibly separate in every lesson and session.

- **Learning content** belongs in the lesson: concepts, diagrams, reasoning, command syntax, instructor demonstrations, expected output, examples, exercises, troubleshooting, professional context and revision.
- **Verification checkpoint** belongs in the course-level status/tracker and a clearly separated compact footer/side panel only when needed: installation state, learner-provided evidence, quiz/interview outcome, topics verified, blockers and exact next action.
- Do not make the verification checklist the opening body of a lesson. Do not repeat the entire course-status table inside lesson content.
- A lesson can have a distinct short "Practice task" within the instructional flow. The existence of a task does not imply that it was attempted or verified.
- Keep command provenance explicit: "Demonstrated" means shown by the instructor; "Learner ran" requires learner evidence.
- In a new session, report the checkpoint briefly, then begin the actual lesson content. If the checkpoint is still pending, do not turn the lesson into a wall of status tables.


## Visual teaching and presentation standard

Use a visual-first approach throughout the seven-day bootcamp, advanced modules A–L and all eight projects. Visuals support the full syllabus; they must never replace detailed explanations, hands-on practice, troubleshooting or assessment.

### Required visual toolkit
- **Color-coded explanations:** use a consistent legend — blue for working directory/active work, amber for staging/pending decisions, green for commits/successful verification, purple for remotes/collaboration, red for risks/conflicts.
- **Mermaid diagrams:** use flowcharts for processes and decisions, sequence diagrams for client/remote interactions, state diagrams for file/branch states, and `gitGraph` for commit/branch/merge history. Choose the diagram type that best explains the concept.
- **Images and screenshots:** include relevant technical illustrations, annotated UI screenshots and terminal captures when they materially improve understanding. Add alt text; redact personal information and all credentials/secrets; credit external assets.
- **Animation:** use short GIFs only when movement is instructional (for example, a branch pointer moving, a merge occurring or a workflow progressing). Provide an equivalent static explanation; avoid decorative or distracting motion.
- **Interactive learning:** in ChatGPT lessons, use supported interactive knowledge checks, quizzes, comparison controls and progress indicators when they improve practice. In repository Markdown, use answer-hidden quizzes, checklists and tables. GitHub Markdown itself does not host general-purpose interactive widgets; do not promise embedded app behavior. A separate GitHub Pages demo may be proposed only when a real interactive simulator is justified.
- **Terminal panels:** show context, command, expected output and explanation in separate labelled blocks. Clearly label outputs as illustrative unless the learner supplied them. Explain Windows Git Bash syntax and note PowerShell/CMD differences when relevant.

### Diagram quality rules
1. One diagram should communicate one main concept.
2. Label nodes and arrows with meaningful Git terms and commands.
3. Use a legend where color carries meaning; also use text/shape differences so color is never the only signal.
4. Explain the diagram in prose and connect it to a practical command or decision.
5. Keep diagrams readable on mobile; split oversized diagrams into smaller stages.
6. Preserve complete syllabus coverage even when a topic has no useful diagram.

### Standard lesson visual sequence
For each substantial concept, consider this order:
1. Short definition and real-world need.
2. Mental model or color-coded diagram.
3. Internal mechanics and terminology.
4. Syntax/options table.
5. Windows Git Bash demonstration with expected output.
6. Practical exercise and troubleshooting decision path.
7. Professional scenario and interview/knowledge check.
8. Revision summary.

Not every small subtopic needs every media type. Select visuals for instructional value, accessibility and clarity rather than decoration.

### Accessibility, accuracy and provenance
- Use descriptive alt text and readable contrast.
- Never rely on color alone.
- Provide static alternatives for animation.
- Do not fabricate screenshots, terminal output, command execution or learner evidence.
- Distinguish instructor demonstration from learner execution.
- Never expose secrets or private information in images, screenshots, logs or diagrams.

## Mandatory lesson layout — instructional content is separate from verification

This is a course-wide rule for every bootcamp day, advanced module, practical project, assessment lesson and ChatGPT teaching session.

### A. Begin with the subject, not administration
- After the lesson title, move directly into its learning purpose/objectives and then teach the subject.
- Never begin a lesson with a large "current checkpoint", progress table, setup checklist, evidence audit or a recap of repository state.
- Do not repeat installation status, course-wide progress, verified topics, learner evidence, blockers or the next session's administrative task inside the lesson.

### B. Keep instructional content complete and coherent
The lesson body contains the actual learning material: definitions, need/purpose, first-principles reasoning, mental models, diagrams, detailed explanations, command syntax and options, Windows Git Bash demonstrations, expected output, practical tasks, troubleshooting, professional scenarios, interview questions, knowledge checks and revision notes.
- A practice task is part of the lesson. It is not a progress checkpoint and does not prove an attempt.
- Mark example terminal output as illustrative unless supplied by the learner. Instructor demonstrations and learner-run commands must remain distinct.
- Do not remove syllabus topics to shorten or beautify the lesson.

### C. Keep verification in the tracking layer
- `COURSE_STATUS.md` is the single compact current checkpoint.
- `SYLLABUS_TRACKER.md` records topic/deliverable status and evidence.
- `PROGRESS_LOG.md` records chronological session evidence and next action.
- Relevant day/module/project files may contain a **separate record area at the end** for session evidence, assessment outcomes and continuation details. Keep it after the instructional syllabus/content, not as the lesson's opening.
- A ChatGPT response may include a brief checkpoint only after the lesson, visually separated from teaching. Do not repeat the whole checkpoint if it is already recorded and unchanged.

### D. Standard lesson sequence
1. Lesson title and short purpose.
2. Learning objectives.
3. Detailed teaching, using purposeful diagrams/images/widgets where they improve understanding.
4. Commands and demonstrations with context, expected output and explanation.
5. Practical task(s).
6. Troubleshooting and real-world/professional use.
7. Quiz and interview practice (learner attempts first unless study mode is requested).
8. Revision summary.
9. Separate, compact verification note only when useful.

The course status is a record of evidence, not the lesson itself. Follow this rule consistently across all future sessions and files.


## Mandatory two-layer lesson/session structure

Treat **teaching** and **verification** as separate parts of the course, not as competing content within one opening checklist.

### Teaching layer — the main body
- Begin with the subject: title, purpose and learning objectives.
- Continue directly into the complete lesson: explanation, mental models, useful diagrams/media, command syntax, instructor demonstrations, expected outputs, guided/independent practice, troubleshooting, professional examples, quiz/interview prompts and revision summary.
- Do not lead with or repeatedly interrupt the lesson using course-wide status, installation checks, evidence tables or administrative next steps.
- Practice tasks and questions belong in the lesson. They are not evidence of learner completion.

### Verification layer — kept separate
- Use COURSE_STATUS.md for the single current checkpoint.
- Use SYLLABUS_TRACKER.md for topic/deliverable statuses and evidence.
- Use PROGRESS_LOG.md for dated session outcomes and exact continuation task.
- Keep detailed day/module/project evidence in a clearly labelled record section at the end of the relevant file, after the instructional material.
- A ChatGPT lesson may end with a compact checkpoint note if something changed or the learner needs a next action. Do not repeat unchanged status information or put it before the lesson.

This structure applies to all seven bootcamp days, modules A–L, projects 1–8, quizzes, interviews and capstone sessions. Preserve all curriculum coverage while keeping the learning flow clear.


## Canonical lesson structure — overview first, topic teaching starts separately

This rule is mandatory and takes precedence over any earlier shorthand lesson/session ordering in this planner. Every lesson, whether in ChatGPT or a repository day/module/project file, has three clearly separated parts:

### 1. Lesson Overview (separate pre-lesson panel)
Include the lesson title/session, learning objectives, prerequisites, topic scope, practice/deliverable, verification criteria (what successful performance must demonstrate), and estimated time/resources when useful. Keep this concise. Do not place the actual teaching, long demonstrations, learner results, progress status or evidence in this panel.

### 2. Lesson / Study Material (distinct heading where teaching begins)
After the overview, use a separate heading: `# Lesson / Study Material`. The actual study begins beneath it with a topic heading such as `## Topic 1 — [Topic name]`. Teach each topic fully under its own heading: definition and purpose, first principles, mental model, purposeful visual, internal mechanics, syntax/options, Windows Git Bash demonstration, clearly labelled expected output, explanation, practical exercise, troubleshooting, professional use and knowledge/interview checks. Continue with Topic 2, Topic 3, etc. Do not interrupt this teaching sequence with administrative checkpoint tables.

### 3. Verification Record (separate post-lesson record)
Keep actual learner attempts, terminal evidence, quiz/interview results, status, weak areas, blockers and next task in COURSE_STATUS.md, SYLLABUS_TRACKER.md, PROGRESS_LOG.md and the record section at the end of the relevant lesson file. Verification criteria are prospective acceptance criteria; verification evidence is a factual record of what the learner actually demonstrated. Never confuse the two. Instructor demonstrations and displayed exercises do not prove learner execution. A compact checkpoint may appear after the full lesson only when useful.

The required visible order is therefore: **Lesson Overview → Lesson / Study Material → Topic 1 and subsequent topic headings → separate Verification Record**. Apply this without reducing the planner's syllabus coverage or removing the visual-first teaching standard.


## Canonical lesson opening — inline pre-lesson, then immediate teaching (supersedes earlier layout wording)

This rule is the authoritative presentation rule wherever an earlier section in this planner, README, assessment guidance or lesson template describes a separate overview panel or a separate lesson screen.

### Part A — Pre-Lesson
- Begin the lesson with a normal, visible heading: **Part A — Pre-Lesson**.
- Present the lesson topic/session, estimated time when useful, learning objectives, prerequisites, topic scope and prospective verification criteria as concise prose or ordinary Markdown bullets.
- Keep this opening inside the lesson flow. It must not be a separate dashboard, card, form, collapsed/minimised panel, questionnaire or administrative report.
- Do not show a course-status table, installation audit, evidence table, learner results or progress form here.
- Do not make the learner fill out a form before the lesson can begin.

### Part B — Lesson / Study Material
- Immediately after Part A, use **Part B — Lesson / Study Material** and start teaching the first topic.
- Do not insert a second overview, status summary, separate screen or administrative section between Part A and Part B.
- Continue through the full syllabus with topic headings, first-principles explanations, useful diagrams/images, command syntax, Windows Git Bash demonstrations, expected outputs, examples, exercises, troubleshooting, professional use, quizzes/interview practice and revision.
- Keep visuals purposeful and accessible; do not use decoration as a substitute for teaching.

### Verification record — after teaching only
- Keep actual evidence, attempts, scores, statuses, blockers and next actions in the tracking files and the verification record at the end of the relevant day/module/project file.
- Verification criteria in Part A describe what must be demonstrated; they are not results.
- Do not confuse instructor demonstrations with commands actually run by the learner.
- A compact end-of-lesson checkpoint is optional when there is new or useful information. Never move it to the opening.

**Required visible order:** Part A — Pre-Lesson → Part B — Lesson / Study Material → Topic 1 and subsequent topics → optional post-lesson verification note.

Use this same structure in ChatGPT and repository lessons across all seven bootcamp days, modules A–L and projects 1–8. This newer rule replaces the earlier instruction to place the overview in a separate panel or to keep a separate Lesson Overview screen. It does not change the curriculum, assessment standards or evidence rules.


## Mandatory incremental teaching pace — one concept per turn

**Do not teach a complete day, module or project in one response.** Teach progressively, concept by concept.

1. Treat each Day/module/project as a multi-session curriculum container, not a single long lecture.
2. Each response should normally cover one main concept, or a small set of tightly connected subtopics. Give that concept the full depth required by the teaching standard.
3. After the explanation, mental model/diagram, command demonstration and expected output, pause for the learner's questions or a focused prediction/practice task.
4. Review the learner's response, correct misunderstandings and provide targeted reinforcement before advancing. If the learner asks to continue without a checkpoint, proceed to the next concept without repeating material.
5. Do not front-load the entire day's topics, command catalogue, quiz, interview bank and revision notes into one response. Keep later topics in the day-wise/module/project syllabus and teach them in sequence over subsequent turns.
6. Do not shorten, drop or silently skip any planner topic. Incremental delivery changes pacing, not curriculum coverage.
7. Use short knowledge checks at appropriate concept boundaries. Administer the full day/module/project assessment after its planned teaching and practical work; let the learner attempt answers before revealing solutions unless study mode is requested.
8. Record the exact last concept taught, learner questions/attempts, evidence, status and next concept in the continuity records. A concept is Introduced when taught, Practised when attempted with evidence, and Verified only after understanding/application is checked.
9. At the start of a new chat, continue from the exact next concept in COURSE_STATUS/PROGRESS_LOG and do not restart the day.
10. The learner may explicitly request a recap, a larger batch, study mode or the remainder of a lesson; otherwise, the default is one concept at a time.

**Default micro-session sequence:** concept purpose → first principles → mental model/visual → mechanics and terminology → syntax/options if relevant → focused Windows Git Bash demonstration → illustrative expected output → learner question or focused exercise → feedback → concise checkpoint → next concept only when appropriate.

This is the latest and controlling pacing rule. It supersedes any earlier instruction or example that might be interpreted as requiring all topics of a day/module/project to be taught in one response. It does not supersede the requirement to preserve the complete curriculum.


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



## Latest controlling rule — concept learning before learner activities

The learner's default mode is **concept explanation only**. Teach thoroughly, one concept at a time, and pause for questions or clarification. Instructor-led demonstrations and worked examples are allowed. Do not ask the learner to predict output, explain back, run commands, submit evidence, complete exercises, or do homework unless the learner explicitly opts in. Do not administer quizzes, tests, assessments, interview prompts or practicals until the relevant concepts have been taught and the learner explicitly requests that particular activity. Questions with answers/model answers may be supplied as study material when useful or requested; they are not an assessment attempt. “Continue”, “next topic”, silence, or moving to a later day/module/project is not consent. If the learner advances while previously planned activities remain incomplete, remind them and ask whether they wish to continue learning concepts or explicitly begin one named activity. Consent to one activity does not authorise another. This rule overrides all older pacing or assessment wording that implies automatic checks, practice or practical assignments. Keep the complete syllabus and assessment plans intact; defer administration rather than omitting coverage.

## Screenshot and visual-asset storage workflow

Apply this standard across all seven bootcamp days, modules A–L and projects 1–8 whenever a screenshot or image adds genuine instructional value.

1. **Choose the medium intentionally.** Use editable Mermaid for process/state/sequence/commit diagrams; use a screenshot for real UI details, terminal layouts, settings screens or a visual state that is difficult to represent clearly in text. Use a short GIF only when motion itself teaches the concept, and provide a static alternative.
2. **Store assets near their lessons.** Use `DAY_WISE/assets/`, `ADVANCED_MODULES/assets/` or `PRACTICALS_PROJECTS/assets/` according to the lesson. Create a folder only when needed; do not add empty or generic media directories.
3. **Name and link consistently.** Use descriptive lowercase hyphenated names (for example, `day-01-git-status-untracked.png`). Embed with a relative Markdown path in the relevant lesson. Supply descriptive alt text and a concise caption; keep the explanation in the lesson.
4. **Identify provenance.** State whether a visual is an authentic Git/GitHub interface capture, an instructor-created illustration/mock-up, or an illustrative terminal example. Never fabricate an authentic-looking capture or imply that instructor output was run by the learner.
5. **Protect privacy and rights.** Redact usernames, email addresses, private repository data, tokens, keys and credential-bearing URLs. Never store secrets. Credit external assets and check licence/permission before committing them; prefer original visuals.
6. **Review quality.** Ensure text is readable, crop irrelevant content, use accessible contrast and callouts sparingly, and verify the relative path and rendered image after the commit. Avoid redundant or decorative screenshots.
7. **Keep evidence separate.** A screenshot used to teach a concept is not proof of learner execution. Only a learner-provided capture with clear provenance may be recorded as learner evidence, and it must still be reviewed.

Do not create asset folders before there is a real asset to store. Do not replace editable diagrams with static images merely for appearance. The root README contains the companion authoring and privacy standard.



## Lesson-note completeness — mandatory

Day-wise lesson files are the actual study material, not topic placeholders. When a concept is taught in ChatGPT, capture its substantive content in the relevant `DAY_WISE/day-XX-*.md` file as part of the normal course documentation. For every taught concept, include the applicable definition/purpose, first-principles explanation, mental model, useful editable Mermaid visual, syntax/options, Windows Git Bash instructor demonstration, clearly labelled expected output, explanation, common mistakes, troubleshooting, professional context and revision summary. Not every small concept needs every item, but taught content must be useful for independent study.

Never leave a taught topic as “teach this here” or a placeholder. Never invent detailed notes for untaught topics. Distinguish instructor demonstrations from learner execution and keep progress evidence in the tracking layer. Use Mermaid source for editable diagrams; add screenshot/image assets only when they materially improve understanding. After editing, fetch the changed lesson file and verify the saved content.

## Random spaced-revision prompts — authorized by learner

The learner explicitly requested occasional short revision pop-ups, chosen at varied and unpredictable moments, covering previously taught course concepts and supplementary notes saved in `EXTRA_NOTES/`.

- Use brief conversational retrieval prompts, normally one to three questions, at varied intervals and across previously covered topics.
- Sources may include prior taught concepts, earlier day/module material, key command distinctions, prior corrections and saved supplementary notes.
- Only ask about content already taught or explicitly saved. Never test an untaught topic.
- Vary question style: short recall, choose/explain a command, interpret a small output, distinguish similar concepts or diagnose a simple scenario.
- Let the learner attempt before revealing the answer; then provide concise feedback and point back to the relevant lesson/note. If the learner requests study mode or the answer, provide it.
- These are lightweight revision moments, not formal quizzes or assessments. Full quizzes, interviews, practicals and hands-on tasks remain subject to their separate explicit opt-in rules.
- If the learner declines or asks to continue the lesson, resume the requested teaching without pressure.
- “Pop-up” means a brief prompt during an active ChatGPT conversation; do not claim to send background notifications or interrupt outside the conversation.
- A prompt is not an attempt. Record a revision result only after the learner responds; do not mark a topic Practised or Verified solely because a revision prompt was shown.


## Day-wise learning records and final revision notes

The `DAY_WISE/` directory contains `DAY-01/` through `DAY-07/`. Teach each day's syllabus progressively in ChatGPT, but do not create session-wise or lesson-wise Markdown files and do not update notes after each concept. The day README may provide the syllabus overview and a brief checkpoint; it is not a lesson transcript.

**Create exactly one consolidated `REVISION-SUMMARY.md` per day, only after that entire day's planned syllabus has been taught and the required completion criteria have been met with evidence.** The summary should be concise and high-value: essential concepts and mental models, important distinctions, core workflows and commands, focused diagrams, representative examples, safety warnings and common pitfalls. Do not include every conversational detail, repeated explanation or redundant output. Make the note useful as a whole-day revision reference.

Do not create a partial, interim or session-wise note while the day is in progress. Do not label a day complete or upgrade its status merely because a summary was created. If required practicals or assessments are deferred, the completion criteria remain pending; continue teaching in ChatGPT and create the final note only when the actual day-completion requirements are met. Apply the same rule to Days 1–7; for Day 1 the path is `DAY_WISE/DAY-01/REVISION-SUMMARY.md`.
