# Git & GitHub — What I Learned


## 1. Git & Version Control Basics
- **Version control** lets you track changes to files over time and go back to any earlier point if needed.
- **Git vs. GitHub**: Git is the local tool that tracks changes on your machine; GitHub is the cloud platform that hosts Git repositories and enables sharing/collaboration.
- **Local vs. Remote architecture**: your project lives in a local repository on your computer, and can be connected to a remote repository (e.g., on GitHub) to sync work with others.

## 2. Setup
- Installing Git on Windows, Mac, and Linux.
- Verifying the installation and setting up the terminal to work with Git.
- Configuring Git's global **username and email**, which get attached to every commit you make.

## 3. Starting a Project
- Creating a local project folder and files.
- `git init` — turns a regular folder into a Git repository.
- Creating a matching **remote repository on GitHub**.
- `git clone` — downloads a copy of an existing remote repository to your machine.

## 4. Tracking & Staging Changes
- `git status` — shows which files are modified, staged, or untracked.
- `git add` — stages changes so they're included in the next commit.
  - Variations: `git add .` (everything), `git add -A` (everything, including deletions), or adding specific files by name.
- `git reset` — unstages files (removes them from the staging area without discarding the actual edits).

## 5. Committing
- `git commit` — permanently saves the staged changes as a snapshot in the project's history.
- `git reset HEAD` (or similar) — undoes the last commit.
- `git log` — view the full commit history.

## 6. Removing Files
- `git rm` — deletes a file from both the working directory and Git's tracking.
- `git rm --cached` — stops Git from tracking a file, without deleting it from disk.

## 7. Branching
- Branches let you develop features or fixes separately from the main codebase.
- `git checkout` — switch between branches.
- `git merge` — combine changes from one branch into another.
- **Resolving merge conflicts** — manually fixing lines Git couldn't automatically merge.
- **Checking out previous commits** ("time travel") — viewing/restoring the project at an earlier point in history.
- `git diff` — compare differences between commits.

## 8. Working with Remotes (GitHub)
- Understanding **push, fetch, and pull** as the core sync operations between local and remote repos.
- `git push` — upload local commits to GitHub.
- `git fetch` vs `git pull` — fetch downloads remote changes without merging them; pull fetches *and* merges automatically.
- `git restore` — discard uncommitted local changes and revert files back to their last committed state.

## 9. Advanced / Real-World Workflow Tools
- `git stash` — temporarily shelve unfinished, uncommitted work so you can switch context, then reapply it later.
- `git revert` — safely undo a specific commit by creating a new commit that reverses it (keeps history intact, safe for shared branches).
- `git rebase` — reapplies commits on top of another branch to produce a cleaner, linear history.

## 10. Collaboration
- **Pull Requests (PRs)** — the mechanism for proposing that changes from one branch be merged into another on GitHub, enabling code review and discussion before merging.

## Key Takeaway
The course builds up the full everyday Git workflow: initialize/clone a repo → track and stage changes → commit → branch and merge → sync with GitHub via push/pull → use stash, revert, and rebase for real-world situations → collaborate through pull requests. Together these cover essentially the full toolkit a developer needs for day-to-day version control.
