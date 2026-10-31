# Day 3 — Branching, merging and conflicts

## Syllabus
- Why branches exist
- branch pointers/commit graph
- branch list/create/delete/rename
- upstream tracking
- switch and legacy checkout
- switch -c
- detached HEAD
- feature branch workflow
- fast-forward vs three-way merge
- merge commit
- conflict causes/markers/ours/theirs
- manual resolution
- status/add/complete/abort
- merge options/strategies
- branch cleanup
- GitHub Flow, Git Flow and trunk-based development.

## Practical deliverable
Create two feature branches that change the same file; create and resolve a conflict; document commit graph.

## Interview focus
Branch pointer, HEAD, fast-forward, three-way merge and conflict resolution.

## Quiz focus
Branch operations, merge outcomes, conflict markers and safe branch cleanup.

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

## Visual guide — branches are movable names for commits

### Feature branch and merge

```mermaid
gitGraph
   commit id: "main: start"
   branch feature
   commit id: "feature work"
   checkout main
   commit id: "main update"
   merge feature id: "merge feature"
```

### Two common merge outcomes

```mermaid
flowchart TD
    A["Are the branch histories divergent?"]
    A -->|"No: target is an ancestor"| B["Fast-forward<br/>move branch pointer"]
    A -->|"Yes: both have new commits"| C["Three-way merge<br/>create merge commit (usually)"]
    classDef fast fill:#dcfce7,stroke:#16a34a,color:#14532d
    classDef three fill:#dbeafe,stroke:#2563eb,color:#172554
    class B fast
    class C three
```

### Conflict resolution loop

```mermaid
flowchart LR
    M["git merge"] --> C{"Conflict?"}
    C -->|"No"| D["Merge completes"]
    C -->|"Yes"| E["Edit conflicted file"]
    E --> F["git add resolved-file"]
    F --> G["git commit or finish merge"]
    classDef decision fill:#fef3c7,stroke:#d97706,color:#78350f
    classDef resolve fill:#dbeafe,stroke:#2563eb,color:#172554
    class C decision
    class E,F,G resolve
```

> [!TIP]
> A branch is not a separate copy of your entire project. It is a movable reference to a commit.
