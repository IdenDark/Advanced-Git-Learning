# Advanced-Git-Learning

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
