# GIT_COM
Some useful git tips and commands.

**Some Tips:**
- One feature one branch.
- It is possible to name github repo differently as local project dir.
- To work on a project (improvement) fork the repo, create a new branch and then create a pull request.
- It is possible to choose an Assignee in case of a new issue.
- Check if someone is already working on an issue before working on it.
- how to write useful commits: https://dev.to/jacobherrington/how-to-write-useful-commit-messages-my-commit-message-template-20n9

## Git Commands:
1. Initialize a git project (to be run in the project directory)
```
git init
```
2. Add multiple files for the commit
```
git add <file1> <file2> <file3>
```
3. Commit the added files 
```
git commit -m "Commit message"
```
4. Create a new branch 
```
git branch <new_branch>
```
5. Show all available branches 
```
git branch
```
6. Switch to an existing branch
```
git checkout <branch_name>
```
7. Check logs of a certain branch
```
git log <branch_name>
```
8. Check differences between two branches
```
git diff <branch1> <branch2>
```
9. Merge: Move to the branch in which you want the merge to be done (e.g master) and merge the 'feature' branch
```
git checkout <master>
git merge <feature_branch>
```
10. Delete an existing branch (Be careful with it !!)
```
git branch --delete <branch_name>
```
11. Add remote server to a local git project (First create a repo in github)
```
git remote add origin <ssh_https_links_to_repo> 
```
12. Push local codes to remote server (Github)
```
git push <remote> <branch>
```
13. Pull changes from remote server 
```
git pull <remote> <branch>
```



