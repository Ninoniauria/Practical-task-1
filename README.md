# Practical-task-1
ninoniauri@Ninos-MacBook-Air Desktop % git version
git version 2.40.0
ninoniauri@Ninos-MacBook-Air Desktop % git config --global user.email ninoniauri3@gmail.com
ninoniauri@Ninos-MacBook-Air Desktop % git config --global user.name "Nino Niauri"
ninoniauri@Ninos-MacBook-Air Desktop % git config --global core.editor mvim  
ninoniauri@Ninos-MacBook-Air Desktop % git config --list
credential.helper=osxkeychain
user.name=Nino Niauri
user.email=ninoniauri3@gmail.com
core.editor=mvim
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true
core.ignorecase=true
core.precomposeunicode=true
ninoniauri@Ninos-MacBook-Air Desktop % mkdir Test
ninoniauri@Ninos-MacBook-Air Desktop % cd Test
ninoniauri@Ninos-MacBook-Air Test % git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint:   git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint:   git branch -m <name>
Initialized empty Git repository in /Users/ninoniauri/Desktop/Test/.git/
ninoniauri@Ninos-MacBook-Air Test % git status on branch master
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
ninoniauri@Ninos-MacBook-Air Test % touch README.txt
ninoniauri@Ninos-MacBook-Air Test % git status on branch master
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
ninoniauri@Ninos-MacBook-Air Test % git add README.txt
ninoniauri@Ninos-MacBook-Air Test % git status on branch master
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
ninoniauri@Ninos-MacBook-Air Test % git add ./README.txt
ninoniauri@Ninos-MacBook-Air Test % git status
On branch master
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.txt

zsh: command not found: On
ninoniauri@Ninos-MacBook-Air Test % git status on branch master
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
ninoniauri@Ninos-MacBook-Air Test % git status
On branch master
On branch master
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.txt

zsh: command not found: On
zsh: command not found: On
ninoniauri@Ninos-MacBook-Air Test % git status
On branch master
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.txt

zsh: command not found: On
ninoniauri@Ninos-MacBook-Air Test % 
ninoniauri@Ninos-MacBook-Air Test % touch README.txt
 git status 
On branch master
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.txt

zsh: command not found: On
ninoniauri@Ninos-MacBook-Air Test % git add ./README.txt
ninoniauri@Ninos-MacBook-Air Test % git status
On branch master
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.txt

zsh: command not found: On
ninoniauri@Ninos-MacBook-Air Test % git commit -m "initial commit"
[master (root-commit) a76de0c] initial commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.txt
ninoniauri@Ninos-MacBook-Air Test % git status
On branch master
On branch master
nothing to commit, working tree clean
zsh: command not found: On
ninoniauri@Ninos-MacBook-Air Test % echo "This's a Test GIT project" > README.txt
ninoniauri@Ninos-MacBook-Air Test % git status
On branch master
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.txt

no changes added to commit (use "git add" and/or "git commit -a")
zsh: command not found: On
ninoniauri@Ninos-MacBook-Air Test % answer: README.txt file become modified: README.txt $
zsh: command not found: answer:
ninoniauri@Ninos-MacBook-Air Test % git commit -a -m "Added README file content"
[master a84b97b] Added README file content
 1 file changed, 1 insertion(+)
ninoniauri@Ninos-MacBook-Air Test % git log --pretty=format:"%h %cd %an '%s'"
a84b97b Mon Mar 27 17:47:09 2023 +0400 Nino Niauri 'Added README file content'
a76de0c Mon Mar 27 17:44:02 2023 +0400 Nino Niauri 'initial commit'
ninoniauri@Ninos-MacBook-Air Test % git log --patch -2
commit a84b97be62c3e97477025e5ade4b56b02b87e303 (HEAD -> master)
Author: Nino Niauri <ninoniauri3@gmail.com>
Date:   Mon Mar 27 17:47:09 2023 +0400

    Added README file content

diff --git a/README.txt b/README.txt
index e69de29..e78a480 100644
--- a/README.txt
+++ b/README.txt
@@ -0,0 +1 @@
+This's a Test GIT project

commit a76de0c772c4d31be45209c297f06fc68f9ec103
:...skipping...
commit a84b97be62c3e97477025e5ade4b56b02b87e303 (HEAD -> master)
Author: Nino Niauri <ninoniauri3@gmail.com>
Date:   Mon Mar 27 17:47:09 2023 +0400

    Added README file content

diff --git a/README.txt b/README.txt
index e69de29..e78a480 100644
--- a/README.txt
+++ b/README.txt
@@ -0,0 +1 @@
+This's a Test GIT project

commit a76de0c772c4d31be45209c297f06fc68f9ec103
Author: Nino Niauri <ninoniauri3@gmail.com>
Date:   Mon Mar 27 17:44:02 2023 +0400

    initial commit

diff --git a/README.txt b/README.txt
new file mode 100644
index 0000000..e69de29
