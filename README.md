<a id="go-to-the-command-list"></a>

# Git Commands & Description

## Description
_[Git](https://git-scm.com/doc) commands are stored in this directory along with their brief descriptions. We welcome translations into other languages._

---

- ### **Translated versions**
    - [Persian Version - فارسی](READMEir.md)

---

- ### **List of commands**
    - [Create empty repository](#create-empty-repository) 
    - [Git status](#git-status) 
    - [Git add](#git-add) 
    - [Git rm](#git-rm) 
    - [Git commit](#git-commit) 
    - [Git tag](#git-tag) 
    - [Git log](#git-log) 

---

<!-- git init -->
## <a id="create-empty-repository"></a>
![create-empty-repository](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/3624c3706fd890ef4a8584d9e45f1d1651a27bb3/images/create-an-empty-git-repository.png)

| commands | descriptions |
|-----|-----|
| `git init` | introducing the project to Git or initializing it |
| `git` | observe git commands |
<br />

👆[list of commands](#go-to-the-command-list)

---

<!-- git status -->
## <a id="git-status"></a>
![git-status](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/09b16830daf385e596a8dbb4cb741334f3a3ec06/images/GIT%20STATUS.png)

| commands | descriptions |
|-----|-----|
| `git status` | Viewing the current status of project files |
| `git status --short` | View the summary of the current project file status |
| `git status -s` | View the summary of the current project file status |
<br />

👈[previous topic](#create-empty-repository) &nbsp;&nbsp;&nbsp; 👆[list of commands](#go-to-the-command-list)

---

<!-- git add -->
## <a id="git-add"></a>
![git-add](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/731249e7b065c208a7606d7b398ce2bac41d26b1/images/git-add.png)

| commands | descriptions |
|-----|-----|
| `git add [file-name]` | it takes the selected file to the `staging area` |
| `git add .` | it takes all files and project changes to the `staging area` |
| `git add -A` | it takes all files and changes of the project to the staging area, just like the previous command |
| `git add *.AnExtension` -> `git add *.css` | it takes all of the files with the selected extension to the `staging area` |
<br />

👈[previous topic](#git-status) &nbsp;&nbsp;&nbsp;👆[list of commands](#go-to-the-command-list) 

---

<!-- git rm -->
## <a id="git-rm"></a>
![git-rm](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2d029aca4b8234e9bac1727223c84d3c6035a776/images/git-rm.png)

| commands | descriptions |
|-----|-----|
| `git rm [file name]` or `git rm -r [file name]` | it removes the selected file from the project |
| `git rm -- *.AnExtension` -> `git rm -- *.py` | it removes all files that have the selected extension from the project |
| `git rm --cached --ignore-unmatch *.js` | it ignores all the files with the selected extension and takes it to the [working directory] |
| `git rm --cached [file name]` -> `git rm --cached .` | it takes the file or all the files that have gone to the staging area to the [working directory] |
| `git rm -rf --cached .` | it tkes all the files from `the local repository` to `working directory` |
<br />

👈[previous topic](#git-add) &nbsp;&nbsp;&nbsp;👆[list of commands](#go-to-the-command-list)

---

<!-- git commit -->
## <a id="git-commit"></a>
![git-commit](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/40f6b1ea94378e16c2cb3bf4650311dfe4578c10/images/git-commit.png)

| commands | descriptions |
|-----|-----|
| `git commit -m [message]` | it takes staging area changes to the repository with a related message |
| `git commit -am [message]` or `git commit -a -m [message]` | it takes the files that are already created in the project (and the files which are chainging) directly to the repository;  But if a file is newly created, it must first be added to the staging area and then added to the repository with the suitable commit <br /> `new file --> git add "file name" --> git commit -m "message"` <br /> `modified file --> git commit -am "message" --> git commit -a -m "message"`|
| `git commit --amend -m [message]` | Renaming the last commit |
| `git commit --amend -am [message]` or `git commit --amend -a -m [message]` | it adds the last working directory changes to the last commit |
<br />

👈[previous topic](#git-rm) &nbsp;&nbsp;&nbsp;👆[list of commands](#go-to-the-command-list)

---

<!-- git tag -->
## <a id="git-tag"></a>
![git-tag](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/9f84915a653decde5acb2d4124e12ad06e610a05/images/git-tag.png)

| commands | descriptions |
|-----|-----|
| `git tag` or `git tag -l` | Displays the list of tags in the project |
| `git tag [tag name]` -> `git tag 3.12.0` | if we put a version or a special name in front of the command, it will be considered for the last commit |
| `git tag 3.13.0 [commit-hash]` -> `git tag v5.2.0 6d2ef95` | By putting the version or a name for the tag plus the hash coad of the selected commit, we can tag our commits |
| `git show [tag name]` -> `git show 3.13.2` | Viewing the changes in every tag |
| `git tag -d [tag name]` -> `git tag -d 3.12.2` | Removing the tag |
| `git tag -f [tag name] [commit-hash]` -> `git tag -f v2.1.1 6d2ef95` | Removing a tag name from one comit and put the same name for another comite |
| `git tag -l '13.*'` - `git tag -l '*.0'` - `git tag -l '*.1.*'` | Searching in tags |
<br />

👈[previous topic](#git-commit) &nbsp;&nbsp;&nbsp;👆[list of commands](#go-to-the-command-list)

---

<!-- git log -->
## <a id="git-log"></a>
![git-log](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/94a989c252f295535c78e677fce6af6b9d2dd0e2/images/git-log.png)

| commands | descriptions |
|-----|-----|
| `git log` | it returns the changes and commits of the project |
| `git log --oneline` | it returns the changes and commits of the project in a summarized and short form |
| `git log --oneline --all` | viewing all commits and seeing the position of origin and head |
| `git log --stat` | it reverts the project changes completely |
| `git log --graph` | it returns the commit information graphically |
| `git log --graph --oneline` | it returns the commits in a graphic , detailed and summeraized way |
| `git log --after="25-10-12"` | it returns the commits after a specified date |
| `git log --before="25-10-12"` | it returns the commits before a specified date |
| `git log --author="user-name"` | it returns the commits of the selected author or user along with the date and time of their insertion |
<br />

👈[previous topic](#git-tag) &nbsp;&nbsp;&nbsp;👆[list of commands](#go-to-the-command-list)

---


<!-- git blame -->
## <a id="git-blame"></a>
![git-blame]()

| commands | descriptions |
|-----|-----|
| `git blame [file name]` | Viewing the `author's name` of the codes in the file, the date of entry, and the commit time |
| `git blame -e [file name]` | Viewing the `author's email` of the codes in the file, the date of entry, and the commit time |
| `git blame [file name] -L [start-line]` | Viewing the author's details of the code in a file, from one line to another |
| `` |  |
<br />

👈[previous topic](#git-tag) &nbsp;&nbsp;&nbsp;👆[list of commands](#go-to-the-command-list)

---

![Updating](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2c6daafcb71ea5808ce52360a5c333d34733048c/images/updating-coming-soon.gif)