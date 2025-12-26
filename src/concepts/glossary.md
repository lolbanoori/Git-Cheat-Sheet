# Glossary

## Section 1: Core Concepts & Systems

- **Git**: A free, open-source distributed version control system used to track changes in source code. It handles projects of any size with speed and efficiency.
- **Version Control System (VCS)**: A software tool that records changes to a file or set of files over time so that you can recall specific versions later. It facilitates collaboration and history tracking.
- **Source Code Management (SCM)**: Often used interchangeably with VCS, this refers to tools and processes for managing the source code history and changes.
- **Repository (Repo)**: A data structure (typically a folder) that manages a specific software project, containing all project files and the entire revision history.
- **Remote Repository**: A version of the repository hosted on a server (like GitHub or GitLab) or another computer. It allows for collaboration and off-site backup.
- **GitHub**: A cloud-based hosting service for Git repositories. It adds social collaboration features like bug tracking, feature requests, task management, and wikis.
- **.gitignore**: A text file that tells Git which files or directories to intentionally ignore (not track), such as build artifacts or sensitive API keys.

## Section 2: The Git Workflow (States of a File)

- **Working Directory (Working Tree)**: The local directory on your computer where you are currently editing files. These changes are not yet tracked by Git until staged.
- **Staging Area (Index)**: A virtual preparation area. It is a file maintained by Git that stores information about what changes will go into your next commit.
- **Commit**: A captured snapshot of the project at a specific point in time. It saves the changes currently in the staging area to the local Git history.
- **Tracked Files**: Files that Git is aware of (they were in the last snapshot or have been staged).
- **Untracked Files**: Files in your working directory that Git is not watching.
- **Modified**: A state where a file has been changed but not yet staged or committed.
- **Staged**: A state where a modified file has been marked to be included in the next commit.

## Section 3: Branching & Merging

- **Branch**: A lightweight, movable pointer to a specific commit. It represents an independent line of development (e.g., a new feature) separate from the main project.
- **HEAD**: A special pointer that refers to the local branch you are currently working on (the tip of the current branch).
- **Master / Main**: The default primary branch created when a new repository is initialized. It typically holds the "production-ready" code. (Note: main is the modern standard name, replacing master.)
- **Merge**: The act of taking the contents of a source branch and integrating them with a target branch.
- **Fast-forward Merge**: A merge where the target branch pointer simply moves forward to the latest commit of the source branch because the history is linear (no divergent commits).
- **Three-way Merge**: A merge performed when the branches have diverged. Git uses three snapshots (the two branch tips and their common ancestor) to create a new "merge commit."
- **Merge Conflict**: A state that occurs when Git cannot automatically resolve differences between two branches (typically when the same line of code is modified differently in both).
- **Merge Commit**: A specific type of commit resulting from a three-way merge, possessing two parent commits.

## Section 4: Advanced Git Operations

- **Diff**: A command/output that shows the specific line-by-line differences between two files or commits.
- **Patch**: A file containing a "diff" that can be applied to code to update it.
- **Rebasing**: The process of moving or combining a sequence of commits to a new base commit. It creates a linear history but rewrites the commit history.
- **Interactive Rebase**: A mode of rebasing that allows you to edit, squash, reorder, or drop individual commits to clean up history before merging.
- **Squash Merge**: Combining multiple commits from a feature branch into a single commit when merging into the main branch.
- **Rollback**: The general act of reverting software to a previous stable state.
- **Reset**: A command (git reset) used to undo changes by moving the HEAD pointer to a previous state, potentially modifying the staging area and working directory.
- **Stash**: A temporary storage area for uncommitted changes (dirty working directory) so you can switch branches without losing your work.
- **Forking**: A GitHub-specific concept (not a Git command) where you create a personal copy of someone else's repository to your own account.

## Section 5: Collaboration & Code Quality

- **Pull Request (PR)**: A platform feature (GitHub/GitLab) used to propose changes. You ask the maintainers of a repository to "pull" your changes into their branch.
- **Code Review**: The systematic examination of computer source code by peers to identify bugs, improve coding style, and learn from each other.
- **Pair Programming**: A development technique where two programmers work together at one workstation (one drives/types, the other navigates/reviews).
- **CI/CD (Continuous Integration/Continuous Deployment)**:
    - **CI**: Automatically building and testing code every time a change is committed.
    - **CD**: Automatically releasing changes to production after they pass the CI tests.
- **Pipelines**: A series of automated steps (build, test, deploy) defined in a CI/CD system.

## Section 6: Security & Protocols

- **SSH (Secure Shell)**: A cryptographic network protocol for operating network services securely over an unsecured network.
- **SSH Key Pair**: A pair of cryptographic keys used for authentication:
    - **Public Key**: The key you share with the server (e.g., upload to GitHub). It encrypts data.
    - **Private Key**: The key you keep secret on your local machine. It decrypts data and signs communications.
- **API Key**: A unique identifier used to authenticate a user, developer, or calling program to an API (Application Programming Interface).

\newpage
