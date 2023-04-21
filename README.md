# assignment-3
admin@ADMIN MINGW64 ~
$ cd documents

admin@ADMIN MINGW64 ~/documents (master)
$ cd ttt

admin@ADMIN MINGW64 ~/documents/ttt (master)
$ touch file1.txt file2.txt

admin@ADMIN MINGW64 ~/documents/ttt (master)
$ git add file1.txt file2.txt

admin@ADMIN MINGW64 ~/documents/ttt (master)
$ git reset file1.txt file2.txt
Unstaged changes after reset:
D       10.docx
D       41_a_vishwa darji cloud.rtf
D       Emotional intelligence.pptx
D       Gujarat University.pptx
D       Microsoft.txt.docx
D       Oracle.txt.docx
D       cross reference .txt.docx
M       vishu stuff/My documents/New folder/chess/abraction task 2.exe
M       vishu stuff/My documents/New folder/chess/abstraction task 1.cpp
M       vishu stuff/My documents/New folder/chess/addition const.cpp
M       vishu stuff/My documents/New folder/chess/addition const.exe
M       vishu stuff/My documents/New folder/chess/login page.exe
D       yyy

admin@ADMIN MINGW64 ~/documents/ttt (master)
$ git add file1.txt

admin@ADMIN MINGW64 ~/documents/ttt (master)
$ git commit -m "Added file1.txt"
[master a1a2cbd] Added file1.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 ttt/file1.txt

admin@ADMIN MINGW64 ~/documents/ttt (master)
$ git add file2.txt

admin@ADMIN MINGW64 ~/documents/ttt (master)
$ git commit -m "Added file2.txt"
[master 1f7f1f2] Added file2.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 ttt/file2.txt

admin@ADMIN MINGW64 ~/documents/ttt (master)
$ git commit --amend -m "Added new file file2.txt"
[master 1417fb0] Added new file file2.txt
 Date: Fri Apr 21 11:11:41 2023 +0530
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 ttt/file2.txt

admin@ADMIN MINGW64 ~/documents/ttt (master)
$ git branch development

admin@ADMIN MINGW64 ~/documents/ttt (master)
$ git checkout development
Switched to branch 'development'
D       10.docx
D       41_a_vishwa darji cloud.rtf
D       Emotional intelligence.pptx
D       Gujarat University.pptx
D       Microsoft.txt.docx
D       Oracle.txt.docx
D       cross reference .txt.docx
M       vishu stuff/My documents/New folder/chess/abraction task 2.exe
M       vishu stuff/My documents/New folder/chess/abstraction task 1.cpp
M       vishu stuff/My documents/New folder/chess/addition const.cpp
M       vishu stuff/My documents/New folder/chess/addition const.exe
M       vishu stuff/My documents/New folder/chess/login page.exe
D       yyy

admin@ADMIN MINGW64 ~/documents/ttt (development)
$ touch file3.txt

admin@ADMIN MINGW64 ~/documents/ttt (development)
$ git add file3.txt

admin@ADMIN MINGW64 ~/documents/ttt (development)
$ git stash
Saved working directory and index state WIP on development: 1417fb0 Added new file file2.txt

admin@ADMIN MINGW64 ~/documents/ttt (development)
$ git stash pop
warning: could not open directory 'My Music/': Permission denied
warning: could not open directory 'My Pictures/': Permission denied
warning: could not open directory 'My Videos/': Permission denied
On branch development
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file3.txt

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    ../10.docx
        deleted:    ../41_a_vishwa darji cloud.rtf
        deleted:    ../Emotional intelligence.pptx
        deleted:    ../Gujarat University.pptx
        deleted:    ../Microsoft.txt.docx
        deleted:    ../Oracle.txt.docx
        deleted:    ../cross reference .txt.docx
        modified:   ../vishu stuff/My documents/New folder/chess/abraction task 2.exe
        modified:   ../vishu stuff/My documents/New folder/chess/abstraction task 1.cpp
        modified:   ../vishu stuff/My documents/New folder/chess/addition const.cpp
        modified:   ../vishu stuff/My documents/New folder/chess/addition const.exe
        modified:   ../vishu stuff/My documents/New folder/chess/login page.exe
        deleted:    ../yyy

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ../MySQL/prcts 1.sql
        ../MySQL/prcts 2.sql
        ../MySQL/prcts.sql
        ../Save Energy.pptx
        ../cpp all tsks.docx
        ../file2.txt
        ../linux.txt
        ../total.cpp
        ../vvv.txt

Dropped refs/stash@{0} (0a08d8952fac7b5c6cde43d47894697f4cd8102b)

admin@ADMIN MINGW64 ~/documents/ttt (development)
$
