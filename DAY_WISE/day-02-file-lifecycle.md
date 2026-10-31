# Day 2 — File lifecycle, inspection and safe undo

## Syllabus
- Repository state lifecycle
- tracked/untracked/modified/staged/deleted/renamed files
- status short/porcelain
- diff, diff --staged/--cached, diff HEAD
- show
- log formats
- commit anatomy and messages
- add file/directory/-A/interactive staging
- .gitignore patterns/negation/already-tracked caveat
- restore working-tree and staged changes
- reset soft/mixed/hard
- revert
- amend
- clean preview and risks.

## Practical deliverable
In a disposable repository, create, stage, unstage, modify, discard, amend and revert changes; document before/after state.

## Interview focus
Reset vs revert vs restore; diff variants; partial staging; ignoring tracked files.

## Quiz focus
Status interpretation, staged/unstaged diffs, ignore rules and safe undo selection.

## Session records
| Session/date | Topics covered | Status | Evidence | Next step |
|---|---|---|---|---|
| | | Not started | | |

## Commands demonstrated vs actually run
- Demonstrated:
- Run by learner:
- Output/evidence:

## Quiz and interview outcome
- Quiz score/gaps:
- Interview questions and answers:
- Remediation / revision:

## Continuation checkpoint
- Verified topics:
- Incomplete topics:
- Blockers:
- Exact next topic:

Do not mark this day verified until the syllabus, practical, quiz and interview preparation have been reviewed.

## Visual guide — inspect before you undo

### File lifecycle

```mermaid
flowchart TD
    U["Untracked file"] -->|"git add"| S["Staged change"]
    S -->|"git commit"| C["Committed snapshot"]
    C -->|"edit"| M["Modified working file"]
    M -->|"git add"| S
    M -->|"git restore file"| C
    S -->|"git restore --staged file"| M
    classDef pending fill:#fef3c7,stroke:#d97706,color:#78350f,stroke-width:2px
    classDef saved fill:#dcfce7,stroke:#16a34a,color:#14532d,stroke-width:2px
    classDef risk fill:#fee2e2,stroke:#dc2626,color:#7f1d1d,stroke-width:2px
    class U,S,M pending
    class C saved
```

### Which diff am I inspecting?

| Command | Comparison | Use it to answer |
|---|---|---|
| `git diff` | Working tree vs index | What have I edited but not staged? |
| `git diff --staged` | Index vs last commit | What will the next commit contain? |
| `git diff HEAD` | Working tree + index vs HEAD | What differs from the last commit overall? |

### Safe undo decision path

```mermaid
flowchart TD
    Q{"Where is the unwanted change?"}
    Q -->|"Unstaged working edit"| R["git restore -- file"]
    Q -->|"Staged, not committed"| U["git restore --staged -- file"]
    Q -->|"Already committed"| V["Consider git revert"]
    Q -->|"Need to move local branch pointer"| X["Understand reset modes first"]
    classDef safe fill:#dcfce7,stroke:#16a34a,color:#14532d
    classDef caution fill:#fee2e2,stroke:#dc2626,color:#7f1d1d
    class R,U,V safe
    class X caution
```

> [!WARNING]
> `git reset --hard` and `git clean` can permanently discard uncommitted work. Preview and practise only in a disposable repository.
