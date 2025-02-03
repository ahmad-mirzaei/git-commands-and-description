<a id="go-to-the-command-list"></a>

# Git Commands & Description

## Description
_[Git](https://git-scm.com/doc) commands are stored in this directory along with their brief descriptions. We welcome translations into other languages._

---

- ### **Translated versions**
    - [Persian Version - فارسی](READMEir.md)

---

### **List of commands**

| Row | Title | Row | Title | Row | Title |
|:-----:|-----|:-----:|-----|:-----:|-----|
| 1 | [Git init](#git-init) | 11 | [Git branch](#git-branch) | 21 |  |
| 2 | [Git status](#git-status) | 12 | `Updating...` ⟲ | 22 |  |
| 3 | [Git add](#git-add) | 13 |  | 23 |  |
| 4 | [Git rm](#git-rm) | 14 |  | 24 |  |
| 5 | [Git commit](#git-commit) | 15 |  | 25 |  |
| 6 | [Git tag](#git-tag) | 16 |  | 26 |  |
| 7 | [Git log](#git-log) | 17 |  | 27 |  |
| 8 | [Git blame](#git-blame) | 18 |  | 28 |  |
| 9 | [Git show](#git-show) | 19 |  | 29 |  |
| 10 | [Git config](#git-config) | 20 |  | 30 |  |

---

<!-- git init -->
## <a id="git-init"></a>
![git-init](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/3624c3706fd890ef4a8584d9e45f1d1651a27bb3/images/create-an-empty-git-repository.png)

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

👈[previous topic](#git-init) &nbsp;&nbsp;&nbsp; 👆[list of commands](#go-to-the-command-list)

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
![git-blame](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/23a05680cf6bd592387e68299797be47dc6add29/images/git-blame.png)

| commands | descriptions |
|-----|-----|
| `git blame [file name]` | Viewing the `author's name` of the codes in the file, the date of entry, and the commit time |
| `git blame -e [file name]` | Viewing the `author's email` of the codes in the file, the date of entry, and the commit time |
| `git blame [file name] -L [start-line],[end-line]` | Viewing the author's details of the code in a file, from one line to another |
| `git blame -L [start-line],[end-line] [file-name]` | It is similar to the previous command with a slight rearrangement of the instructions |
<br />

👈[previous topic](#git-log) &nbsp;&nbsp;&nbsp;👆[list of commands](#go-to-the-command-list)

---

<!-- git show -->
## <a id="git-show"></a>
![git-show](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/42834c805f3cb89302e3e0d94652766b4d0a6087/images/git-show.png)

| commands | descriptions |
|-----|-----|
| `git show` | Viewing all changes in the latest commit |
| `git show [commit-hash]` | Viewing the changes in the specific commit using its commit hash |
| `git show [commit-hash] --stat` | It displays the changes made in the specific commit in a summarized form along with the author's details |
| `git show [commit-hash] --path` | Viewing the actual differences made in the specific commit |
| `git show [tag name]` | Viewing the changes within each tag |
<br />

👈[previous topic](#git-blame) &nbsp;&nbsp;&nbsp;👆[list of commands](#go-to-the-command-list)

---

<!-- git config -->
## <a id="git-config"></a>
![git-config](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/23a93a088f87ae7106cffd3f9f45214ae88ec6fd/images/git-config.png)

| commands | descriptions |
|-----|-----|
| `git config --list` | It displays a list of all the configuration settings currently present in your installed version of Git, such as local settings, global settings, and system settings |
| `git config --local alias.[name] [command-name]` -> `git config --local alias.com commit` | With this command, we can choose shorter and more concise names for Git commands in our local environment |
| `git config --global alias.com commit` | If we want to use an alias across all our projects, we use the word `global` instead of `local`, like in this command where we have shortened **`commit`** to **`com`** |
| `git config --global user.name [your-name]` & `git config --global user.email [your-email]` | Setting the username and email for `all projects` |
| `git config --global user.name` & `git config --global user.email` | Viewing the username or email that we have selected for `all projects` |
| `git config user.name [your-name]` & `git config user.email [your-email]` | Setting the username or email for `a specific project` |
| `git config user.name` or git `config user.email` | Viewing the username or email that we have selected for a specific project |
<br />

👈[previous topic](#git-show) &nbsp;&nbsp;&nbsp;👆[list of commands](#go-to-the-command-list)

---

<!-- git branch -->
## <a id="git-branch"></a>
![git-branch](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/6b54be5ba9a395f603ec67c3020dfe950f1c5a49/images/git-branch.png)

| commands | descriptions |
|-----|-----|
| `git branch` | Viewing the names of the project's branches and the branch we are currently on |
| `git branch -a` | Viewing the list of all branches, including both local and remote branches |
| `git branch origin --delete [branch-name]` | Deleting a remote branch |
| `git branch [new-branch]` | Creating a new branch |
| `git switch [branch-name]` | Switching from one branch to another |
| `git switch -c [new-branch-name]` | Creating a new branch and switching to it |
| `git branch -d [branch-name]` | Deleting a branch that has had no changes made to it after creation |
| `git branch -D [branch-name]` | It is used to delete a branch where changes and commits have been made. You should not be on the branch you want to delete; instead, you need to switch to another branch and then delete the previous branch |
| `git branch -m [new-name]` or `git branch -m [branch-name] [new-name]` | Renaming the desired branch. The second method is used when, for example, we are on branch A and want to rename branch B. In this case, there's no need to switch to branch B |
<br />

👈[previous topic](#git-show) &nbsp;&nbsp;&nbsp;👆[list of commands](#go-to-the-command-list)

---

![Updating](https://github.com/ahmad-mirzaei/git-commands-and-explanations/blob/2c6daafcb71ea5808ce52360a5c333d34733048c/images/updating-coming-soon.gif)