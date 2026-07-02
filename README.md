# Pull Request Practice

## What I Learned

This project helped me practice the basic GitHub pull request workflow. I learned how branches, commits, pushing, pull requests, merging, and cleanup all connect together when working with a repository.

I also learned the difference between **forking** and **cloning** a repository.

A **fork** creates a copy of someone else's repository under my own GitHub account. This is useful because I usually do not have permission to push changes directly to someone else's original repository.

A **clone** downloads a repository from GitHub onto my computer so I can work on the files locally.

The reason for forking first and then cloning is to create a GitHub copy that I am allowed to push changes to. After making changes locally on my computer, I can push those changes to my fork and then create a pull request to suggest those changes to the original repository.

The workflow looks like this:

```text
Original repo -> My fork -> My computer
```

Then after making changes:

```text
My computer -> My fork -> Pull request to original repo
```

A repository can usually be cloned without forking if the repository already belongs to me or if I have permission to push directly to it.

## Skills Practiced

* Create and switch to a new branch
* Make changes to a file
* Stage changes using `git add .`
* Commit changes with a message
* Push a branch to GitHub
* Open a pull request
* Compare changes between branches
* Merge a pull request into the main branch
* Close pull requests that are no longer needed
* Delete unused branches after they are merged or no longer needed
* Understand the difference between forking and cloning
* Push changes from a local computer to a fork
* Create a pull request from a fork into the original repository

## Commands I Practiced

```bash
git clone https://github.com/username/repository-name.git
cd repository-name
git status
git branch
git checkout -b branch-name
git switch -c branch-name
git add .
git commit -m "commit message"
git push --set-upstream origin branch-name
git push -u origin branch-name
git pull origin main
git branch -d branch-name
git branch -D branch-name
```

## Pull Request Flow

For this workflow, the pull request usually goes from a fork and branch into the original repository's main branch.

```text
FROM: my fork and my branch
INTO: the original repository and its main branch
```

Example:

```text
FROM: bracytrae/github-chapter-2-contributions, branch: final-exercise-bracytrae
INTO: codedex-io/github-chapter-2-contributions, branch: main
```

This allows the original repository owner to review the changes before deciding whether to merge them.

## Credit

Credit to CodeDex for the Git and GitHub course material this pull request practice is based on.

## Reflection

This practice helped me understand that GitHub is not just about saving code. It is also about organizing changes, working safely on branches, and keeping a project clean after changes are merged.

The biggest thing I learned is that branches let me experiment without directly affecting the main version of a project. Forks make it possible to contribute to repositories I do not own, and pull requests make it possible to suggest changes in an organized way.
