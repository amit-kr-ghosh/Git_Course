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

## Teaching standard
Teach from first principles. Explain purpose, terminology, mental model, syntax, flags, preconditions, local/remote effects, expected output and verification. Use visuals only when useful. Follow explain → demonstrate → guided practice → independent challenge → verify → knowledge check. Never claim commands ran on the learner's machine.

## Assessments
Daily quizzes and interview preparation begin Day 1. Quizzes include recall, command choice, output prediction, comparisons, troubleshooting and practical verification. Do not reveal answers before an attempt. Explain missed answers and map gaps to syllabus topics. Quiz scores alone do not prove practical mastery. Interview reference notes place each question immediately before its answer; mock interviews include scoring and feedback.

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
