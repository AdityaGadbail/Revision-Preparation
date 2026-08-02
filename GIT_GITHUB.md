# Git & GitHub Interview Questions & Answers — Complete Revision Guide

A complete, structured collection of Git and GitHub interview questions — from core version-control fundamentals to branching, merging, rebasing, internals, and GitHub-specific collaboration features — with clear answers and command examples where they help. Built to be your one-stop revision resource the night before an interview or test.

## 📚 Table of Contents

- [🔥 Most Asked / Tricky Questions](#-most-asked--tricky-questions)
  - [What is the difference between Git and GitHub?](#what-is-the-difference-between-git-and-github)
  - [What is the difference between `git merge` and `git rebase`?](#what-is-the-difference-between-git-merge-and-git-rebase)
  - [What is the difference between `git fetch` and `git pull`?](#what-is-the-difference-between-git-fetch-and-git-pull)
  - [What is the difference between `git reset` and `git revert`?](#what-is-the-difference-between-git-reset-and-git-revert)
  - [What is a merge conflict, and when does it happen?](#what-is-a-merge-conflict-and-when-does-it-happen)
  - [What is the difference between a `git reset --soft`, `--mixed`, and `--hard`?](#what-is-the-difference-between-a-git-reset---soft---mixed-and---hard)
  - [What is a detached HEAD state?](#what-is-a-detached-head-state)
  - [What is the difference between `git branch -d` and `git branch -D`?](#what-is-the-difference-between-git-branch--d-and-git-branch--d)
  - [What does `git cherry-pick` do?](#what-does-git-cherry-pick-do)
  - [What is the difference between the working directory, staging area, and repository in Git?](#what-is-the-difference-between-the-working-directory-staging-area-and-repository-in-git)
  - [What is `.gitignore` used for?](#what-is-gitignore-used-for)
  - [What is the difference between a fork and a clone?](#what-is-the-difference-between-a-fork-and-a-clone)
  - [What happens when you run `git push` and someone else has already pushed conflicting commits?](#what-happens-when-you-run-git-push-and-someone-else-has-already-pushed-conflicting-commits)
  - [What is the difference between `git stash` and just committing work-in-progress changes?](#what-is-the-difference-between-git-stash-and-just-committing-work-in-progress-changes)
  - [What is a fast-forward merge?](#what-is-a-fast-forward-merge)
- [Git Basics](#git-basics)
  - [What is version control, and why is it important?](#what-is-version-control-and-why-is-it-important)
  - [What is the difference between a centralized and a distributed version control system?](#what-is-the-difference-between-a-centralized-and-a-distributed-version-control-system)
  - [How do you initialize a new Git repository?](#how-do-you-initialize-a-new-git-repository)
  - [What is the difference between `git add .` and `git add -A`?](#what-is-the-difference-between-git-add--and-git-add--a)
  - [What is the purpose of a commit message, and what makes a good one?](#what-is-the-purpose-of-a-commit-message-and-what-makes-a-good-one)
  - [What is the difference between `git status` and `git log`?](#what-is-the-difference-between-git-status-and-git-log)
  - [What does `git diff` show, and how does it change when you add `--staged`?](#what-does-git-diff-show-and-how-does-it-change-when-you-add---staged)
  - [What is a SHA (commit hash), and how is it generated?](#what-is-a-sha-commit-hash-and-how-is-it-generated)
  - [What is the difference between tracked, untracked, staged, and modified files?](#what-is-the-difference-between-tracked-untracked-staged-and-modified-files)
  - [What does `git clone` do?](#what-does-git-clone-do)
- [Committing & History](#committing--history)
  - [What does `git commit --amend` do?](#what-does-git-commit---amend-do)
  - [Why is it risky to amend or rebase commits that have already been pushed and shared with others?](#why-is-it-risky-to-amend-or-rebase-commits-that-have-already-been-pushed-and-shared-with-others)
  - [What is the difference between `git log` and `git log --oneline`?](#what-is-the-difference-between-git-log-and-git-log---oneline)
  - [How would you view the history of changes made to a specific file?](#how-would-you-view-the-history-of-changes-made-to-a-specific-file)
  - [What is `git blame` used for?](#what-is-git-blame-used-for)
  - [What is a squash commit, and why would you use one?](#what-is-a-squash-commit-and-why-would-you-use-one)
  - [What is the difference between `HEAD`, `HEAD~1`, and `HEAD^`?](#what-is-the-difference-between-head-head1-and-head)
  - [What is a tag in Git, and what's the difference between a lightweight and an annotated tag?](#what-is-a-tag-in-git-and-whats-the-difference-between-a-lightweight-and-an-annotated-tag)
  - [How would you find which commit introduced a bug?](#how-would-you-find-which-commit-introduced-a-bug)
  - [What information does a Git commit object actually store?](#what-information-does-a-git-commit-object-actually-store)
- [Branching](#branching)
  - [What is a branch in Git, conceptually?](#what-is-a-branch-in-git-conceptually)
  - [What command creates a new branch, and what's the difference between that and also switching to it?](#what-command-creates-a-new-branch-and-whats-the-difference-between-that-and-also-switching-to-it)
  - [What is the difference between `git checkout` and `git switch`?](#what-is-the-difference-between-git-checkout-and-git-switch)
  - [Why is branching considered cheap and fast in Git compared to some older version control systems?](#why-is-branching-considered-cheap-and-fast-in-git-compared-to-some-older-version-control-systems)
  - [What is the difference between a local branch and a remote-tracking branch?](#what-is-the-difference-between-a-local-branch-and-a-remote-tracking-branch)
  - [What does it mean for a local branch to "track" a remote branch?](#what-does-it-mean-for-a-local-branch-to-track-a-remote-branch)
  - [What is the difference between `git branch` and `git branch -a`?](#what-is-the-difference-between-git-branch-and-git-branch--a)
  - [How would you rename a branch, including one already pushed to a remote?](#how-would-you-rename-a-branch-including-one-already-pushed-to-a-remote)
  - [What is a feature branch, and why is the pattern commonly used?](#what-is-a-feature-branch-and-why-is-the-pattern-commonly-used)
  - [What happens to a branch pointer when you make a new commit while on that branch?](#what-happens-to-a-branch-pointer-when-you-make-a-new-commit-while-on-that-branch)
- [Merging & Rebasing](#merging--rebasing)
  - [What happens internally during a `git merge`?](#what-happens-internally-during-a-git-merge)
  - [What is a three-way merge?](#what-is-a-three-way-merge)
  - [What are the trade-offs between a merge-based workflow and a rebase-based workflow?](#what-are-the-trade-offs-between-a-merge-based-workflow-and-a-rebase-based-workflow)
  - [What does interactive rebase (`git rebase -i`) let you do?](#what-does-interactive-rebase-git-rebase--i-let-you-do)
  - [What is the "golden rule of rebasing"?](#what-is-the-golden-rule-of-rebasing)
  - [What is a merge conflict marker, and what do the different sections mean?](#what-is-a-merge-conflict-marker-and-what-do-the-different-sections-mean)
  - [What is `git rebase --continue`, `--abort`, and `--skip` used for?](#what-is-git-rebase---continue---abort-and---skip-used-for)
  - [What is a merge strategy, and what's the difference between the default strategy and squash merging?](#what-is-a-merge-strategy-and-whats-the-difference-between-the-default-strategy-and-squash-merging)
  - [What is `git rerere`, and what problem does it solve?](#what-is-git-rerere-and-what-problem-does-it-solve)
  - [When would you choose `git merge --no-ff` over a regular merge?](#when-would-you-choose-git-merge---no-ff-over-a-regular-merge)
- [Merge Conflicts](#merge-conflicts)
  - [What causes a merge conflict, specifically?](#what-causes-a-merge-conflict-specifically)
  - [What is the general process for resolving a merge conflict?](#what-is-the-general-process-for-resolving-a-merge-conflict)
  - [What is the difference between resolving a conflict during a `merge` versus during a `rebase`?](#what-is-the-difference-between-resolving-a-conflict-during-a-merge-versus-during-a-rebase)
  - [How can you use a merge tool to help resolve conflicts?](#how-can-you-use-a-merge-tool-to-help-resolve-conflicts)
  - [What does `git diff` show you while a merge conflict is unresolved?](#what-does-git-diff-show-you-while-a-merge-conflict-is-unresolved)
  - [How would you abort a merge that's gone wrong and return to the state before you started?](#how-would-you-abort-a-merge-thats-gone-wrong-and-return-to-the-state-before-you-started)
  - [How do binary file conflicts differ from text file conflicts, and how are they resolved?](#how-do-binary-file-conflicts-differ-from-text-file-conflicts-and-how-are-they-resolved)
  - [What are `--ours` and `--theirs` in the context of resolving a conflict, and does their meaning change between merge and rebase?](#what-are---ours-and---theirs-in-the-context-of-resolving-a-conflict-and-does-their-meaning-change-between-merge-and-rebase)
- [Remote Repositories](#remote-repositories)
  - [What is a remote in Git?](#what-is-a-remote-in-git)
  - [What is the difference between `git push` and `git push -u` (or `--set-upstream`)?](#what-is-the-difference-between-git-push-and-git-push--u-or---set-upstream)
  - [How do you add, view, and remove a remote?](#how-do-you-add-view-and-remove-a-remote)
  - [What is the difference between `origin` and `upstream` in a typical forking workflow?](#what-is-the-difference-between-origin-and-upstream-in-a-typical-forking-workflow)
  - [What does `git fetch --all` do, and how does it differ from a plain `git fetch`?](#what-does-git-fetch---all-do-and-how-does-it-differ-from-a-plain-git-fetch)
  - [What happens if you try to `git push` to a branch that has protection rules enabled on GitHub?](#what-happens-if-you-try-to-git-push-to-a-branch-that-has-protection-rules-enabled-on-github)
  - [What is a shallow clone, and when would you use one?](#what-is-a-shallow-clone-and-when-would-you-use-one)
  - [What is the difference between `git push origin --delete <branch>` and just deleting a branch locally?](#what-is-the-difference-between-git-push-origin---delete-branch-and-just-deleting-a-branch-locally)
  - [What is a bare repository, and why do Git servers typically use one?](#what-is-a-bare-repository-and-why-do-git-servers-typically-use-one)
  - [How would you change the URL of an existing remote, e.g. after a repository is renamed or moved?](#how-would-you-change-the-url-of-an-existing-remote-eg-after-a-repository-is-renamed-or-moved)
- [Undoing Changes & Recovery](#undoing-changes--recovery)
  - [How do you discard uncommitted changes to a single file, reverting it to its last committed state?](#how-do-you-discard-uncommitted-changes-to-a-single-file-reverting-it-to-its-last-committed-state)
  - [How do you unstage a file without discarding its changes?](#how-do-you-unstage-a-file-without-discarding-its-changes)
  - [How would you completely undo the last commit but keep its changes available to re-commit differently?](#how-would-you-completely-undo-the-last-commit-but-keep-its-changes-available-to-re-commit-differently)
  - [What is the reflog, and how can it help recover "lost" commits?](#what-is-the-reflog-and-how-can-it-help-recover-lost-commits)
  - [How would you recover a branch that was accidentally deleted?](#how-would-you-recover-a-branch-that-was-accidentally-deleted)
  - [What is the difference between `git revert` and `git reset` in terms of safety on a shared branch?](#what-is-the-difference-between-git-revert-and-git-reset-in-terms-of-safety-on-a-shared-branch)
  - [How would you undo changes made by a specific commit somewhere in the middle of your history, without affecting later commits?](#how-would-you-undo-changes-made-by-a-specific-commit-somewhere-in-the-middle-of-your-history-without-affecting-later-commits)
  - [What happens to uncommitted changes when you check out a different branch, and when does Git prevent it?](#what-happens-to-uncommitted-changes-when-you-check-out-a-different-branch-and-when-does-git-prevent-it)
  - [How would you completely remove a file from an entire repository's history, e.g. one that accidentally contained a secret?](#how-would-you-completely-remove-a-file-from-an-entire-repositorys-history-eg-one-that-accidentally-contained-a-secret)
  - [What is the difference between `git clean` and `git reset --hard`?](#what-is-the-difference-between-git-clean-and-git-reset---hard)
- [Stashing, Tags & Cleaning](#stashing-tags--cleaning)
  - [What does `git stash` do by default, and how do you restore stashed changes?](#what-does-git-stash-do-by-default-and-how-do-you-restore-stashed-changes)
  - [What is the difference between `git stash pop` and `git stash apply`?](#what-is-the-difference-between-git-stash-pop-and-git-stash-apply)
  - [How would you stash only some of your changes, not everything?](#how-would-you-stash-only-some-of-your-changes-not-everything)
  - [What is the difference between a lightweight tag and an annotated tag, and how do you create each?](#what-is-the-difference-between-a-lightweight-tag-and-an-annotated-tag-and-how-do-you-create-each)
  - [How do you push tags to a remote, since `git push` doesn't push them by default?](#how-do-you-push-tags-to-a-remote-since-git-push-doesnt-push-them-by-default)
  - [What does `git clean -fd` do, and why does it require the `-f` flag?](#what-does-git-clean--fd-do-and-why-does-it-require-the--f-flag)
  - [How would you preview what `git clean` would delete without actually deleting anything?](#how-would-you-preview-what-git-clean-would-delete-without-actually-deleting-anything)
  - [What happens to your stashes if you delete the branch you created them on?](#what-happens-to-your-stashes-if-you-delete-the-branch-you-created-them-on)
- [Git Internals](#git-internals)
  - [What are the four main types of objects stored in Git's object database?](#what-are-the-four-main-types-of-objects-stored-in-gits-object-database)
  - [How does Git store file content internally — does it store diffs between versions?](#how-does-git-store-file-content-internally--does-it-store-diffs-between-versions)
  - [What is the `.git` directory, and what are some of its important contents?](#what-is-the-git-directory-and-what-are-some-of-its-important-contents)
  - [What is a Git object's SHA hash actually computed from?](#what-is-a-git-objects-sha-hash-actually-computed-from)
  - [What is the difference between a symbolic reference like `HEAD` and a direct object reference?](#what-is-the-difference-between-a-symbolic-reference-like-head-and-a-direct-object-reference)
  - [What is packing in Git, and why does it matter for repository size?](#what-is-packing-in-git-and-why-does-it-matter-for-repository-size)
  - [What does `git gc` do?](#what-does-git-gc-do)
  - [What is the difference between a "loose" object and a "packed" object?](#what-is-the-difference-between-a-loose-object-and-a-packed-object)
- [GitHub Specific Features](#github-specific-features)
  - [What is a pull request, and how does it differ from just pushing directly to a branch?](#what-is-a-pull-request-and-how-does-it-differ-from-just-pushing-directly-to-a-branch)
  - [What is the difference between "merge commit," "squash and merge," and "rebase and merge" when merging a pull request on GitHub?](#what-is-the-difference-between-merge-commit-squash-and-merge-and-rebase-and-merge-when-merging-a-pull-request-on-github)
  - [What are GitHub Actions, and what is a workflow file?](#what-are-github-actions-and-what-is-a-workflow-file)
  - [What is a GitHub Issue, and how does it differ from a pull request?](#what-is-a-github-issue-and-how-does-it-differ-from-a-pull-request)
  - [What is a branch protection rule on GitHub, and what does it typically enforce?](#what-is-a-branch-protection-rule-on-github-and-what-does-it-typically-enforce)
  - [What is the difference between "watching," "starring," and "forking" a repository on GitHub?](#what-is-the-difference-between-watching-starring-and-forking-a-repository-on-github)
  - [What is a draft pull request?](#what-is-a-draft-pull-request)
  - [What does it mean to "squash and merge" a PR, and what's a downside of doing so for every PR?](#what-does-it-mean-to-squash-and-merge-a-pr-and-whats-a-downside-of-doing-so-for-every-pr)
  - [What is a GitHub Codespace?](#what-is-a-github-codespace)
  - [What is the difference between a public and a private repository on GitHub?](#what-is-the-difference-between-a-public-and-a-private-repository-on-github)
  - [What is CODEOWNERS in a GitHub repository used for?](#what-is-codeowners-in-a-github-repository-used-for)
  - [What is the difference between a GitHub "release" and a Git tag?](#what-is-the-difference-between-a-github-release-and-a-git-tag)
- [Workflows & Best Practices](#workflows--best-practices)
  - [What is Gitflow, and what are its main branch types?](#what-is-gitflow-and-what-are-its-main-branch-types)
  - [What is trunk-based development, and how does it differ from Gitflow?](#what-is-trunk-based-development-and-how-does-it-differ-from-gitflow)
  - [What is a hotfix branch, and why is it typically branched from `main`/production rather than `develop`?](#what-is-a-hotfix-branch-and-why-is-it-typically-branched-from-mainproduction-rather-than-develop)
  - [What is a good rule of thumb for how often to commit?](#what-is-a-good-rule-of-thumb-for-how-often-to-commit)
  - [What is semantic commit messaging (e.g. Conventional Commits), and what benefit does it provide?](#what-is-semantic-commit-messaging-eg-conventional-commits-and-what-benefit-does-it-provide)
  - [Why is it generally discouraged to commit directly to `main` in a team setting, even for small changes?](#why-is-it-generally-discouraged-to-commit-directly-to-main-in-a-team-setting-even-for-small-changes)
  - [What is the purpose of a `.gitattributes` file?](#what-is-the-purpose-of-a-gitattributes-file)
  - [Why is it considered bad practice to commit generated files (like build output or `node_modules`) to a repository?](#why-is-it-considered-bad-practice-to-commit-generated-files-like-build-output-or-node_modules-to-a-repository)
- [Behavioral / Scenario-Based Questions](#behavioral--scenario-based-questions)
  - [You accidentally committed a sensitive API key to a public repository — what would you do?](#you-accidentally-committed-a-sensitive-api-key-to-a-public-repository--what-would-you-do)
  - [A teammate force-pushed to a shared branch and now your local branch has diverged unexpectedly — how would you handle it?](#a-teammate-force-pushed-to-a-shared-branch-and-now-your-local-branch-has-diverged-unexpectedly--how-would-you-handle-it)
  - [How would you review a large, sprawling pull request that touches many unrelated things at once?](#how-would-you-review-a-large-sprawling-pull-request-that-touches-many-unrelated-things-at-once)
  - [How would you decide whether to use `git merge` or `git rebase` when integrating your feature branch's upstream changes?](#how-would-you-decide-whether-to-use-git-merge-or-git-rebase-when-integrating-your-feature-branchs-upstream-changes)
  - [You need to make an urgent fix, but your working directory is full of unrelated in-progress changes — how would you handle it?](#you-need-to-make-an-urgent-fix-but-your-working-directory-is-full-of-unrelated-in-progress-changes--how-would-you-handle-it)
  - [How would you investigate exactly when and by whom a specific line of buggy code was introduced?](#how-would-you-investigate-exactly-when-and-by-whom-a-specific-line-of-buggy-code-was-introduced)
  - [A CI pipeline is failing only on a pull request, not on `main` — how would you approach debugging it?](#a-ci-pipeline-is-failing-only-on-a-pull-request-not-on-main--how-would-you-approach-debugging-it)
  - [How would you set up a new team member's Git workflow for contributing to a repository they don't have direct write access to?](#how-would-you-set-up-a-new-team-members-git-workflow-for-contributing-to-a-repository-they-dont-have-direct-write-access-to)
- [How to Use This Guide](#how-to-use-this-guide)

---

<a id="-most-asked--tricky-questions"></a>
## 🔥 Most Asked / Tricky Questions

These come up in almost every Git and GitHub interview. If you're short on time, start here.

<a id="what-is-the-difference-between-git-and-github"></a>
### Q: What is the difference between Git and GitHub?
**Answer:** Git is a distributed version control system that runs locally on your machine, tracking changes to files over time. GitHub is a cloud-based hosting platform built around Git, adding remote repository hosting, collaboration features like pull requests and issues, and CI/CD via Actions — Git works perfectly fine without GitHub, and GitHub is just one of several git hosting providers (alongside GitLab, Bitbucket, etc.).

<a id="what-is-the-difference-between-git-merge-and-git-rebase"></a>
### Q: What is the difference between `git merge` and `git rebase`?
**Answer:** `git merge` combines two branches by creating a new merge commit that ties both histories together, preserving the exact history of both branches. `git rebase` replays your branch's commits one by one on top of the target branch, producing a linear history with no merge commit, but rewriting commit hashes in the process.

<a id="what-is-the-difference-between-git-fetch-and-git-pull"></a>
### Q: What is the difference between `git fetch` and `git pull`?
**Answer:** `git fetch` downloads new commits/branches from a remote but doesn't touch your working directory or local branches — it just updates your local copy of the remote's state. `git pull` does a `fetch` immediately followed by a `merge` (or `rebase`, if configured) into your current branch, actually updating your working files.

<a id="what-is-the-difference-between-git-reset-and-git-revert"></a>
### Q: What is the difference between `git reset` and `git revert`?
**Answer:** `git reset` moves the current branch pointer backward (optionally also changing the working directory/staging area), effectively erasing commits from the branch's history — safe only on commits not yet pushed/shared. `git revert` creates a brand-new commit that undoes the changes of a previous commit, leaving the original commit intact in history — safe to use on already-shared/pushed commits.

<a id="what-is-a-merge-conflict-and-when-does-it-happen"></a>
### Q: What is a merge conflict, and when does it happen?
**Answer:** A merge conflict happens when Git can't automatically reconcile changes to the same lines of a file made independently on two branches being merged (or rebased), and requires a human to manually decide which changes to keep.

<a id="what-is-the-difference-between-a-git-reset---soft---mixed-and---hard"></a>
### Q: What is the difference between a `git reset --soft`, `--mixed`, and `--hard`?
**Answer:** `--soft` moves the branch pointer but leaves both the staging area and working directory untouched — changes from the "undone" commits appear as staged changes. `--mixed` (the default) also moves the pointer and unstages changes, but leaves them in the working directory as unstaged edits. `--hard` moves the pointer AND discards all changes in both the staging area and working directory, permanently losing any uncommitted work.

<a id="what-is-a-detached-head-state"></a>
### Q: What is a detached HEAD state?
**Answer:** A state where `HEAD` points directly to a specific commit instead of to a branch — common after checking out a commit hash, a tag, or a remote branch directly. Commits made in this state aren't attached to any branch, so they can become unreachable and eventually garbage-collected unless you create a new branch to keep pointing to them.

<a id="what-is-the-difference-between-git-branch--d-and-git-branch--d"></a>
### Q: What is the difference between `git branch -d` and `git branch -D`?
**Answer:** `-d` deletes a branch only if it's already been fully merged into its upstream branch, refusing otherwise as a safety check. `-D` force-deletes the branch regardless of its merge status, discarding any unmerged commits on it permanently.

<a id="what-does-git-cherry-pick-do"></a>
### Q: What does `git cherry-pick` do?
**Answer:** It applies the changes introduced by a specific commit from one branch onto your current branch, creating a new commit with the same changes but a different commit hash — useful for pulling in a single specific fix without merging an entire branch.

<a id="what-is-the-difference-between-the-working-directory-staging-area-and-repository-in-git"></a>
### Q: What is the difference between the working directory, staging area, and repository in Git?
**Answer:** The working directory is your actual files on disk, where you make edits. The staging area (or "index") is a holding area where you mark exactly which changes will go into the next commit, via `git add`. The repository (`.git` folder) is where committed history is permanently stored.

<a id="what-is-gitignore-used-for"></a>
### Q: What is `.gitignore` used for?
**Answer:** A file listing patterns for files/directories that Git should never track — build artifacts, dependency folders like `node_modules`, environment files with secrets, OS-specific files — keeping them out of the repository entirely, even if `git add .` is run broadly.

<a id="what-is-the-difference-between-a-fork-and-a-clone"></a>
### Q: What is the difference between a fork and a clone?
**Answer:** A clone is a local copy of a repository on your own machine, still linked to the original remote. A fork is a full copy of someone else's repository made under your own GitHub account, giving you a separate remote repository you have write access to, typically used to contribute to a project you don't have direct push access to.

<a id="what-happens-when-you-run-git-push-and-someone-else-has-already-pushed-conflicting-commits"></a>
### Q: What happens when you run `git push` and someone else has already pushed conflicting commits?
**Answer:** Git rejects the push with a "non-fast-forward" error, since your local branch's history has diverged from the remote's — you need to `git pull` (or `fetch` + `merge`/`rebase`) to incorporate the remote's new commits first before you can push successfully.

<a id="what-is-the-difference-between-git-stash-and-just-committing-work-in-progress-changes"></a>
### Q: What is the difference between `git stash` and just committing work-in-progress changes?
**Answer:** `git stash` temporarily shelves uncommitted changes (both staged and unstaged) without creating a permanent commit, letting you switch context cleanly and reapply them later with `git stash pop`. Committing WIP work creates a permanent, visible commit in history that you'd otherwise need to explicitly amend or squash away later.

<a id="what-is-a-fast-forward-merge"></a>
### Q: What is a fast-forward merge?
**Answer:** A merge where the target branch's pointer can simply be moved forward to match the branch being merged in, because the target branch has no new commits of its own since they diverged — no actual merge commit is needed, and history stays perfectly linear.

---

<a id="git-basics"></a>
## Git Basics

<a id="what-is-version-control-and-why-is-it-important"></a>
### Q: What is version control, and why is it important?
**Answer:** Version control is a system that tracks changes to files over time, letting you see history, compare versions, revert mistakes, and collaborate with others without overwriting each other's work. It's essential for any non-trivial software project, providing both a safety net and a coordination mechanism for teams.

<a id="what-is-the-difference-between-a-centralized-and-a-distributed-version-control-system"></a>
### Q: What is the difference between a centralized and a distributed version control system?
**Answer:** A centralized system (like old-school SVN) keeps the full history on a single central server, and clients only hold a working copy of the current version. A distributed system like Git gives every clone a complete copy of the entire project history, so most operations (like viewing history or committing) work fully offline.

<a id="how-do-you-initialize-a-new-git-repository"></a>
### Q: How do you initialize a new Git repository?
**Answer:** `git init` in a project directory creates a new, empty `.git` folder that turns that directory into a Git repository, ready to start tracking files.

<a id="what-is-the-difference-between-git-add--and-git-add--a"></a>
### Q: What is the difference between `git add .` and `git add -A`?
**Answer:** `git add .` stages new and modified files within the current directory and its subdirectories, but in older Git versions it wouldn't stage deletions outside the current directory. `git add -A` (or `--all`) stages all changes across the entire repository, including deletions, regardless of your current directory — in modern Git, `git add .` from the repo root behaves almost identically to `-A`.

<a id="what-is-the-purpose-of-a-commit-message-and-what-makes-a-good-one"></a>
### Q: What is the purpose of a commit message, and what makes a good one?
**Answer:** A commit message documents what changed and, more importantly, why — future readers (including yourself) rely on it to understand the intent behind a change without having to fully re-read the diff. A good message has a short, descriptive summary line (often under ~50 characters), written in the imperative mood ("Fix bug" not "Fixed bug"), with an optional longer body explaining context or reasoning if needed.

<a id="what-is-the-difference-between-git-status-and-git-log"></a>
### Q: What is the difference between `git status` and `git log`?
**Answer:** `git status` shows the current state of your working directory and staging area — what's changed, staged, or untracked right now. `git log` shows the historical record of past commits already made to the repository.

<a id="what-does-git-diff-show-and-how-does-it-change-when-you-add---staged"></a>
### Q: What does `git diff` show, and how does it change when you add `--staged`?
**Answer:** `git diff` shows the differences between your working directory and the staging area (unstaged changes). `git diff --staged` (or `--cached`) shows the differences between the staging area and the last commit — i.e., exactly what will go into your next commit.

<a id="what-is-a-sha-commit-hash-and-how-is-it-generated"></a>
### Q: What is a SHA (commit hash), and how is it generated?
**Answer:** A unique identifier for a commit, generated by hashing the commit's content, its metadata (author, timestamp, message), and a reference to its parent commit(s), using SHA-1 (or SHA-256 in newer Git configurations). Because the hash depends on the parent, changing any earlier commit changes the hashes of every commit after it.

<a id="what-is-the-difference-between-tracked-untracked-staged-and-modified-files"></a>
### Q: What is the difference between tracked, untracked, staged, and modified files?
**Answer:** Untracked files exist in the working directory but Git isn't watching them at all yet. Tracked files are already known to Git (previously committed or staged). Modified means a tracked file has changed since its last commit. Staged means those changes have been added to the index, ready to be included in the next commit.

<a id="what-does-git-clone-do"></a>
### Q: What does `git clone` do?
**Answer:** It creates a full local copy of a remote repository, including its entire commit history and all branches/tags, and automatically sets up a remote connection (named `origin` by default) pointing back to the source.

---

<a id="committing--history"></a>
## Committing & History

<a id="what-does-git-commit---amend-do"></a>
### Q: What does `git commit --amend` do?
**Answer:** It modifies the most recent commit — updating its message and/or adding newly staged changes to it — rather than creating a brand-new commit, effectively replacing the previous commit with a new one (with a new hash).

<a id="why-is-it-risky-to-amend-or-rebase-commits-that-have-already-been-pushed-and-shared-with-others"></a>
### Q: Why is it risky to amend or rebase commits that have already been pushed and shared with others?
**Answer:** Both operations rewrite commit history, generating new commit hashes for what look like "the same" changes. Anyone who already pulled the original commits now has a diverged history, and will hit confusing conflicts or duplicate commits when they try to sync — hence the common advice to only rewrite history that hasn't been shared yet.

<a id="what-is-the-difference-between-git-log-and-git-log---oneline"></a>
### Q: What is the difference between `git log` and `git log --oneline`?
**Answer:** `git log` shows the full details of each commit — hash, author, date, and full message — one after another. `git log --oneline` condenses each commit to a single line with an abbreviated hash and the summary line, useful for quickly scanning a lot of history.

<a id="how-would-you-view-the-history-of-changes-made-to-a-specific-file"></a>
### Q: How would you view the history of changes made to a specific file?
**Answer:** `git log -- <filename>` shows the commits that touched that file; adding `-p` (`git log -p -- <filename>`) also shows the actual diff introduced to that file in each of those commits.

<a id="what-is-git-blame-used-for"></a>
### Q: What is `git blame` used for?
**Answer:** It annotates each line of a file with the commit and author responsible for last changing that line, useful for tracking down when and why a particular piece of code was introduced.

<a id="what-is-a-squash-commit-and-why-would-you-use-one"></a>
### Q: What is a squash commit, and why would you use one?
**Answer:** Combining multiple commits into a single commit, typically done via an interactive rebase (`git rebase -i`) or when merging a pull request with a "squash and merge" option. It's used to clean up a messy series of small, incremental "WIP" commits into one clean, logical commit before it lands in the main history.

<a id="what-is-the-difference-between-head-head1-and-head"></a>
### Q: What is the difference between `HEAD`, `HEAD~1`, and `HEAD^`?
**Answer:** `HEAD` refers to your current commit/branch tip. `HEAD~1` and `HEAD^` both refer to the immediate parent of the current commit — for a normal commit with a single parent they're identical, but `HEAD^2` specifically refers to the second parent of a merge commit, which `HEAD~2` (two generations back) does not.

<a id="what-is-a-tag-in-git-and-whats-the-difference-between-a-lightweight-and-an-annotated-tag"></a>
### Q: What is a tag in Git, and what's the difference between a lightweight and an annotated tag?
**Answer:** A tag is a fixed, named pointer to a specific commit, typically used to mark release points (`v1.0.0`). A lightweight tag is just a simple pointer with no extra metadata. An annotated tag is stored as a full object in Git's database, including a tagger name, date, and message, and is the generally recommended type for actual releases.

<a id="how-would-you-find-which-commit-introduced-a-bug"></a>
### Q: How would you find which commit introduced a bug?
**Answer:** `git bisect` performs a binary search through commit history — you mark a known-good and known-bad commit, and Git checks out commits in between for you to test one at a time, narrowing down the exact commit that introduced the issue in roughly log(n) steps.

<a id="what-information-does-a-git-commit-object-actually-store"></a>
### Q: What information does a Git commit object actually store?
**Answer:** A pointer to the tree object representing the project's file/directory structure at that point, a pointer to its parent commit(s), the author and committer's name/email/timestamp, and the commit message.

---

<a id="branching"></a>
## Branching

<a id="what-is-a-branch-in-git-conceptually"></a>
### Q: What is a branch in Git, conceptually?
**Answer:** A branch is simply a lightweight, movable pointer to a specific commit — creating a branch doesn't copy any files, it just creates a new named reference, which is why branching in Git is extremely fast and cheap compared to some other version control systems.

<a id="what-command-creates-a-new-branch-and-whats-the-difference-between-that-and-also-switching-to-it"></a>
### Q: What command creates a new branch, and what's the difference between that and also switching to it?
**Answer:** `git branch <name>` creates a new branch pointer without switching to it. `git checkout -b <name>` (or the newer `git switch -c <name>`) creates the branch AND immediately switches your working directory to it in one step.

<a id="what-is-the-difference-between-git-checkout-and-git-switch"></a>
### Q: What is the difference between `git checkout` and `git switch`?
**Answer:** `git checkout` is an older, multi-purpose command that can switch branches, restore files, and check out specific commits — its broad scope makes it a bit confusing. `git switch` (added later) is a narrower, dedicated command specifically for switching/creating branches, and `git restore` was added alongside it specifically for restoring files, splitting `checkout`'s responsibilities into clearer, separate commands.

<a id="why-is-branching-considered-cheap-and-fast-in-git-compared-to-some-older-version-control-systems"></a>
### Q: Why is branching considered cheap and fast in Git compared to some older version control systems?
**Answer:** Because a Git branch is just a small pointer (a file containing a commit hash), not a full copy of the codebase — creating one is nearly instantaneous and takes almost no extra disk space, unlike systems where branching involved physically copying the entire project directory.

<a id="what-is-the-difference-between-a-local-branch-and-a-remote-tracking-branch"></a>
### Q: What is the difference between a local branch and a remote-tracking branch?
**Answer:** A local branch exists only in your own repository. A remote-tracking branch (like `origin/main`) is a local, read-only reference reflecting the last-known state of a branch on the remote, updated whenever you `fetch` — it isn't a branch you directly commit to yourself.

<a id="what-does-it-mean-for-a-local-branch-to-track-a-remote-branch"></a>
### Q: What does it mean for a local branch to "track" a remote branch?
**Answer:** It means the local branch is explicitly linked to a corresponding remote branch, so commands like `git pull` and `git push` (without extra arguments) automatically know which remote branch to sync with, and `git status` can tell you how many commits you're ahead/behind.

<a id="what-is-the-difference-between-git-branch-and-git-branch--a"></a>
### Q: What is the difference between `git branch` and `git branch -a`?
**Answer:** `git branch` lists only your local branches. `git branch -a` lists both local branches and all known remote-tracking branches.

<a id="how-would-you-rename-a-branch-including-one-already-pushed-to-a-remote"></a>
### Q: How would you rename a branch, including one already pushed to a remote?
**Answer:** Rename it locally with `git branch -m <old-name> <new-name>` (or `-m <new-name>` if it's your current branch), then push the new name and delete the old one on the remote.

**Example:**
```bash
git branch -m old-name new-name
git push origin -u new-name
git push origin --delete old-name
```

<a id="what-is-a-feature-branch-and-why-is-the-pattern-commonly-used"></a>
### Q: What is a feature branch, and why is the pattern commonly used?
**Answer:** A branch created specifically to develop one feature or fix in isolation from the main line of development, merged back in (often via a pull request) once it's complete and reviewed. It keeps `main`/`master` always in a stable, deployable state, and lets multiple people work on different things in parallel without stepping on each other.

<a id="what-happens-to-a-branch-pointer-when-you-make-a-new-commit-while-on-that-branch"></a>
### Q: What happens to a branch pointer when you make a new commit while on that branch?
**Answer:** The branch pointer automatically moves forward to point at the newly created commit — this automatic movement is exactly what "being on a branch" means, as opposed to a detached `HEAD` state where no branch pointer follows along.

---

<a id="merging--rebasing"></a>
## Merging & Rebasing

<a id="what-happens-internally-during-a-git-merge"></a>
### Q: What happens internally during a `git merge`?
**Answer:** Git finds the common ancestor commit of the two branches, then either fast-forwards if possible, or computes the combined diff (a three-way merge) and creates a new commit with two parents — one from each branch — representing that combination.

<a id="what-is-a-three-way-merge"></a>
### Q: What is a three-way merge?
**Answer:** A merge strategy that compares three points: the common ancestor commit, and the tip of each of the two branches being merged, to determine what changed on each side since they diverged — allowing Git to intelligently combine non-overlapping changes automatically.

<a id="what-are-the-trade-offs-between-a-merge-based-workflow-and-a-rebase-based-workflow"></a>
### Q: What are the trade-offs between a merge-based workflow and a rebase-based workflow?
**Answer:** Merging preserves the true, complete history of how branches actually diverged and came back together, but can result in a cluttered history full of merge commits. Rebasing produces a cleaner, linear history that's easier to read, but rewrites commit hashes and loses the record of exactly when/how branches originally diverged — and is riskier on shared branches.

<a id="what-does-interactive-rebase-git-rebase--i-let-you-do"></a>
### Q: What does interactive rebase (`git rebase -i`) let you do?
**Answer:** It opens an editable list of commits being replayed, letting you reorder them, edit their content or message ("reword"/"edit"), combine multiple commits into one ("squash"/"fixup"), or drop commits entirely — a powerful tool for cleaning up local history before sharing it.

<a id="what-is-the-golden-rule-of-rebasing"></a>
### Q: What is the "golden rule of rebasing"?
**Answer:** Never rebase commits that have already been pushed to a shared/public branch and that others may have already based work on — doing so rewrites history that others depend on, causing painful, confusing conflicts for them when they try to sync.

<a id="what-is-a-merge-conflict-marker-and-what-do-the-different-sections-mean"></a>
### Q: What is a merge conflict marker, and what do the different sections mean?
**Answer:** The `<<<<<<<`, `=======`, and `>>>>>>>` markers Git inserts directly into a conflicted file. Content between `<<<<<<< HEAD` and `=======` is your current branch's version; content between `=======` and `>>>>>>> branch-name` is the incoming branch's version — you edit the file to resolve it to the version you actually want, then remove the markers.

<a id="what-is-git-rebase---continue---abort-and---skip-used-for"></a>
### Q: What is `git rebase --continue`, `--abort`, and `--skip` used for?
**Answer:** During a rebase paused by a conflict, `--continue` resumes the rebase after you've manually resolved the conflict and staged the fix. `--abort` cancels the entire rebase and returns the branch to exactly the state it was in before starting. `--skip` skips the current conflicting commit entirely, discarding its changes, and moves on to the next one.

<a id="what-is-a-merge-strategy-and-whats-the-difference-between-the-default-strategy-and-squash-merging"></a>
### Q: What is a merge strategy, and what's the difference between the default strategy and squash merging?
**Answer:** A merge strategy is the algorithm Git uses to combine branches. The default strategy creates a normal merge commit with two parents, preserving both branches' individual commit history. A squash merge takes all the changes from the branch being merged and applies them as a single new commit on the target branch, with no merge commit and no individual commit history preserved from the source branch.

<a id="what-is-git-rerere-and-what-problem-does-it-solve"></a>
### Q: What is `git rerere`, and what problem does it solve?
**Answer:** Short for "reuse recorded resolution" — when enabled, Git remembers how you resolved a specific conflict once, and automatically applies that same resolution again if the identical conflict shows up later, common during a long-running rebase or when repeatedly merging the same two branches.

<a id="when-would-you-choose-git-merge---no-ff-over-a-regular-merge"></a>
### Q: When would you choose `git merge --no-ff` over a regular merge?
**Answer:** `--no-ff` forces a merge commit to be created even when a fast-forward would otherwise be possible, explicitly preserving a record that a feature branch existed and was merged in at a specific point — useful for keeping a clear, visible history of feature integration even on branches that could have fast-forwarded silently.

---

<a id="merge-conflicts"></a>
## Merge Conflicts

<a id="what-causes-a-merge-conflict-specifically"></a>
### Q: What causes a merge conflict, specifically?
**Answer:** Git can automatically combine changes when they touch different, non-overlapping parts of a file, or the same part in an identical way. A conflict arises specifically when both branches modify the exact same lines (or one branch modifies a line the other deleted) in genuinely different, incompatible ways — Git can't determine which version is "correct" on its own.

<a id="what-is-the-general-process-for-resolving-a-merge-conflict"></a>
### Q: What is the general process for resolving a merge conflict?
**Answer:** Open each conflicted file, locate the conflict markers, decide (or combine) which changes to keep, remove the conflict markers entirely, then stage the resolved file with `git add` and complete the merge with `git commit` (or `git rebase --continue` if mid-rebase).

<a id="what-is-the-difference-between-resolving-a-conflict-during-a-merge-versus-during-a-rebase"></a>
### Q: What is the difference between resolving a conflict during a `merge` versus during a `rebase`?
**Answer:** During a `merge`, you resolve conflicts once and finish with a single `git commit`. During a `rebase`, since commits are replayed one at a time, a conflict might occur — and need to be resolved — separately for each individual commit being replayed, potentially multiple times for the same overall change.

<a id="how-can-you-use-a-merge-tool-to-help-resolve-conflicts"></a>
### Q: How can you use a merge tool to help resolve conflicts?
**Answer:** `git mergetool` launches a configured visual diff/merge tool (like VS Code, Meld, or KDiff3) that shows the conflicting versions side by side and lets you pick or combine changes with a GUI, instead of manually editing the raw conflict markers in a text editor.

<a id="what-does-git-diff-show-you-while-a-merge-conflict-is-unresolved"></a>
### Q: What does `git diff` show you while a merge conflict is unresolved?
**Answer:** It highlights the conflicting sections with special formatting showing both sides of the conflict inline (a "combined diff"), which can help you understand exactly what each branch changed even before opening the file directly.

<a id="how-would-you-abort-a-merge-thats-gone-wrong-and-return-to-the-state-before-you-started"></a>
### Q: How would you abort a merge that's gone wrong and return to the state before you started?
**Answer:** `git merge --abort` cancels the in-progress merge and restores the working directory and staging area to exactly how they were before the merge was attempted.

<a id="how-do-binary-file-conflicts-differ-from-text-file-conflicts-and-how-are-they-resolved"></a>
### Q: How do binary file conflicts differ from text file conflicts, and how are they resolved?
**Answer:** Git can't merge binary files line by line the way it does text, so it can't insert conflict markers inside them — it just presents both versions as entirely separate options. Resolution means manually choosing which entire version to keep with `git checkout --ours <file>` or `--theirs <file>`, then staging it.

<a id="what-are---ours-and---theirs-in-the-context-of-resolving-a-conflict-and-does-their-meaning-change-between-merge-and-rebase"></a>
### Q: What are `--ours` and `--theirs` in the context of resolving a conflict, and does their meaning change between merge and rebase?
**Answer:** They let you resolve a conflict by keeping one side's entire version of a file. Their meaning flips between the two operations: during a `merge`, "ours" is your current branch and "theirs" is the branch being merged in; during a `rebase`, since your commits are being replayed onto the target, "ours" refers to the target branch and "theirs" refers to your own commit being replayed — a common source of confusion.

---

<a id="remote-repositories"></a>
## Remote Repositories

<a id="what-is-a-remote-in-git"></a>
### Q: What is a remote in Git?
**Answer:** A named reference to a version of your repository hosted elsewhere — typically on a server like GitHub — that you can push to and pull/fetch from. `origin` is the conventional default name for the remote a repository was cloned from.

<a id="what-is-the-difference-between-git-push-and-git-push--u-or---set-upstream"></a>
### Q: What is the difference between `git push` and `git push -u` (or `--set-upstream`)?
**Answer:** `git push` pushes to an already-configured upstream branch. `git push -u origin <branch>` both pushes AND sets up the tracking relationship for that local branch to that specific remote branch, so future plain `git push`/`git pull` commands on that branch know where to sync automatically.

<a id="how-do-you-add-view-and-remove-a-remote"></a>
### Q: How do you add, view, and remove a remote?
**Answer:** `git remote add <name> <url>` adds a new remote, `git remote -v` lists all configured remotes and their URLs, and `git remote remove <name>` removes one.

**Example:**
```bash
git remote add origin https://github.com/user/repo.git
git remote -v
git remote remove origin
```

<a id="what-is-the-difference-between-origin-and-upstream-in-a-typical-forking-workflow"></a>
### Q: What is the difference between `origin` and `upstream` in a typical forking workflow?
**Answer:** `origin` conventionally refers to your own fork on GitHub, which you have push access to. `upstream` conventionally refers to the original repository you forked from, added as a second remote so you can pull in the latest changes from the original project without needing write access to it.

<a id="what-does-git-fetch---all-do-and-how-does-it-differ-from-a-plain-git-fetch"></a>
### Q: What does `git fetch --all` do, and how does it differ from a plain `git fetch`?
**Answer:** A plain `git fetch` updates remote-tracking branches for the default remote (`origin`, typically). `git fetch --all` fetches updates from every configured remote in the repository, not just one.

<a id="what-happens-if-you-try-to-git-push-to-a-branch-that-has-protection-rules-enabled-on-github"></a>
### Q: What happens if you try to `git push` to a branch that has protection rules enabled on GitHub?
**Answer:** GitHub rejects the push (or specific parts of it) if it violates the configured protection rules — commonly, requiring changes to go through a reviewed and approved pull request instead of a direct push, blocking force-pushes, or requiring status checks (like CI) to pass first.

<a id="what-is-a-shallow-clone-and-when-would-you-use-one"></a>
### Q: What is a shallow clone, and when would you use one?
**Answer:** `git clone --depth 1` (or another small number) fetches only the most recent commit(s) instead of the entire project history, resulting in a much smaller, faster clone — useful in CI pipelines or other contexts where you only need the current state of the code, not its full history.

<a id="what-is-the-difference-between-git-push-origin---delete-branch-and-just-deleting-a-branch-locally"></a>
### Q: What is the difference between `git push origin --delete <branch>` and just deleting a branch locally?
**Answer:** `git branch -d <branch>` only removes the branch reference from your local repository. `git push origin --delete <branch>` additionally removes that branch from the remote repository, deleting it for everyone who fetches from that remote.

<a id="what-is-a-bare-repository-and-why-do-git-servers-typically-use-one"></a>
### Q: What is a bare repository, and why do Git servers typically use one?
**Answer:** A bare repository (`git init --bare`) contains only the `.git` internal data — no working directory of checked-out files at all. Servers use bare repositories because nobody needs to directly edit files on the server; it exists purely to be pushed to and pulled from, avoiding potential conflicts between a server-side working copy and incoming pushes.

<a id="how-would-you-change-the-url-of-an-existing-remote-eg-after-a-repository-is-renamed-or-moved"></a>
### Q: How would you change the URL of an existing remote, e.g. after a repository is renamed or moved?
**Answer:** `git remote set-url origin <new-url>` updates the URL associated with an existing remote without needing to remove and re-add it.

---

<a id="undoing-changes--recovery"></a>
## Undoing Changes & Recovery

<a id="how-do-you-discard-uncommitted-changes-to-a-single-file-reverting-it-to-its-last-committed-state"></a>
### Q: How do you discard uncommitted changes to a single file, reverting it to its last committed state?
**Answer:** `git restore <file>` (or the older `git checkout -- <file>`) discards unstaged changes in the working directory for that file, reverting it back to match the last commit.

<a id="how-do-you-unstage-a-file-without-discarding-its-changes"></a>
### Q: How do you unstage a file without discarding its changes?
**Answer:** `git restore --staged <file>` (or the older `git reset <file>`) removes the file from the staging area, but leaves your actual edits intact in the working directory.

<a id="how-would-you-completely-undo-the-last-commit-but-keep-its-changes-available-to-re-commit-differently"></a>
### Q: How would you completely undo the last commit but keep its changes available to re-commit differently?
**Answer:** `git reset --soft HEAD~1` moves the branch pointer back one commit while leaving all its changes staged, ready to be adjusted and re-committed.

<a id="what-is-the-reflog-and-how-can-it-help-recover-lost-commits"></a>
### Q: What is the reflog, and how can it help recover "lost" commits?
**Answer:** The reflog (`git reflog`) is a local log of every place `HEAD` has pointed to recently — including commits that are no longer reachable from any branch after a hard reset, rebase, or branch deletion. Since the actual commit data typically still exists in Git's object database for a while, you can find its hash in the reflog and recover it, e.g. with `git checkout <hash>` or `git branch recovered-work <hash>`.

<a id="how-would-you-recover-a-branch-that-was-accidentally-deleted"></a>
### Q: How would you recover a branch that was accidentally deleted?
**Answer:** Look through `git reflog` for the commit hash the deleted branch used to point to (its last known tip), then recreate the branch pointing at that commit.

**Example:**
```bash
git reflog
git branch recovered-branch <commit-hash>
```

<a id="what-is-the-difference-between-git-revert-and-git-reset-in-terms-of-safety-on-a-shared-branch"></a>
### Q: What is the difference between `git revert` and `git reset` in terms of safety on a shared branch?
**Answer:** `git revert` is safe on shared/pushed history because it adds a new commit rather than removing existing ones — everyone's history stays consistent. `git reset` rewrites the branch's history by removing commits, which is unsafe once others have already pulled those commits, since it creates divergent histories.

<a id="how-would-you-undo-changes-made-by-a-specific-commit-somewhere-in-the-middle-of-your-history-without-affecting-later-commits"></a>
### Q: How would you undo changes made by a specific commit somewhere in the middle of your history, without affecting later commits?
**Answer:** `git revert <commit-hash>` creates a new commit that applies the inverse of that specific commit's changes, without touching any of the commits that came after it.

<a id="what-happens-to-uncommitted-changes-when-you-check-out-a-different-branch-and-when-does-git-prevent-it"></a>
### Q: What happens to uncommitted changes when you check out a different branch, and when does Git prevent it?
**Answer:** If the changes don't conflict with anything different between the branches, Git carries your uncommitted changes along with you to the new branch. If checking out would overwrite files that differ between your uncommitted changes and the target branch, Git refuses the checkout and asks you to commit, stash, or discard those changes first.

<a id="how-would-you-completely-remove-a-file-from-an-entire-repositorys-history-eg-one-that-accidentally-contained-a-secret"></a>
### Q: How would you completely remove a file from an entire repository's history, e.g. one that accidentally contained a secret?
**Answer:** Simply deleting the file in a new commit isn't enough, since it still exists in earlier commits' history. You need a history-rewriting tool like `git filter-repo` (or the older `git filter-branch`/BFG Repo-Cleaner) to strip the file from every commit, followed by a force-push and, critically, rotating/invalidating the exposed secret itself since it remains recoverable from anyone's existing clone.

<a id="what-is-the-difference-between-git-clean-and-git-reset---hard"></a>
### Q: What is the difference between `git clean` and `git reset --hard`?
**Answer:** `git reset --hard` discards changes to already-tracked files, reverting them to match a specific commit, but doesn't touch untracked files. `git clean` removes untracked files (and, with `-d`, untracked directories) from the working directory entirely — the two are often used together to fully reset a working directory back to a pristine state.

---

<a id="stashing-tags--cleaning"></a>
## Stashing, Tags & Cleaning

<a id="what-does-git-stash-do-by-default-and-how-do-you-restore-stashed-changes"></a>
### Q: What does `git stash` do by default, and how do you restore stashed changes?
**Answer:** It saves your currently staged and unstaged changes to a temporary stack, and reverts your working directory to match the last commit, leaving you a clean state to switch tasks. `git stash pop` reapplies the most recent stash and removes it from the stash list; `git stash apply` reapplies it but keeps it in the list.

<a id="what-is-the-difference-between-git-stash-pop-and-git-stash-apply"></a>
### Q: What is the difference between `git stash pop` and `git stash apply`?
**Answer:** `git stash apply` reapplies a stash's changes to your working directory but keeps the stash saved in the stash list afterward. `git stash pop` does the same but also removes that stash from the list once successfully applied.

<a id="how-would-you-stash-only-some-of-your-changes-not-everything"></a>
### Q: How would you stash only some of your changes, not everything?
**Answer:** `git stash push -p` (or `--patch`) interactively lets you choose specific hunks to stash, rather than stashing every uncommitted change at once.

<a id="what-is-the-difference-between-a-lightweight-tag-and-an-annotated-tag-and-how-do-you-create-each"></a>
### Q: What is the difference between a lightweight tag and an annotated tag, and how do you create each?
**Answer:** A lightweight tag is just a simple named pointer to a commit. An annotated tag is a full Git object storing a message, tagger name, and date — generally recommended for actual release tags since it carries more information.

**Example:**
```bash
git tag v1.0.0                          # lightweight
git tag -a v1.0.0 -m "Release message"  # annotated
```

<a id="how-do-you-push-tags-to-a-remote-since-git-push-doesnt-push-them-by-default"></a>
### Q: How do you push tags to a remote, since `git push` doesn't push them by default?
**Answer:** `git push origin <tag-name>` pushes a single tag; `git push origin --tags` pushes all local tags that aren't already on the remote.

<a id="what-does-git-clean--fd-do-and-why-does-it-require-the--f-flag"></a>
### Q: What does `git clean -fd` do, and why does it require the `-f` flag?
**Answer:** It permanently deletes untracked files (`-f`, "force") and untracked directories (`-d`) from the working directory. The `-f` flag is required by default as a safety measure, since `git clean` is a destructive, irreversible operation with no built-in undo.

<a id="how-would-you-preview-what-git-clean-would-delete-without-actually-deleting-anything"></a>
### Q: How would you preview what `git clean` would delete without actually deleting anything?
**Answer:** `git clean -n` (or `--dry-run`) lists exactly which files/directories would be removed, without actually touching anything — always worth running before the real `git clean -f`.

<a id="what-happens-to-your-stashes-if-you-delete-the-branch-you-created-them-on"></a>
### Q: What happens to your stashes if you delete the branch you created them on?
**Answer:** Nothing — stashes aren't tied to any particular branch; they're stored independently in the repository and remain accessible via `git stash list` from any branch, regardless of which branch was checked out when they were created.

---

<a id="git-internals"></a>
## Git Internals

<a id="what-are-the-four-main-types-of-objects-stored-in-gits-object-database"></a>
### Q: What are the four main types of objects stored in Git's object database?
**Answer:** Blobs (the raw content of a file), trees (representing a directory's structure, listing blobs and other trees with names/permissions), commits (pointing to a tree plus parent commit(s) and metadata), and tags (annotated tags pointing to another object, usually a commit).

<a id="how-does-git-store-file-content-internally--does-it-store-diffs-between-versions"></a>
### Q: How does Git store file content internally — does it store diffs between versions?
**Answer:** Contrary to common assumption, Git doesn't store diffs between file versions internally. Each unique version of a file's content is stored as its own compressed blob object, identified by the hash of its content — Git computes diffs on the fly for display purposes (like `git diff`), rather than storing them.

<a id="what-is-the-git-directory-and-what-are-some-of-its-important-contents"></a>
### Q: What is the `.git` directory, and what are some of its important contents?
**Answer:** The hidden folder at the root of a Git repository holding all of Git's internal data: the `objects` directory (blobs, trees, commits), `refs` (branch and tag pointers), `HEAD` (what you currently have checked out), and `config` (repository-specific settings).

<a id="what-is-a-git-objects-sha-hash-actually-computed-from"></a>
### Q: What is a Git object's SHA hash actually computed from?
**Answer:** A hash of the object's type, size, and content combined — meaning identical content always produces the identical hash, which is also how Git deduplicates storage: two files with exactly the same content, even in unrelated commits, are stored as a single blob object referenced from both places.

<a id="what-is-the-difference-between-a-symbolic-reference-like-head-and-a-direct-object-reference"></a>
### Q: What is the difference between a symbolic reference like `HEAD` and a direct object reference?
**Answer:** `HEAD` is typically a symbolic reference — a small file containing a pointer to a branch reference (e.g. `ref: refs/heads/main`), which itself then points to a commit hash. In a detached `HEAD` state, `HEAD` instead points directly to a commit hash, with no branch reference in between.

<a id="what-is-packing-in-git-and-why-does-it-matter-for-repository-size"></a>
### Q: What is packing in Git, and why does it matter for repository size?
**Answer:** Over time, Git can compress many loose objects together into a single "packfile," using delta compression between similar objects to save significant space — this happens automatically during operations like `git gc` (garbage collection) or when pushing/fetching, keeping the repository's overall size manageable.

<a id="what-does-git-gc-do"></a>
### Q: What does `git gc` do?
**Answer:** Garbage collection — it cleans up unnecessary/unreachable loose objects, compresses file history into packfiles for efficiency, and generally optimizes the repository's internal storage, which Git also runs automatically in the background periodically.

<a id="what-is-the-difference-between-a-loose-object-and-a-packed-object"></a>
### Q: What is the difference between a "loose" object and a "packed" object?
**Answer:** A loose object is stored as its own individual compressed file within `.git/objects`. A packed object is bundled together with many other objects into a single, more efficiently compressed packfile — Git periodically repacks loose objects to save space and improve performance.

---

<a id="github-specific-features"></a>
## GitHub Specific Features

<a id="what-is-a-pull-request-and-how-does-it-differ-from-just-pushing-directly-to-a-branch"></a>
### Q: What is a pull request, and how does it differ from just pushing directly to a branch?
**Answer:** A pull request proposes merging changes from one branch (often a fork or feature branch) into another, providing a dedicated space for code review, discussion, automated checks, and approval before the changes are actually merged — rather than commits landing directly and immediately.

<a id="what-is-the-difference-between-merge-commit-squash-and-merge-and-rebase-and-merge-when-merging-a-pull-request-on-github"></a>
### Q: What is the difference between "merge commit," "squash and merge," and "rebase and merge" when merging a pull request on GitHub?
**Answer:** "Merge commit" creates a standard merge commit preserving the PR branch's full individual commit history. "Squash and merge" combines every commit in the PR into a single new commit on the target branch. "Rebase and merge" replays each of the PR's commits individually onto the target branch with new hashes, keeping them separate but producing a linear history with no merge commit.

<a id="what-are-github-actions-and-what-is-a-workflow-file"></a>
### Q: What are GitHub Actions, and what is a workflow file?
**Answer:** GitHub Actions is GitHub's built-in CI/CD and automation platform, running defined jobs in response to repository events (a push, a pull request, a schedule). A workflow is defined in a YAML file under `.github/workflows/`, specifying triggers, jobs, and the sequence of steps each job runs.

**Example:**
```yaml
name: CI
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm test
```

<a id="what-is-a-github-issue-and-how-does-it-differ-from-a-pull-request"></a>
### Q: What is a GitHub Issue, and how does it differ from a pull request?
**Answer:** An issue tracks a task, bug report, or feature discussion — it's not tied to any specific code changes. A pull request specifically proposes actual code changes for review and merging, though PRs and issues can be linked together (e.g. a PR that "closes" a referenced issue automatically once merged).

<a id="what-is-a-branch-protection-rule-on-github-and-what-does-it-typically-enforce"></a>
### Q: What is a branch protection rule on GitHub, and what does it typically enforce?
**Answer:** A repository setting that restricts certain actions on specific branches (commonly `main`) — such as requiring pull request reviews before merging, requiring status checks (like CI) to pass, disallowing force-pushes, or requiring linear history — used to keep important branches stable and prevent accidental or unreviewed changes.

<a id="what-is-the-difference-between-watching-starring-and-forking-a-repository-on-github"></a>
### Q: What is the difference between "watching," "starring," and "forking" a repository on GitHub?
**Answer:** Watching subscribes you to notifications about a repository's activity. Starring bookmarks a repository to your own profile as a way of showing appreciation or saving it for later, with no functional effect on the repo itself. Forking creates your own independent copy of the entire repository under your account, which you can freely modify.

<a id="what-is-a-draft-pull-request"></a>
### Q: What is a draft pull request?
**Answer:** A pull request explicitly marked as not yet ready for review or merging, useful for sharing work-in-progress, getting early feedback, or triggering CI checks before the work is actually complete — it can be converted to a regular, "ready for review" pull request once finished.

<a id="what-does-it-mean-to-squash-and-merge-a-pr-and-whats-a-downside-of-doing-so-for-every-pr"></a>
### Q: What does it mean to "squash and merge" a PR, and what's a downside of doing so for every PR?
**Answer:** It condenses the entire pull request's commit history into a single commit on the target branch, producing a very clean `main` branch history. A downside is that any intentional, meaningful intermediate commit history from within the PR itself is permanently lost, which can make `git bisect` or detailed history review across many small logical steps less useful later.

<a id="what-is-a-github-codespace"></a>
### Q: What is a GitHub Codespace?
**Answer:** A cloud-hosted, containerized development environment tied to a repository, pre-configured (often via a `devcontainer.json` file) with the tools and dependencies needed to work on that project, accessible from a browser or a local editor without setting anything up locally.

<a id="what-is-the-difference-between-a-public-and-a-private-repository-on-github"></a>
### Q: What is the difference between a public and a private repository on GitHub?
**Answer:** A public repository is visible to anyone on the internet, and anyone can view, clone, and fork it (though not necessarily push to it without permission). A private repository is visible and accessible only to the owner and explicitly invited collaborators.

<a id="what-is-codeowners-in-a-github-repository-used-for"></a>
### Q: What is CODEOWNERS in a GitHub repository used for?
**Answer:** A `CODEOWNERS` file maps specific files/directories in the repository to specific people or teams, automatically requesting their review whenever a pull request modifies those paths — used to make sure changes to sensitive or specialized areas get seen by the right people.

<a id="what-is-the-difference-between-a-github-release-and-a-git-tag"></a>
### Q: What is the difference between a GitHub "release" and a Git tag?
**Answer:** A Git tag is purely a version-control concept — a named pointer to a specific commit. A GitHub release builds on top of a tag, adding a dedicated page with release notes, downloadable source archives, and the ability to attach compiled binaries or other build artifacts.

---

<a id="workflows--best-practices"></a>
## Workflows & Best Practices

<a id="what-is-gitflow-and-what-are-its-main-branch-types"></a>
### Q: What is Gitflow, and what are its main branch types?
**Answer:** A structured branching model built around long-lived `main` (production-ready) and `develop` (integration) branches, with short-lived supporting branches for `feature/*`, `release/*`, and `hotfix/*` work that each merge back into `develop` and/or `main` following defined rules. It's fairly heavyweight and has become less common in favor of simpler models for teams practicing continuous delivery.

<a id="what-is-trunk-based-development-and-how-does-it-differ-from-gitflow"></a>
### Q: What is trunk-based development, and how does it differ from Gitflow?
**Answer:** A workflow where developers integrate small, frequent changes directly into a single main branch (the "trunk"), often behind feature flags rather than long-lived feature branches, aiming for continuous integration and fast, frequent releases. It's simpler than Gitflow's multi-branch structure, but requires strong CI/testing discipline and a culture of small, incremental changes.

<a id="what-is-a-hotfix-branch-and-why-is-it-typically-branched-from-mainproduction-rather-than-develop"></a>
### Q: What is a hotfix branch, and why is it typically branched from `main`/production rather than `develop`?
**Answer:** A branch created to urgently fix a critical bug already live in production. It branches from `main` (the current production state) specifically so the fix doesn't accidentally pull in unrelated, not-yet-released work sitting in `develop`, letting the fix ship immediately and independently.

<a id="what-is-a-good-rule-of-thumb-for-how-often-to-commit"></a>
### Q: What is a good rule of thumb for how often to commit?
**Answer:** Commit small, logically complete, self-contained changes frequently, rather than one enormous commit at the end of a long work session — smaller commits are easier to review, revert individually if something's wrong, and understand later via `git log` or `git bisect`.

<a id="what-is-semantic-commit-messaging-eg-conventional-commits-and-what-benefit-does-it-provide"></a>
### Q: What is semantic commit messaging (e.g. Conventional Commits), and what benefit does it provide?
**Answer:** A convention prefixing commit messages with a type like `feat:`, `fix:`, `docs:`, or `chore:` describing the nature of the change. It provides a consistent, machine-parseable structure that tools can use to automatically generate changelogs and determine semantic version bumps.

<a id="why-is-it-generally-discouraged-to-commit-directly-to-main-in-a-team-setting-even-for-small-changes"></a>
### Q: Why is it generally discouraged to commit directly to `main` in a team setting, even for small changes?
**Answer:** Direct commits bypass code review, automated CI checks, and the discussion/visibility a pull request provides — even small changes can introduce bugs or break something unexpected, and a protected `main` with mandatory PRs creates a consistent safety net for every change, regardless of size.

<a id="what-is-the-purpose-of-a-gitattributes-file"></a>
### Q: What is the purpose of a `.gitattributes` file?
**Answer:** It lets you configure how Git handles specific paths/file types — commonly normalizing line endings consistently across different operating systems, marking certain files as binary so Git doesn't try to diff/merge them as text, or specifying files to exclude from `git diff`/export archives.

<a id="why-is-it-considered-bad-practice-to-commit-generated-files-like-build-output-or-node_modules-to-a-repository"></a>
### Q: Why is it considered bad practice to commit generated files (like build output or `node_modules`) to a repository?
**Answer:** Generated files can always be recreated from source and a build step, so committing them bloats the repository's size and history unnecessarily, creates noisy diffs on every build, and risks the committed version silently drifting out of sync with the actual source that's supposed to generate it — they belong in `.gitignore` instead.

---

<a id="behavioral--scenario-based-questions"></a>
## Behavioral / Scenario-Based Questions

<a id="you-accidentally-committed-a-sensitive-api-key-to-a-public-repository--what-would-you-do"></a>
### Q: You accidentally committed a sensitive API key to a public repository — what would you do?
**Answer:** Immediately rotate/invalidate the exposed key at the source, since it must be treated as compromised the moment it was pushed, regardless of any later history rewriting. Then remove it from history with a tool like `git filter-repo` or BFG Repo-Cleaner, force-push the rewritten history, and add the file/pattern to `.gitignore` going forward.

<a id="a-teammate-force-pushed-to-a-shared-branch-and-now-your-local-branch-has-diverged-unexpectedly--how-would-you-handle-it"></a>
### Q: A teammate force-pushed to a shared branch and now your local branch has diverged unexpectedly — how would you handle it?
**Answer:** Check `git log` on both to understand what changed, then typically fetch the latest remote state and reset your local branch to match it (`git reset --hard origin/<branch>`) if your own unpushed work isn't important to keep, or otherwise carefully rebase your own commits on top of the new remote history — while raising with the team that force-pushing to a shared branch is generally risky and worth avoiding going forward.

<a id="how-would-you-review-a-large-sprawling-pull-request-that-touches-many-unrelated-things-at-once"></a>
### Q: How would you review a large, sprawling pull request that touches many unrelated things at once?
**Answer:** Ask the author to split it into smaller, focused PRs if practical, since large PRs are harder to reason about and more likely to hide bugs. If it can't be split, review it in logical chunks by file/feature area rather than top to bottom, and focus first on architecture/approach before nitpicking style.

<a id="how-would-you-decide-whether-to-use-git-merge-or-git-rebase-when-integrating-your-feature-branchs-upstream-changes"></a>
### Q: How would you decide whether to use `git merge` or `git rebase` when integrating your feature branch's upstream changes?
**Answer:** Consider whether the branch has already been pushed/shared — rebasing shared branches is risky. For a purely local, not-yet-shared feature branch, rebasing onto the latest main keeps history clean; for shared or already-public branches, merging is the safer default since it doesn't rewrite commits others may depend on.

<a id="you-need-to-make-an-urgent-fix-but-your-working-directory-is-full-of-unrelated-in-progress-changes--how-would-you-handle-it"></a>
### Q: You need to make an urgent fix, but your working directory is full of unrelated in-progress changes — how would you handle it?
**Answer:** Stash the current, unrelated changes with `git stash`, switch to the appropriate base branch, make and commit the urgent fix there, and once it's pushed/handled, switch back to your original branch and reapply your stashed work with `git stash pop`.

<a id="how-would-you-investigate-exactly-when-and-by-whom-a-specific-line-of-buggy-code-was-introduced"></a>
### Q: How would you investigate exactly when and by whom a specific line of buggy code was introduced?
**Answer:** Use `git blame <file>` to see which commit last touched that line, then examine that commit's full diff and message with `git show <hash>`. If the line has been touched by many small commits over time obscuring the real origin, `git log -S"<code snippet>"` can search history for when that exact text was added or removed.

<a id="a-ci-pipeline-is-failing-only-on-a-pull-request-not-on-main--how-would-you-approach-debugging-it"></a>
### Q: A CI pipeline is failing only on a pull request, not on `main` — how would you approach debugging it?
**Answer:** Check the CI logs for the specific failing step, confirm whether the PR branch is actually up to date with the latest `main` (a stale branch can fail against dependencies/config that have since changed), and try reproducing the exact same command locally on the PR branch to rule out an environment-specific difference between local and CI.

<a id="how-would-you-set-up-a-new-team-members-git-workflow-for-contributing-to-a-repository-they-dont-have-direct-write-access-to"></a>
### Q: How would you set up a new team member's Git workflow for contributing to a repository they don't have direct write access to?
**Answer:** Have them fork the repository to their own account, clone their fork locally, add the original repository as an `upstream` remote for pulling in updates, do their work on feature branches within their fork, and open pull requests from those branches back to the original repository's `main`.

---

<a id="how-to-use-this-guide"></a>
## How to Use This Guide

- **A few days before an interview?** Go section by section, top to bottom — each one builds on the last, from basics to internals and workflows.
- **Revising the night before?** Jump straight to 🔥 Most Asked / Tricky Questions, then skim section headers for anything you're unsure about.
- **During quick revision:** Use `Ctrl+F` (or `Cmd+F`) to jump straight to a keyword or topic instead of scrolling.
- **After every interview:** Come back and add any question you got asked that isn't already here — this file is meant to grow with you.

Good luck — you've got this. 🚀
