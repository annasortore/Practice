# Practice

Anna@AESPC1 MINGW64 /
$ echo "# Practice" >> README.md

Anna@AESPC1 MINGW64 /
$ git init
Initialized empty Git repository in C:/Users/Anna/AppData/Local/Programs/Git/.git/

Anna@AESPC1 MINGW64 / (master)
$ git add README.md
warning: LF will be replaced by CRLF in README.md.
The file will have its original line endings in your working directory

Anna@AESPC1 MINGW64 / (master)
$ git commit -m "first commit"
[master (root-commit) 56a7081] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

Anna@AESPC1 MINGW64 / (master)
$ git remote add origin https://github.com/annasortore/Practice.git             
Anna@AESPC1 MINGW64 / (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 220 bytes | 110.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/annasortore/Practice.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

Anna@AESPC1 MINGW64 / (master)
$ mkdir cool

Anna@AESPC1 MINGW64 / (master)
$ cd cool

Anna@AESPC1 MINGW64 /cool (master)
$ git init
Initialized empty Git repository in C:/Users/Anna/AppData/Local/Programs/Git/cool/.git/

Anna@AESPC1 MINGW64 /cool (master)
$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

Anna@AESPC1 MINGW64 /cool (master)
$ git config user.name "ANNA"

Anna@AESPC1 MINGW64 /cool (master)
$ git config user.email "annasortore6@gmail.com?
> git config user.email "annasortore6@gmail.com

Anna@AESPC1 MINGW64 /cool (master)
$ notepad os.c

Anna@AESPC1 MINGW64 /cool (master)
$ git add os.c

Anna@AESPC1 MINGW64 /cool (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   os.c


Anna@AESPC1 MINGW64 /cool (master)
$ git commit -a -m "Initial checkin"
[master (root-commit) 7fcee2c] Initial checkin
 1 file changed, 6 insertions(+)
 create mode 100644 os.c

Anna@AESPC1 MINGW64 /cool (master)
$ git status
On branch master
nothing to commit, working tree clean

Anna@AESPC1 MINGW64 /cool (master)
$ git log
commit 7fcee2ccf2c509610c273d51666d9a243714996a (HEAD -> master)
Author: ANNA <annasortore6@gmail.com?git config user.email annasortore6@gmail.com>
Date:   Sat Jan 25 23:30:01 2020 -0500

    Initial checkin

Anna@AESPC1 MINGW64 /cool (master)
$ notepad os.c

Anna@AESPC1 MINGW64 /cool (master)
$ git commit -a
hint: Waiting for your editor to close the file...
[main 2020-01-26T04:31:55.031Z] update#setState idle
Aborting commit due to empty commit message.

Anna@AESPC1 MINGW64 /cool (master)
$ git diff
diff --git a/os.c b/os.c
index 864340b..96c741a 100644
--- a/os.c
+++ b/os.c
@@ -3,4 +3,5 @@ Main()
   printf("I like being outside\n");
   printf("When I'm inside too long\n");
   printf("I get sad\n");
+  printf("So winter is hard\n");
 }
\ No newline at end of file

Anna@AESPC1 MINGW64 /cool (master)
$ git diff os.c
diff --git a/os.c b/os.c
index 864340b..96c741a 100644
--- a/os.c
+++ b/os.c
@@ -3,4 +3,5 @@ Main()
   printf("I like being outside\n");
   printf("When I'm inside too long\n");
   printf("I get sad\n");
+  printf("So winter is hard\n");
 }
\ No newline at end of file
