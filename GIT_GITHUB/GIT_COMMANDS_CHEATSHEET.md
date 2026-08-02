# Git Commands Cheat Sheet

A quick, categorized reference for the Git commands you'll actually use — from everyday staging and committing to branching, remotes, and history rewriting. Anything in `<angle brackets>` is a placeholder you replace with your own value.

## 📚 Table of Contents

- [⚡ Quick Reference: Most-Used Commands](#quick-reference-most-used-commands)
- [Configuration](#configuration)
- [Creating & Cloning Repositories](#creating--cloning-repositories)
- [Staging & Committing](#staging--committing)
- [Branching](#branching)
- [Merging & Rebasing](#merging--rebasing)
- [Remote Repositories](#remote-repositories)
- [Inspecting & Comparing](#inspecting--comparing)
- [Undoing Changes](#undoing-changes)
- [Stashing](#stashing)
- [Tags](#tags)
- [History Search & Debugging](#history-search--debugging)
- [Ignoring Files (`.gitignore`)](#ignoring-files-gitignore)
- [Useful Aliases](#useful-aliases)
- [Bonus: GitHub CLI (`gh`)](#bonus-github-cli-gh)

---

<a id="quick-reference-most-used-commands"></a>
## ⚡ Quick Reference: Most-Used Commands

The 90% of Git you'll use on any given day.

| Command | What it does |
|---|---|
| `git status` | Show what's changed, staged, or untracked |
| `git add <file>` | Stage a file |
| `git add .` | Stage everything in the current directory |
| `git commit -m "message"` | Commit staged changes |
| `git push` | Push commits to the remote |
| `git pull` | Fetch and merge from the remote |
| `git branch` | List local branches |
| `git switch -c <branch>` | Create and switch to a new branch |
| `git merge <branch>` | Merge a branch into the current one |
| `git log --oneline` | Compact commit history |
| `git diff` | Show unstaged changes |
| `git stash` | Temporarily shelve uncommitted changes |

---

<a id="configuration"></a>
## Configuration

| Command | What it does |
|---|---|
| `git config --global user.name "Your Name"` | Set your commit author name |
| `git config --global user.email "you@example.com"` | Set your commit author email |
| `git config --global init.defaultBranch main` | Set the default branch name for new repos |
| `git config --global core.editor "code --wait"` | Set your default Git editor |
| `git config --list` | Show all active config settings |
| `git config --get <key>` | Show the value of one setting, e.g. `remote.origin.url` |
| `git config --global --edit` | Open your global config file directly |

---

<a id="creating--cloning-repositories"></a>
## Creating & Cloning Repositories

| Command | What it does |
|---|---|
| `git init` | Turn the current directory into a new Git repo |
| `git init <dir>` | Create a new repo in a new directory |
| `git clone <url>` | Clone a remote repo into a new directory |
| `git clone <url> <dir>` | Clone into a specifically named directory |
| `git clone --depth 1 <url>` | Shallow clone — only the latest commit, no full history |
| `git clone --branch <branch> <url>` | Clone and check out a specific branch |

---

<a id="staging--committing"></a>
## Staging & Committing

| Command | What it does |
|---|---|
| `git add <file>` | Stage a specific file |
| `git add .` | Stage all changes in and below the current directory |
| `git add -A` | Stage all changes in the whole repo, including deletions |
| `git add -p` | Interactively stage specific hunks within a file |
| `git status` | Show the working directory and staging area state |
| `git status -s` | Short-format status output |
| `git commit -m "message"` | Commit staged changes with a message |
| `git commit -am "message"` | Stage all tracked file changes and commit in one step |
| `git commit --amend` | Edit the most recent commit's message and/or content |
| `git commit --amend --no-edit` | Add staged changes to the last commit, keep its message |
| `git rm <file>` | Delete a file and stage the deletion |
| `git rm --cached <file>` | Stop tracking a file, but keep it on disk |
| `git mv <old> <new>` | Rename/move a file and stage the change |

---

<a id="branching"></a>
## Branching

| Command | What it does |
|---|---|
| `git branch` | List local branches |
| `git branch -a` | List local and remote-tracking branches |
| `git branch -r` | List only remote-tracking branches |
| `git branch <name>` | Create a new branch (doesn't switch to it) |
| `git branch -d <name>` | Delete a branch (only if already merged) |
| `git branch -D <name>` | Force-delete a branch, merged or not |
| `git branch -m <old> <new>` | Rename a branch |
| `git checkout <branch>` | Switch to an existing branch |
| `git checkout -b <branch>` | Create a new branch and switch to it |
| `git switch <branch>` | Switch to an existing branch (modern syntax) |
| `git switch -c <branch>` | Create a new branch and switch to it (modern syntax) |

---

<a id="merging--rebasing"></a>
## Merging & Rebasing

| Command | What it does |
|---|---|
| `git merge <branch>` | Merge `<branch>` into your current branch |
| `git merge --no-ff <branch>` | Merge and always create a merge commit, even if fast-forward is possible |
| `git merge --abort` | Cancel an in-progress merge with conflicts |
| `git rebase <branch>` | Replay your current branch's commits on top of `<branch>` |
| `git rebase -i HEAD~<n>` | Interactively edit/squash/reorder the last `n` commits |
| `git rebase --continue` | Resume a rebase after resolving a conflict |
| `git rebase --abort` | Cancel an in-progress rebase entirely |
| `git rebase --skip` | Skip the current commit during a rebase |
| `git cherry-pick <hash>` | Apply a specific commit from another branch onto the current one |

---

<a id="remote-repositories"></a>
## Remote Repositories

| Command | What it does |
|---|---|
| `git remote -v` | List configured remotes and their URLs |
| `git remote add <name> <url>` | Add a new remote |
| `git remote remove <name>` | Remove a remote |
| `git remote set-url origin <url>` | Change an existing remote's URL |
| `git fetch` | Download new commits/branches from the default remote |
| `git fetch --all` | Fetch from every configured remote |
| `git pull` | Fetch and merge from the tracked remote branch |
| `git pull --rebase` | Fetch and rebase instead of merge |
| `git push` | Push commits to the tracked remote branch |
| `git push -u origin <branch>` | Push and set up tracking for a branch |
| `git push origin --delete <branch>` | Delete a branch on the remote |
| `git push --force` | Force-push, overwriting the remote's history |
| `git push --force-with-lease` | Safer force-push — fails if the remote has new commits you haven't seen |
| `git push --tags` | Push all local tags to the remote |

---

<a id="inspecting--comparing"></a>
## Inspecting & Comparing

| Command | What it does |
|---|---|
| `git log` | Full commit history |
| `git log --oneline` | One line per commit |
| `git log --graph --oneline --all` | Visual branch/merge graph of all branches |
| `git log -p` | Show the full diff for each commit |
| `git log -- <file>` | Show only commits that touched a specific file |
| `git diff` | Show unstaged changes vs. the last commit |
| `git diff --staged` | Show staged changes vs. the last commit |
| `git diff <branch1>..<branch2>` | Show differences between two branches |
| `git show <hash>` | Show the details and diff of a specific commit |
| `git blame <file>` | Show who last changed each line of a file, and in which commit |

---

<a id="undoing-changes"></a>
## Undoing Changes

| Command | What it does |
|---|---|
| `git restore <file>` | Discard unstaged changes to a file |
| `git restore --staged <file>` | Unstage a file, keeping its edits |
| `git reset <file>` | Older equivalent of `restore --staged` |
| `git reset --soft HEAD~1` | Undo the last commit, keep changes staged |
| `git reset --mixed HEAD~1` | Undo the last commit, keep changes unstaged (default) |
| `git reset --hard HEAD~1` | Undo the last commit and discard its changes entirely |
| `git revert <hash>` | Create a new commit that undoes a specific past commit |
| `git clean -n` | Preview which untracked files would be deleted |
| `git clean -fd` | Delete untracked files and directories |

---

<a id="stashing"></a>
## Stashing

| Command | What it does |
|---|---|
| `git stash` | Shelve all uncommitted changes |
| `git stash push -m "message"` | Stash with a descriptive message |
| `git stash push -p` | Interactively stash specific hunks only |
| `git stash list` | List all stashes |
| `git stash pop` | Reapply the most recent stash and remove it from the list |
| `git stash apply` | Reapply the most recent stash, keep it in the list |
| `git stash show -p` | Show the diff contained in the latest stash |
| `git stash drop` | Delete the most recent stash without applying it |
| `git stash clear` | Delete all stashes |

---

<a id="tags"></a>
## Tags

| Command | What it does |
|---|---|
| `git tag` | List all tags |
| `git tag <name>` | Create a lightweight tag on the current commit |
| `git tag -a <name> -m "message"` | Create an annotated tag with a message |
| `git tag -d <name>` | Delete a local tag |
| `git push origin <name>` | Push a single tag to the remote |
| `git push origin --tags` | Push all local tags to the remote |
| `git push origin --delete <name>` | Delete a tag on the remote |

---

<a id="history-search--debugging"></a>
## History Search & Debugging

| Command | What it does |
|---|---|
| `git bisect start` | Begin a binary search for the commit that introduced a bug |
| `git bisect bad` | Mark the current commit as broken |
| `git bisect good <hash>` | Mark a known-working commit |
| `git bisect reset` | End the bisect session and return to your original branch |
| `git log -S"<string>"` | Find commits that added or removed a specific string |
| `git log --author="<name>"` | Filter commit history by author |
| `git reflog` | Show a local log of everywhere `HEAD` has pointed — useful for recovering "lost" commits |

---

<a id="ignoring-files-gitignore"></a>
## Ignoring Files (`.gitignore`)

Common patterns to drop into a `.gitignore` file:

```gitignore
# Dependencies
node_modules/
vendor/

# Build output
dist/
build/
*.log

# Environment & secrets
.env
.env.local

# OS/editor files
.DS_Store
.vscode/
*.swp
```

| Pattern | Matches |
|---|---|
| `file.txt` | That exact file, anywhere it appears |
| `*.log` | Any file ending in `.log` |
| `build/` | A directory named `build`, anywhere |
| `/build` | Only a `build` directory at the repo root |
| `!important.log` | Un-ignores a file that a broader pattern above would otherwise exclude |

---

<a id="useful-aliases"></a>
## Useful Aliases

Add these once, then use the short version forever.

```bash
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.st status
git config --global alias.cm "commit -m"
git config --global alias.unstage "restore --staged"
git config --global alias.lg "log --graph --oneline --all --decorate"
```

| Alias | Expands to |
|---|---|
| `git co <branch>` | `git checkout <branch>` |
| `git br` | `git branch` |
| `git st` | `git status` |
| `git cm "msg"` | `git commit -m "msg"` |
| `git unstage <file>` | `git restore --staged <file>` |
| `git lg` | `git log --graph --oneline --all --decorate` |

---

<a id="bonus-github-cli-gh"></a>
## Bonus: GitHub CLI (`gh`)

Not core Git, but worth knowing if you work on GitHub daily.

| Command | What it does |
|---|---|
| `gh repo clone <owner>/<repo>` | Clone a GitHub repo |
| `gh pr create` | Open a pull request from the current branch |
| `gh pr checkout <number>` | Check out a pull request locally |
| `gh pr view --web` | Open the current branch's PR in the browser |
| `gh pr merge` | Merge a pull request from the terminal |
| `gh issue create` | Create a new issue |
| `gh repo view --web` | Open the current repo on GitHub in the browser |

---

Keep this handy — `Ctrl+F` (or `Cmd+F`) any command name to jump straight to it. 🚀
