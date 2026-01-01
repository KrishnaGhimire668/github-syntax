
## Section 1: Configuration 

# git config --global user.name "name" =>  Sets your professional identity.
# git config --global user.email "email" =>  Sets your contact email for commits.
# git config --global core.editor "code --wait" =>  Sets VS Code as your default editor for Git.
# git config --global init.defaultBranch main =>  Ensures all new projects start with 'main' branch.
# git config --global credential.helper store => Remembers your login token so you don't type it every time.
# git config --global core.autocrlf input => Fixes line-ending issues between different operating systems.


## Section 2: Starting a Project 

# git init  => Creates a new local Git repository.
# touch .gitignore  => Creates a file to exclude secret files like node_modules and .env.
# git add .  => Stages all files in the current folder for the first commit.
# git commit -m "chore: initial setup" =>  Officially saves your project's starting code.
# git remote add origin <url> =>  Links your local folder to your GitHub repository URL.
# git push -u origin main => Uploads your code and sets the link between local and remote main.


# Section 3: When working on a specific task

# git checkout main && git pull origin main => Syncs your local main with the latest team code.
# git switch -C feat/add-user-auth => Creates and switches to a new branch for a specific feature.
# git status -s => Shows a quick, short summary of which files you modified.
# git diff =>  Shows the exact line-by-line changes you made in your code.
# git add . =>  Stages all your current progress to prepare for a save.
# git commit -m "feat: implement JWT login" => Saves your work with a professional message prefix.
# git push origin feat/add-user-auth => Uploads your branch to GitHub to open a Pull Request.


# Section 4: When the main branch has new team updates

# git checkout main && git pull origin main -> Updates your local main branch with the team's latest code.
# git checkout feat/my-feature && git rebase main -> Moves your work to the very top of the new main history.
# git add . -> Stages your conflict fixes after you resolve them in VS Code.
# git rebase --continue -> Tells Git to finish the rebase after you have fixed conflicts.
# git push origin feat/my-feature --force-with-lease -> Safely updates your GitHub branch after history changes.




# Section 5: Emergency & History (When you make a mistake or need context)

# git stash -> Hides your unfinished code changes to switch branches quickly.
# git stash pop -> Brings back your hidden code so you can continue working.
# git reset --soft HEAD~1 -> Undoes the last commit but keeps your code changes in the editor.
# git reset --hard HEAD~1 -> Deletes the last commit and all work inside it (Permanent).
# git checkout -- <file> -> Discards changes in one specific file to match the last saved version.
# git reflog -> Shows every single action you've taken in Git (The ultimate "Undo" list).
# git log --oneline --graph --all -> Shows a visual map of all your branches and history.


# Section 6: When a feature is finished and merged

# git branch -> Lists all your current local branches.
# git branch -d feat/name -> Deletes a branch safely after it has been merged.
# git branch -D feat/name -> Forces a branch deletion even if it wasn't merged.