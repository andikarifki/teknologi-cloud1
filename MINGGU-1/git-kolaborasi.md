User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1 (master)
$ git clone https://github.com/andikarifki/farizasandaira98.github.io
Cloning into 'farizasandaira98.github.io'...
remote: Enumerating objects: 61, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 61 (delta 0), reused 3 (delta 0), pack-reused 58R
Receiving objects: 100% (61/61), 4.47 MiB | 3.55 MiB/s, done.
Resolving deltas: 100% (2/2), done.

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1 (master)
$ git remote -v

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1 (master)
$ ls -la
total 17
drwxr-xr-x 1 User 197121    0 Feb 16 08:22 ./
drwxr-xr-x 1 User 197121    0 Feb 16 07:01 ../
drwxr-xr-x 1 User 197121    0 Feb 16 08:05 .git/
drwxr-xr-x 1 User 197121    0 Feb 16 08:06 Pictures/
-rw-r--r-- 1 User 197121  149 Feb 16 08:12 README.md
drwxr-xr-x 1 User 197121    0 Feb 16 08:23 farizasandaira98.github.io/
-rw-r--r-- 1 User 197121 1747 Feb 16 08:10 rangkuman-cloud-computing.md

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1 (master)
$ git remote -v

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1 (master)
$ cd farizasandaira98.github.io

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1/farizasandaira98.github.io (master)
$ ls -la
total 33
drwxr-xr-x 1 User 197121    0 Feb 16 08:23 ./
drwxr-xr-x 1 User 197121    0 Feb 16 08:22 ../
drwxr-xr-x 1 User 197121    0 Feb 16 08:23 .git/
-rw-r--r-- 1 User 197121    9 Feb 16 08:23 README.md
-rw-r--r-- 1 User 197121    0 Feb 16 08:23 about.html
drwxr-xr-x 1 User 197121    0 Feb 16 08:23 images/
-rw-r--r-- 1 User 197121 5341 Feb 16 08:23 index.html
-rw-r--r-- 1 User 197121 4260 Feb 16 08:23 modernizr-custom.js
drwxr-xr-x 1 User 197121    0 Feb 16 08:23 style/
drwxr-xr-x 1 User 197121    0 Feb 16 08:23 test/

[1]+  Stopped                 vim README.MD

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1/farizasandaira98.github.io (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .README.md.swp

nothing added to commit but untracked files present (use "git add" to track)

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1/farizasandaira98.github.io (master)
$ git add -A

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1/farizasandaira98.github.io (master)
$ git commit -m "Add: Contributor"
[master c4e6520] Add: Contributor
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 .README.md.swp

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1/farizasandaira98.github.io (master)
$ git push origin add-contributor
error: src refspec add-contributor does not match any
error: failed to push some refs to 'https://github.com/andikarifki/farizasandair
a98.github.io'

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1/farizasandaira98.github.io (master)
$ git push origin add-contributor
error: src refspec add-contributor does not match any
error: failed to push some refs to 'https://github.com/andikarifki/farizasandair
a98.github.io'

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1/farizasandaira98.github.io (master)
$ git checkout master
Already on 'master'
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1/farizasandaira98.github.io (master)
$ git push origin add-contributor
error: src refspec add-contributor does not match any
error: failed to push some refs to 'https://github.com/andikarifki/farizasandair
a98.github.io'

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1/farizasandaira98.github.io (master)
$ git push github master
fatal: 'github' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

User@WINDOWS-1K4PNGP MINGW64 /e/My file/KULIAH BOSS/TCLOUD/MINGGU-1/farizasandaira98.github.io (master)
$ git pull origin master
From https://github.com/andikarifki/farizasandaira98.github.io
 * branch            master     -> FETCH_HEAD
Already up to date.
