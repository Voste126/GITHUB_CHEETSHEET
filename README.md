# GITHUB_CHEETSHEET

## getting started with git and github

## Module 2 Cheat Sheet: Git Commands and Managing GitHub Projects

## Git Commands in DevOps

| Command               | Description                                        | Code Example                              |
|-----------------------|----------------------------------------------------|-------------------------------------------|
| `git add`             | Used to move changes from the working directory to the staging area | `git add sample.md`                      |
|                       | Allows to move the changed files into the staging area on GitHub repositories | `git add .`                            |
| `git am`              | Used to apply patches emailed to the repository    | `git am <patchfile.patch>`                |
| `git branch`          | Allows to create an isolated environment within the repository to make changes | `git branch <new-branch>`             |
| `git checkout`        | Allows to see and change existing branches         | `git checkout <existing-branch>`          |
|                       | Allows to switch to the main branch                | `git checkout main`                       |
| `git clone`           | Allows to create a copy of the remote repository   | `git clone <repository-url>`              |
| `git commit`          | Allows you to take staged snapshots of changes and commit them to the project | `git commit -m "Your commit message here"` |
| `git config --global user.email` | Sets a global email configuration for Git  | `git config --global user.email "your.email@example.com"` |
|                       | Sets a global username configuration for Git       | `git config --global user.name "Your Name"` |
| `git daemon`          | Used to allow anonymous download from the repository | `git daemon --reuseaddr --verbose`    |
| `git diff`            | Helps others to review your code to identify and compare the changes | `git diff example.txt`                |
| `git fetch`           | Used to transfer the changes from the remote repo to your local repo | `git fetch <options> <remote name> <branch name>` |
|                       | Used to grab upstream branches                     | `git fetch upstream master:upstream-master` |
| `git format-patch`    | Generates or prepares e-mail submission if you adopt Linux kernel-style public forum workflow | `git format-patch -n <number_of_commits>` |
| `git http-backend`    | Provides a server-side implementation of Git-over-HTTP, allowing both fetch and push services | `git clone --bare /path/to/repos/myrepo.git`\|`cd myrepo.git`\|`git update-server-info` |
| `git init`            | Used to clone an existing repository               | `git init <directory>`                    |
| `git instaweb`        | Allows to set up web front-end to Git repositories | `git instaweb -p 8080`                    |
| `git log`             | Enables to browse previous changes to a project    | `git log -p filename`                     |
|                       | Shows the commit history with diff outputs         | `git log -p`                              |
|                       | Displays a graph of commits                        | `git log --graph`                         |
|                       | Shows a summary of commits                         | `git log --oneline`                       |
| `git merge`           | Used to merge changes in the active branch into another branch | `git merge feature_branch`             |
|                       | Merges changes from the 'upstream/master' branch to the current branch | `git merge upstream/master`        |
| `git pull`            | Used to transfer the changes from the remote repo to your local repo, and merge them to a branch | `git pull origin main`                |
|                       | Pulls changes from a downstream repository, specifically from the master branch of that repository | `git pull downstream main`         |
|                       | Pulls changes from the "upstream" repository into the current branch | `git pull upstream main`            |
| `git push`            | Used to push all the committed changes into the repository | `git push origin your_branch_name`     |
| `git remote`          | A command to manage a set of tracked repositories  | `git remote add upstream https://github.com/original/repo.git` |
|                       | Adds a remote repository named "origin" with the specified URL | `git remote add origin https://github.com/yourusername/your-repo.git` |
|                       | Adds the original repository as a new remote repository labeled upstream | `git remote add upstream https://github.com/original/repo.git` |
| `git remote rename`   | Renames a remote repository                        | `git remote rename origin new-origin`     |
| `git remote -v`       | Allows to view the remotes associated with the local repository | `git remote -v`                       |
| `git request-pull`    | Creates a summary of changes for your upstream to pull | `git request-pull origin/main your-branch` |
|                       | Generates a summary of pending changes for an email request | `git request-pull <base> <head> <repository>` |
| `git rerere`          | Reuses recorded resolution of previously resolved merge conflicts | `git rerere` \| `git rerere diff`    |
| `git reset`           | Undoes changes that were made to the files in your working directory | `git reset HEAD~1`                   |
| `git revert`          | Used to undo botched commits                       | `git revert HEAD`                        |
| `git shell`           | Used as a restricted login shell for shared central repository users | `sudo usermod -s /usr/bin/git-shell gituser` |
| `git status`          | Allows to see the state of your working directory and the staged snapshot of the changes | `git status`                       |
| `git tag`             | Used to create, list, delete, or verify a tag object signed with GPG | `git tag -a v1.0 -m "Version 1.0"`   |
|                       | Lists all tags                                      | `git tag`                                |
|                       | Deletes a tag                                       | `git tag -d <tag_name>`                  |
|                       | Shows information about the given tag               | `git show <tag_name>`                    |
|                       | Verifies the GPG signature of a tag                 | `git tag -v <tag_name>`                  |
|                       | Lists tags that match a specific pattern            | `git tag -l 'v1.*'`                      |
|                       | Creates a lightweight tag                          | `git tag v1.0`                           |
|                       | Pushes all tags to remote repository                | `git push --tags`                        |
| `git version`         | Displays the current Git version installed on your system | `git --version`                      |
| `git web`             | Provides a web front-end to Git repositories        | `git instaweb --port=8080`               |
| `git send-email`      | Sends your email submission without corruption by your MUA | `git send-email --to=recipient@example.com path/to/patchfile.patch` |
|                       | Sends a collection of patches as emails             | `git send-email --to=recipient@example.com patches/*.patch` |
| `git stash`           | Temporarily shelves (or stashes) changes you've made to your working directory so you can work on something else and then come back and re-apply them later | `git stash` |
|                       | Applies the stashed changes                        | `git stash apply`                       |
|                       | Lists all stashes                                   | `git stash list`                         |
|                       | Drops a specific stash                              | `git stash drop stash@{0}`               |
|                       | Pops the most recent stash and applies it           | `git stash pop`                          |
|                       | Creates a new branch from the stashed changes       | `git stash branch <branch_name>`         |
| `git rebase`          | Allows to reapply commits on top of another base tip | `git rebase <base>`                     |
|                       | Interactively rebase                                | `git rebase -i <commit>`                 |
| `git bisect`          | Helps to find the commit that introduced a bug by binary search | `git bisect start` \| `git bisect bad` \| `git bisect good <commit>` |
| `git cherry-pick`     | Applies the changes introduced by some existing commits | `git cherry-pick <commit>`            |
| `git blame`           | Shows what revision and author last modified each line of a file | `git blame <file>`                    |
| `git clean`           | Removes untracked files from the working directory  | `git clean -f`                           |
| `git archive`         | Creates an archive of files from a named tree       | `git archive --format=tar <commit> <path>` |

### THESE ARE THE BLUEPRINT COMMANDS FOR DEVOPS Developers
