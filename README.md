# 11-17-2026

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069
$ mkdir exp6

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069
$ cd exp5

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp5 (main)
$ git init
Reinitialized existing Git repository in C:/Users/CMRIT-ISE-L208-002/Documents/1CR25IS069/exp5/.git/

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp5 (main)
$ vi main.c

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp5 (main)
$ cd ..

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069
$ exp6
bash: exp6: command not found

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069
$  cd exp6

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6
$ git init
Initialized empty Git repository in C:/Users/CMRIT-ISE-L208-002/Documents/1CR25IS069/exp6/.git/

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ vi main.c

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ cat main.c
#include<stdio.h>
int main()
{
printf("hello worldi");
}

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ git add .
warning: in the working copy of 'main.c', LF will be replaced by CRLF the next time Git touches it

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   main.c


CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ git commit -m"fkere"
[master (root-commit) d6114d2] fkere
 1 file changed, 5 insertions(+)
 create mode 100644 main.c

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ git checkout-b feature_bramch
git: 'checkout-b' is not a git command. See 'git --help'.

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ git checkout -b feature_bramch
Switched to a new branch 'feature_bramch'

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (feature_bramch)
$ vi main.c

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (feature_bramch)
$ cat main.c
#include<stdio.h>
int main()
{
printf("hello worldi");
printf("cmr");
}

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (feature_bramch)
$ git add .
warning: in the working copy of 'main.c', LF will be replaced by CRLF the next time Git touches it

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (feature_bramch)
$ git status
On branch feature_bramch
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   main.c


CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (feature_bramch)
$ git commit -m "just commiting"
[feature_bramch 336f61e] just commiting
 1 file changed, 1 insertion(+)

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (feature_bramch)
$ git checkout master
Switched to branch 'master'

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ git merge --no-ff feature_branch -m" "
merge: feature_branch - not something we can merge

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ ^[[200~git merge --no-ff feature_branch -m" "
bash: $'\E[200~git': command not found

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ git merge --no-ff feature_branch -m"efiofje"
merge: feature_branch - not something we can merge

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ git merge --no-ff feature_bramch -m"efiofje"
Merge made by the 'ort' strategy.
 main.c | 1 +
 1 file changed, 1 insertion(+)

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ cat main.c
#include<stdio.h>
int main()
{
printf("hello worldi");
printf("cmr");
}

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ git log --oneline --graph --all
*   74861a3 (HEAD -> master) efiofje
|\
| * 336f61e (feature_bramch) just commiting
|/
* d6114d2 fkere

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp6 (master)
$ cd ..

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069
$ mkdir exp7

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069
$ cd exp7

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp7
$ git init
Initialized empty Git repository in C:/Users/CMRIT-ISE-L208-002/Documents/1CR25IS069/exp7/.git/

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp7 (master)
$ vi main.c

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp7 (master)
$ cat main.c
#include<stdio.h>
int main()
{
printf("whedjed");
return 0;
}

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp7 (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        main.c

nothing added to commit but untracked files present (use "git add" to track)

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp7 (master)
$ git add .
warning: in the working copy of 'main.c', LF will be replaced by CRLF the next time Git touches it

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp7 (master)
$ git commit -m"main branch"
[master (root-commit) 56015b6] main branch
 1 file changed, 6 insertions(+)
 create mode 100644 main.c

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp7 (master)
$ git tag v1.0

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp7 (master)
$ git tag
v1.0

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp7 (master)
$ git show v1.0
commit 56015b6d5b3d53e527d4fc95fc45da8070524c96 (HEAD -> master, tag: v1.0)
Author: prerana <prajwaldanappanavar@gamil.com>
Date:   Tue Nov 17 11:23:27 2026 +0530

    main branch

diff --git a/main.c b/main.c
new file mode 100644
index 0000000..acb23d6
--- /dev/null
+++ b/main.c
@@ -0,0 +1,6 @@
+#include<stdio.h>
+int main()
+{
+printf("whedjed");
+return 0;
+}

CMRIT-ISE-L208-002@ISE-L208-DT002 MINGW64 ~/Documents/1CR25IS069/exp7 (master)
$
