# Git Commands

## Basic Commands

1. **Initialize a Git repository**
    ```bash
    git init
    ```

2. **Clone a repository**
    ```bash
    git clone <repository_url>
    ```

## Configuration

3. **Configure user information**
    ```bash
    git config --global user.name "Your Name"
    git config --global user.email "your.email@example.com"
    ```

4. **View configuration**
    ```bash
    git config --list
    ```

## Add and Commit

5. **Add changes to the staging area**
    ```bash
    git add <file>
    git add .
    ```

6. **Commit changes**
    ```bash
    git commit -m "Your commit message"
    ```

## Branching

7. **Create a new branch**
    ```bash
    git branch <branch_name>
    ```

8. **Switch to a branch**
    ```bash
    git checkout <branch_name>
    ```

9. **Create and switch to a new branch**
    ```bash
    git checkout -b <new_branch_name>
    ```

## Merge and Rebase

10. **Merge branches**
    ```bash
    git merge <branch_name>
    ```

11. **Rebase branches**
    ```bash
    git rebase <branch_name>
    ```

## Remote Repositories

12. **Add a remote repository**
    ```bash
    git remote add <remote_name> <remote_url>
    ```

13. **Fetch changes from a remote repository**
    ```bash
    git fetch <remote_name>
    ```

14. **Pull changes from a remote repository**
    ```bash
    git pull <remote_name> <branch_name>
    ```

15. **Push changes to a remote repository**
    ```bash
    git push <remote_name> <branch_name>
    ```

## Undoing Changes

16. **Discard changes in the working directory**
    ```bash
    git checkout -- <file>
    ```

17. **Undo the last commit**
    ```bash
    git reset HEAD^
    ```

18. **Undo the last commit and discard changes**
    ```bash
    git reset --hard HEAD^
    ```

## Log and Status

19. **View commit history**
    ```bash
    git log
    ```

20. **View changes in the working directory**
    ```bash
    git status
    ```

# Pushing a New Project Using Git

To push a new project using Git, follow these steps. Replace placeholders such as `<repository_url>` and `<branch_name>` with your actual repository URL and branch name.

1. **Initialize a Git repository (if not done already):**
    ```bash
    git init
    ```

2. **Add and commit your initial changes:**
    ```bash
    git add .
    git commit -m "Initial commit"
    ```

3. **Add a remote repository:**
    ```bash
    git remote add origin <repository_url>
    ```

   Replace `<repository_url>` with the URL of your remote repository.

4. **Push the changes to the remote repository:**
    ```bash
    git push -u origin <branch_name>
    ```

   Replace `<branch_name>` with the branch you want to push. The `-u` flag sets the upstream branch, linking the local branch to the remote branch.

   If you are pushing to the main branch (commonly named `main` or `master`), the command might look like:
    ```bash
    git push -u origin main
    ```

5. **Enter your credentials if prompted.**

After these steps, your new project should be pushed to the remote repository.

Remember that these commands are generic, and the exact steps may vary depending on the specific platform you are using (GitHub, GitLab, Bitbucket, etc.) and your branch naming conventions. Always check the documentation of the platform you're using for any additional steps or requirements.
