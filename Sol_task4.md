#### Task 1: Save Changes Temporarily with `git stash`

1. When we apply changes into the file without committing

2. Create a new file
```
    echo "Creating new file..." >> temp-file.txt
```

3. View tracked and untracked files
```
    git status
```

4. Stash the changes:  
```
   git stash
```

5. View all stashes as a list format
```
    git stash list
```

#### Task 2: Apply and Drop Stashed Changes

1. To apply recently added stash:  
```
   git stash apply
```
2. To drop recently added stash after applying  
```
   git stash drop
```

3. When we need to apply a specific stash:  
```
   git stash apply stash@{1}
 ```

#### Task 3: Stash Untracked Files

1. Stash changes, including untracked files:  
   ```
   git stash -u
   ```
2. To apply stashed changes including untracked files:  
   ```
   git stash apply
   ```

#### Task 4: Rebase Commits to a New Base














#### Task 12: Add a Remote Repository

1. Add a remote repository URL  
   ```
   git remote add origin https://github.com/username/repo.git
   ```

#### Task 13: Fetch Changes from Remote

1. Fetch the repository without merging  
   ```
   git fetch origin
   ```

2. View fetched branches:  
   ```
   git branch -r
   ```

#### Task 14: Pull Changes from Remote

1. To pull the latest changes from the remote repository  
   ```
   git pull origin main
   ```

#### Task 15: Push Changes to Remote

1. Push changes to the  repository:  
   ```
   git push origin main
   ```

2. Push a new branch in the repository:  
   ```
   git push origin feature-branch
   ```

#### Task 16: Delete Remote Branch

1. To delete a remote branch:  
   ```
   git push origin --delete feature-branch
   ```

#### Task 17: Fork a Repository on GitHub

1. Open github and go to the repository and then click the "fork" button 

2. Clone the repository into your local device
```
    git clone "url"
```
#### Task 18: Make Changes and Commit

1. Create a new branch in your repository
``` 
    git checkout -b feature
```

2. Make some changes and commit them
```
    git add README.md
    git commit -m "commited"
```

#### Task 19: Push Changes to Your Fork

1. Then after push the changes to your fork repository:  
```
   git push origin fix-typo
```

#### Task 20: Create a Pull Request

1. Go to the forked repository and click "create pull request" and add some title and discription


#### Task 21: Sync Your Fork with the Original Repository
1. Add the original repository as a remote source:  
   ```bash
   git remote add upstream url
   ```

2. Fetch changes from the original repository:  
   ```bash
   git fetch upstream
   ```

3. Merge changes from the original repository into your local branch:  
   ```bash
   git checkout main
   git merge upstream/main
   ```

4. Push the changes to your fork:  
   ```bash
   git push origin main
   ```
