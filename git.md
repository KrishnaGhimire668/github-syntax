git installation

git config --global user.name "name"
git config --global user.email "hsnxj@email.com"
git config --global core.editor "code --wait"
git config --global core.autocrlf
git config --global -e(edit)

stages:
U- untracked
A- added or staged
C- Commited

git log --oneline => to know current status of saved points
git status -s => to know current status of unstaged and staged files
git reset --hard HEAD~1(2,3,4)(to go back to previous commit)

