# Git Commands & Explanations

## Description
_[Git](https://git-scm.com/doc) commands are stored in this directory along with their brief descriptions. We welcome translations into other languages._

---

- **Translated versions**
    - [Persian Version - فارسی](READMEir.md)

---

<!-- git init -->
![create-an-empty-git-repository](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/3624c3706fd890ef4a8584d9e45f1d1651a27bb3/images/create-an-empty-git-repository.png)

| commands | descriptions |
|-----|-----|
| `git init` | introducing the project to Git or initializing it |
| `git` | observe git commands |
<br />

---

<!-- git status -->
![git-status](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/09b16830daf385e596a8dbb4cb741334f3a3ec06/images/GIT%20STATUS.png)

| commands | descriptions |
|-----|-----|
| `git status` | Viewing the current status of project files |
| `git status --short` | View the summary of the current project file status |
| `git status -s` | View the summary of the current project file status |
<br />

---

<!-- git add -->
![git-add](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/731249e7b065c208a7606d7b398ce2bac41d26b1/images/git-add.png)

| commands | descriptions |
|-----|-----|
| `git add [file-name]` | it takes the selected file to the `staging area` |
| `git add .` | it takes all files and project changes to the `staging area` |
| `git add -A` | it takes all files and changes of the project to the staging area, just like the previous command |
| `git add *.AnExtension` -> `git add *.css` | it takes all of the files with the selected extension to the `staging area` |
<br />

---

<!-- git rm -->
![git-rm](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2d029aca4b8234e9bac1727223c84d3c6035a776/images/git-rm.png)

| commands | descriptions |
|-----|-----|
| `git rm [file name]` or `git rm -r [file name]` | it removes the selected file from the project |
| `git rm -- *.AnExtension` -> `git rm -- *.py` | it removes all files that have the selected extension from the project |
| `git rm --cached --ignore-unmatch *.js` | it ignores all the files with the selected extension and takes it to the [working directory] |
| `git rm --cached [file name]` -> `git rm --cached .` | it takes the file or all the files that have gone to the staging area to the [working directory] |
| `git rm -rf --cached .` | it tkes all the files from `the local repository` to `working directory` |
<br />

---

<!-- git commit -->
![git-commit](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/40f6b1ea94378e16c2cb3bf4650311dfe4578c10/images/git-commit.png)

| commands | descriptions |
|-----|-----|
| `git commit -m [message]` | it takes staging area changes to the repository with a related message |
| `git commit -m [message]` | it takes the files that are already created in the project (and the files which are chainging) directly to the repository;  But if a file is newly created, it must first be added to the staging area and then added to the repository with the suitable commit <br /> `new file --> git add "file name" --> git commit -m "message"` <br /> `modified file --> git commit -am "message" --> git commit -a -m "message"`|
| `git commit --amend -m [message]` | Renaming the last commit |
| `git commit --amend -am [message]` or `git commit --amend -a -m [message]` | it adds the last working directory changes to the last commit |
<br />

---

<!-- git tag -->
![git-tag](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/9f84915a653decde5acb2d4124e12ad06e610a05/images/git-tag.png)

| commands | descriptions |
|-----|-----|
| `git tag` or `git tag -l` | Displays the list of tags in the project |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
<br />

---