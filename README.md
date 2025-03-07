# Advanced-Git-Learning

# Exercise 1

```bash
Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git
$ echo "# Advanced-Git-Learning" >> README.md


Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git
$ git init
Initialized empty Git repository in C:/Users/Shepherd/Documents/GYM/Advanced Git
/.git/

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (master)
$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the nex
t time Git touches it

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (master)
$ git commit -m "First commission"
[master (root-commit) ab7789b] First commission
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (master)
$ git branch  -m  main

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git remote add origin git@github.com:IdenDark/Advanced-Git-Learning.git
Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 247 bytes | 41.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:IdenDark/Advanced-Git-Learning.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ touch test {1..4}.md

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git add test1.md && git commit -m "chore: Creating initial file "
fatal: pathspec 'test1.md' did not match any files

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ ls
1.md  2.md  3.md  4.md  README.md  test

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ rm test {1..4}.md

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ ls
README.md

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ touch test{1..4}.md

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ ls
README.md  test1.md  test2.md  test3.md  test4.md

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git add test1.md && git commit -m "chore: Creating initial file "
[main b9e91fb] chore: Creating initial file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git add test2.md && git commit -m "chore: Creating another file "
[main 13994b7] chore: Creating another file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md


Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git add test3.md && git commit -m "chore: Creating third and forth file "
[main cadd810] chore: Creating third and forth file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
```

## Exercise 2

```bash
$ git log
commit 34d8419a047970bb876c9b1c72c0ebd5cffaf5c5 (HEAD -> main, origin/main)
Author: IdenDark <bonheurndacyayisenga@gmail.com>
Date:   Fri Feb 28 12:14:36 2025 +0200

     First commision
```

```bash
commit e3f5bd29b13f879a045a4db745e983894f592081
commit 34d8419a047970bb876c9b1c72c0ebd5cffaf5c5 (HEAD -> main, origin/main)
Author: IdenDark <bonheurndacyayisenga@gmail.com>
Date:   Fri Feb 28 12:14:36 2025 +0200

     First commision

commit e3f5bd29b13f879a045a4db745e983894f592081
commit 34d8419a047970bb876c9b1c72c0ebd5cffaf5c5 (HEAD -> main, origin/main)
Author: IdenDark <bonheurndacyayisenga@gmail.com>
Date:   Fri Feb 28 12:14:36 2025 +0200

     First commision

commit e3f5bd29b13f879a045a4db745e983894f592081
Author: IdenDark <bonheurndacyayisenga@gmail.com>
Date:   Fri Feb 28 12:09:16 2025 +0200

     First commision

commit cadd8100aa306e7ce33451d1fe7ba6542caef1fc
Author: IdenDark <bonheurndacyayisenga@gmail.com>
Date:   Fri Feb 28 12:04:52 2025 +0200

    chore: Creating third and forth file

commit 13994b756bacf77ef0add6c43b5d149fdbc762ca
Author: IdenDark <bonheurndacyayisenga@gmail.com>
Date:   Fri Feb 28 12:04:08 2025 +0200

    chore: Creating another file

commit b9e91fb54f206b967d6279c164b87a5d6845ca74
Author: IdenDark <bonheurndacyayisenga@gmail.com>
Date:   Fri Feb 28 12:03:53 2025 +0200
```

```bash

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git log --online --graph --all
fatal: unrecognized argument: --online

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git log --oneline --graph --all

- 34d8419 (HEAD -> main, origin/main) First commision
- e3f5bd2 First commision
- cadd810 chore: Creating third and forth file
- 13994b7 chore: Creating another file
- b9e91fb chore: Creating initial file
- ab7789b First commission
```

```bash

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
 modified: README.md

no changes added to commit (use "git add" and/or "git commit -a")

Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ ls
README.md test1.md test2.md test3.md test4.md

```

```bash
Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git add test4.md
```

```bash
Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git commit --amend -m "chore: Create the forth file"
[main a9e799a] chore: Create the forth file
Date: Fri Feb 28 12:14:36 2025 +0200
1 file changed, 4 insertions(+)
```

```bash
Shepherd@Syndicate MINGW64 ~/Documents/GYM/Advanced Git (main)
$ git log --oneline
a9e799a (HEAD -> main) chore: Create the forth file
e3f5bd2 First commision
cadd810 chore: Creating third and forth file
13994b7 chore: Creating another file
b9e91fb chore: Creating initial file
ab7789b First commission

```

### Exercise 3

```bash
$ git reflog

251b3d7 (HEAD -> main, origin/main) HEAD@{0}: rebase (finish): returning to refs
/heads/main
251b3d7 (HEAD -> main, origin/main) HEAD@{1}: rebase (pick): Exercise 2 Amending
efa8cc3 HEAD@{2}: rebase (pick): chore: Create the forth file
0cd49e4 HEAD@{3}: rebase (pick): First commision
43d9373 HEAD@{4}: rebase (pick): chore: Creating third and forth file
4d31f5f HEAD@{5}: rebase (reword): chore: Creating a second file
13994b7 HEAD@{6}: rebase: fast-forward
b9e91fb HEAD@{7}: rebase (start): checkout HEAD~6
1cfb6db HEAD@{8}: rebase (finish): returning to refs/heads/main

```

```bash
$ git rebase -i HEAD~6

pick b9e91fb chore: Creating initial file
reword 13994b7 chore: Creating another file
pick cadd810 chore: Creating third and forth file
pick e3f5bd2 First commission
pick 34d8419 First commision
pick a9e799a Exercise 2 Amending

Successfully rebased and updated refs/heads/main.

```

```bash
$ git push origin main --force

```

#### Exercise 4

$ git reflog

```bash
...
1cfb6db HEAD@{25}: reset: moving to HEAD
1cfb6db HEAD@{26}: commit: Exercise 2 Amending
a9e799a HEAD@{27}: commit (amend): chore: Create the forth file
34d8419 HEAD@{28}: commit: First commision
e3f5bd2 HEAD@{29}: commit: First commision
cadd810 HEAD@{30}: commit: chore: Creating third and forth file
13994b7 HEAD@{31}: commit: chore: Creating another file
b9e91fb HEAD@{32}: commit: chore: Creating initial file
ab7789b HEAD@{33}: Branch: renamed refs/heads/master to refs/heads/main
ab7789b HEAD@{35}: commit (initial): First commission
```
