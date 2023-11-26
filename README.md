# How to create new repository:
This is a list of instructions, which will help you to create a new repository in git, add new branch and commit file changes.

## Initialization
- Create new folder for git repository on the local machine by typing from console **git init new-project**. This will create a git repo inside your current folder.
- Go into this repo with **cd new-project**
- Provide your personal info for git by typing **git config --global user.name "your_name"** and **git config --global user.email your_email**
- Check your current branch with **git branch** --> Should be **main**. If not --> type **git config --global init.defaultBranch "main"**.

## First commit
- Create a new file with name README.md. Add inside init text for first commit. You can do it with **echo 'init' > README.md** or by creating this file manually (with **touch** or **vim** command) and by adding some text inside.
- To check status type **git status**
- To add REAMDE.md to git type **git add README.md**
- For first commit type **git commit -m 'init'** (-m --> means Message).

## Create development branch and save changes
- To create new branch with name "developer" type **git checkout -b development**. This will create new branch from existed "main" and jump inside.
- Update README.md file or add additional files to the repo. Save results with **git add** and **git commit -m 'Developers changes'**.
- Go back into main branch with **git checkout master**.
- Add developer changes by typing **git merge development**.
- Type **git log** to check for latest commits.

## Results
As a result we created new repo with two branches and separate commits inside. In future we can use **development** branch to add new features without touching **main** files.
