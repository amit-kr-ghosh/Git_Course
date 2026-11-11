# Git & GitHub Command Reference

Track commands actually taught and practised. Record syntax, purpose, preconditions, local/remote effects, risk and a verified example.

| Command / family | Purpose | Status | Example / notes |
|---|---|---|---|
| git --version | Check installed Git version | Not started | Day 1 Topic 6 |
| git config | Configure and inspect identity/settings | Not started | Day 1 Topic 6; learner configuration not confirmed |
| git init / clone | Create or copy a repository | Not started | Day 1 Topic 7 |
| git status / diff / log / show | Inspect state and history | Introduced | Demonstrated conceptually in Day 1 Topics 4–5; no learner execution evidenced |
| git add / commit | Stage and record changes | Introduced | Their roles in the four-area workflow were introduced conceptually; no learner execution evidenced |
| git restore / reset / revert / clean | Undo or clean changes; understand risks | Not started | |
| git branch / switch / merge / rebase | Branch and integrate work | Introduced | Branch references and HEAD introduced conceptually in Day 1 Topic 5; command practice not evidenced |
| git remote / fetch / pull / push | Synchronise with remotes | Introduced | Roles of local and remote repositories and push/fetch/pull were introduced conceptually; commands not yet taught |
| git stash / tag / cherry-pick / reflog | Manage temporary work, releases and history | Not started | |
| GitHub CLI / Actions | Platform automation | Not started | |
| Plumbing / maintenance | Advanced object and repository operations | Introduced | `git cat-file` and `git hash-object` demonstrated conceptually in Day 1 Topic 5; no learner execution evidenced |

Add entries as the curriculum advances. Verify syntax against installed Git version and official documentation.


## Day 1 Topic 5 — commands introduced

| Command | Purpose | Provenance |
|---|---|---|
| `git diff` | Compare Working Tree with Index | Instructor demonstration |
| `git diff --staged` | Compare Index with HEAD | Instructor demonstration |
| `git show --stat HEAD` | Inspect commit summary | Instructor demonstration |
| `git log --oneline --graph --decorate --all` | Inspect commit graph and refs | Instructor demonstration |
| `git cat-file -t` / `-p` | Inspect Git object type/content | Instructor demonstration |
| `git hash-object` / `-w` | Calculate/store object content | Instructor demonstration |

No learner execution has been reported.


## Day 1 Topic 6 — installation and configuration commands introduced

| Command | Purpose | Provenance |
|---|---|---|
| `git --version` | Display installed Git version | Instructor demonstration |
| `git config --global user.name "Your Name"` | Set global commit identity name | Instructor demonstration |
| `git config --global user.email "you@example.com"` | Set global commit identity email | Instructor demonstration |
| `git config --global init.defaultBranch main` | Set default initial branch for new repositories | Instructor demonstration |
| `git config --global core.editor "code --wait"` | Configure editor | Instructor demonstration |
| `git config --global core.autocrlf true` | Configure common Windows line-ending conversion | Instructor demonstration |
| `git config --list` | Display effective configuration | Instructor demonstration |
| `git config --show-origin --list` | Display configuration values and their origin | Instructor demonstration |
| `git config --global --list` / `git config --local --list` | Inspect scope-specific configuration | Instructor demonstration |

No learner execution has been reported. Git installation and identity/configuration remain unconfirmed.
