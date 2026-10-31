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
