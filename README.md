# Story

Last login: Fri May  8 06:53:31 on console

The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
Mac-mini-de-Rodolphe:~ rodolphedupuy$ cd Desktop
Mac-mini-de-Rodolphe:Desktop rodolphedupuy$ mkdir Story
Mac-mini-de-Rodolphe:Desktop rodolphedupuy$ cd Story
Mac-mini-de-Rodolphe:Story rodolphedupuy$ ls
Mac-mini-de-Rodolphe:Story rodolphedupuy$ touch chapter1.txt
Mac-mini-de-Rodolphe:Story rodolphedupuy$ open chapter1.txt
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git init
Initialized empty Git repository in /Users/rodolphedupuy/Desktop/Story/.git/
Mac-mini-de-Rodolphe:Story rodolphedupuy$ ls -a
.		..		.git		chapter1.txt
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	chapter1.txt

nothing added to commit but untracked files present (use "git add" to track)
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git add chapter1.txt
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   chapter1.txt

Mac-mini-de-Rodolphe:Story rodolphedupuy$ git commit -m "Completed Chaptern 1"
[master (root-commit) 0b85f39] Completed Chaptern 1
 1 file changed, 1 insertion(+)
 create mode 100644 chapter1.txt
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git log
commit 0b85f395f797c331fb004342908f6ec4a7593347 (HEAD -> master)
Author: Rodolphe DUPUY <rodolphe.dupuy@free.fr>
Date:   Fri May 8 11:14:11 2020 +0200

    Completed Chaptern 1
Mac-mini-de-Rodolphe:Story rodolphedupuy$ touch chapter2.text
Mac-mini-de-Rodolphe:Story rodolphedupuy$ touch chapter3.text
Mac-mini-de-Rodolphe:Story rodolphedupuy$ open chapter2.txt
Mac-mini-de-Rodolphe:Story rodolphedupuy$ open chapter3.txt
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	chapter2.txt
	chapter3.txt

nothing added to commit but untracked files present (use "git add" to track)
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git add .
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   chapter2.txt
	new file:   chapter3.txt

Mac-mini-de-Rodolphe:Story rodolphedupuy$ git commit -m "complete Chapter 2 & 3"
[master 55d6bfa] complete Chapter 2 & 3
 2 files changed, 2 insertions(+)
 create mode 100644 chapter2.txt
 create mode 100644 chapter3.txt
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git log
commit 55d6bfa8b45930d1dede0430a05f35cc1a69c3a5 (HEAD -> master)
Author: Rodolphe DUPUY <rodolphe.dupuy@free.fr>
Date:   Fri May 8 11:18:20 2020 +0200

    complete Chapter 2 & 3

commit 0b85f395f797c331fb004342908f6ec4a7593347
Author: Rodolphe DUPUY <rodolphe.dupuy@free.fr>
Date:   Fri May 8 11:14:11 2020 +0200

    Completed Chaptern 1
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   chapter3.txt

no changes added to commit (use "git add" and/or "git commit -a")
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git diff Chapter3.txt
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git diff chapter3.txt
diff --git a/chapter3.txt b/chapter3.txt
index 8f6e057..d22c05c 100644
--- a/chapter3.txt
+++ b/chapter3.txt
@@ -1 +1 @@
-Troisième fichier Chapter
\ No newline at end of file
+sjhqdb;jhsbdjshb
\ No newline at end of file
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git checkout chapter3.txt
Updated 1 path from the index
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git log
commit 55d6bfa8b45930d1dede0430a05f35cc1a69c3a5 (HEAD -> master)
Author: Rodolphe DUPUY <rodolphe.dupuy@free.fr>
Date:   Fri May 8 11:18:20 2020 +0200

    complete Chapter 2 & 3

commit 0b85f395f797c331fb004342908f6ec4a7593347
Author: Rodolphe DUPUY <rodolphe.dupuy@free.fr>
Date:   Fri May 8 11:14:11 2020 +0200

    Completed Chaptern 1
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git remote add origin https://github.com/Somplesi/Story.git
Mac-mini-de-Rodolphe:Story rodolphedupuy$ git push -u origin master
Username for 'https://github.com': somplesi
Password for 'https://somplesi@github.com': 
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (7/7), 592 bytes | 592.00 KiB/s, done.
Total 7 (delta 0), reused 0 (delta 0)
To https://github.com/Somplesi/Story.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
Mac-mini-de-Rodolphe:Story rodolphedupuy$ 

