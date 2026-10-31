# Day 1 — Foundations, mental model and first repository

## Syllabus
- Version control and why it exists
- manual backups vs version history
- local, centralised and distributed version control
- Git's distributed nature
- Git history at a high level
- Git vs GitHub
- hosting platforms
- repository, working directory, index/staging area, local and remote repositories
- tracked/untracked/modified/staged/committed states
- commit, parent, hash/object ID, branch and HEAD
- install Git for Windows and verify git --version
- configure user.name/user.email and inspect config scopes
- create directory, git init, README, status/add/commit/log
- make second change and inspect git diff.

## Practical deliverable
Create git-learning-journey with README, day1 notes and commands file; make at least two meaningful commits.

## Interview focus
Define Git, DVCS, repository, commit and staging area; explain Git vs GitHub.

## Quiz focus
Definitions, repository states, command purpose and first-repository workflow.

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

## Visual guide — how Git remembers work

### The four places to understand

```mermaid
flowchart LR
    W["📝 Working tree<br/>edit files"] -->|"git add"| I["🟨 Index / staging<br/>choose snapshot"]
    I -->|"git commit"| L["🟩 Local repository<br/>save commit"]
    L <-->|"fetch / pull / push"| R["🟪 Remote repository<br/>share and sync"]
    classDef work fill:#dbeafe,stroke:#2563eb,color:#172554,stroke-width:2px
    classDef index fill:#fef3c7,stroke:#d97706,color:#78350f,stroke-width:2px
    classDef local fill:#dcfce7,stroke:#16a34a,color:#14532d,stroke-width:2px
    classDef remote fill:#f3e8ff,stroke:#9333ea,color:#581c87,stroke-width:2px
    class W work
    class I index
    class L local
    class R remote
```

### File-state transition

```mermaid
stateDiagram-v2
    [*] --> Untracked
    Untracked --> Staged: git add
    Staged --> Committed: git commit
    Committed --> Modified: edit tracked file
    Modified --> Staged: git add
    Staged --> Modified: edit after staging
```

| Visual cue | Meaning |
|---|---|
| 🔵 Blue | Work is being edited |
| 🟡 Amber | Change is staged for the next commit |
| 🟢 Green | Snapshot is committed |
| 🟣 Purple | Work is shared with a remote |

> [!TIP]
> A commit records the staged snapshot, not every unsaved edit in the working directory.

### First repository — command sequence

```mermaid
flowchart TD
    A["Create project folder"] --> B["git init"]
    B --> C["Create README.md"]
    C --> D["git status"]
    D --> E["git add README.md"]
    E --> F["git commit -m \"Initial commit\""]
    F --> G["git log --oneline"]
    classDef start fill:#dbeafe,stroke:#2563eb,color:#172554
    classDef action fill:#dcfce7,stroke:#16a34a,color:#14532d
    classDef inspect fill:#fef3c7,stroke:#d97706,color:#78350f
    class A,B,C start
    class E,F action
    class D,G inspect
```

