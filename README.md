# JEST internal workshop &#8594; Git + GitHub

Internal training workshop to introduce Git and GitHub.

## Requirements

- Installing [Git](https://github.com/git-guides/install-git) and [GitHub](https://docs.github.com/pt/free-pro-team@latest/github/teaching-and-learning-with-github-education/applying-for-a-student-developer-pack) account.

## Installation

1. Install [Git](https://github.com/git-guides/install-git).
1. Create a [GitHub](https://docs.github.com/pt/free-pro-team@latest/github/teaching-and-learning-with-github-education/applying-for-a-student-developer-pack) account.

Git was installed? At the terminal:

```bash
git --version
```

Git setup:

```bash
# set your name for version history
git config --global user.name “[firstname lastname]”
# set your email for version history
git config --global user.email “[valid-email]”
# set automatic staining of command line for Git
git
```

## Topics

- [ ] `git init` - create a Git repository.
- [ ] `git add [file]` - add or update changes.
  - [ ] `git add .` - add all updates in working directory.
- [ ] `git commit -m “[descriptive message]”` - commit your added content.
- [ ] `git status` - show modified files in working directory.
- [ ] `git log` - show all commits in the current branch’s history.
- [ ] `git show` - show modified files in working directory.
- [ ] `git branch` - manage your branches.
  - [ ] `git branch [branch]` - create a new branch.
  - [ ] `git branch -D [branch]` - delete a branch.
- [ ] `git checkout [branch]` - switch to another branch.
  - [ ] `git checkout -b [branch]` - create a branch and switch to it.
- [ ] `git merge` - merge branches.
- [ ] `git push` - transmit local branch commits to the remote repository branch.
- [ ] `git clone [url]` - clone a remote repository.
- [ ] `git pull` - pull from the remote repository.

## Advanced Topics

- [ ] Ignoring files
  - create a file named .gitignore (linux: `touch .gitignore`)
  - `git rm --cached [filename]` - file to ignore.
  - see [gitignore.io](https://www.gitignore.io/) and [github/gitignore](https://github.com/github/gitignore) for more information.
- [ ] recovery deleted file.
  - `git log` (look for the commit where the file was deleted)
  - `git checkout [checkpoint] -- filename`
- [ ] adding an existing project to GitHub.
  - `git init -b main` - create a new project.
  - `git commit -m "First commit"` - add files and commit.
  - `git remote add origin [remote repository URL]` - sets the new remote repository.
  - `git remote -v` - to view the remote repository.
  - `git push origin main` - push local changes to remote repository.
- [ ] workflow to contribute to an open source project (from reference [4])
  - fork the repository to your account.
  - `git clone https://github.com/your-username/name-of-repo.git` - clone.
  - `cd name-of-repo` - enter into folder.
  - `git remote add upstream https://github.com/not-your-username/name-of-repo.git`
  - `git status && git remote -v` - view remote and local branch.
  - `git fetch upstream` - manually sync up with upstream.
  - `git branch --set-upstream-to=upstream/master master` - fix master folder to use git pull.
  - `git pull` - manually sync up with upstream.
  - `git checkout -b my_feature_name` - create your features.
  - `git commit -m "description of fix"` - commit your changes.
  - `git push origin feature-branch` - push your feature branch to remote repository.
  - `git branch -D my_feature_name` - delete local branch.
  - `git push origin --delete my_feature_name` - delete you branch from remote repository.

## Complementary material

- [1] [Git Guide](https://github.com/git-guides/) - Explanation of almost everything you need on github.
- [2] [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf) - A quick reference to the Github commands.
- [3] [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/) - A quick reference to the Markdown syntax.
- [4] [Open Source Git Workflow](https://dev.to/adamreidelbach/open-source-git-workflow-an-overview-2oo2)

This workshop uses complementary materials 1 and 2 as a source.

## License

[MIT](LICENSE) © [Tamagusko](https://tamagusko.github.io/) & [JEST](https://jest.pt/).
