# Tips

- Use `switch` instead of `branch` and `checkout`

# Commands

- `git switch -c <branchName>` = Create new branch if it doesn't exist and switch to it
- `git swithc <branchName>` = Switch to another branch
- `git reset --hard` = discard all current changes and go back to last commit in this branch
- `git reset --hard <commitHash>` = discard all current changes adn go back to the commit with the hash commitHash
- `git fetch` = Downloads copies of all the contents from remote repo
- `git log -n 10` = Limit the number of commits show by log to 10
- `git push origin <localbranch>:<remotebranch>` = push changes from local branch to remote branch
- `git push origin :<remotebranch>` = delete remote branch
- `git pull [<remote>/<branch>]` = pulls changes from repo (you have the option to specify which ones) to our local repo
- `git merge <otherbranch>` = merge current branch with otherbranch

# Workflow

1. Update local `main` branch = `git pull origin main`
2. Checkout a new branch for the changes you want to make = `git switch -c <newBranch>`
3. Make changes to files
4. Commit changes = `git add. && git commit -m "<msg>"`
5. Push changes (preferably push them to a new branch, not main) = `git push origin <newBranch>`
6. Open pull request to merge `newBranch` into `main`
7. Ask someone to review your pull request
8. Once approved, merge them
9. Delete feature branch = `git push origin:<newBranch> && git branch -d <newBranch>`