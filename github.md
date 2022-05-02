Lucas@DESKTOP-FKNE1T1 MINGW64 ~
$ git config --global user.name "Lucas Luciano Pires"

Lucas@DESKTOP-FKNE1T1 MINGW64 ~
$ git config --global user.email "lucas.fbueno@aluno.faculdadeimpacta.com.br"

Lucas@DESKTOP-FKNE1T1 MINGW64 ~
$ git config user.name
Lucas Luciano Pires

Lucas@DESKTOP-FKNE1T1 MINGW64 ~
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager-core
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.name=Lucas Luciano Pires
user.email=lucas.fbueno@aluno.faculdadeimpacta.com.br

Lucas@DESKTOP-FKNE1T1 MINGW64 ~
$ mkdir git-course

Lucas@DESKTOP-FKNE1T1 MINGW64 ~
$ dir git-course/

Lucas@DESKTOP-FKNE1T1 MINGW64 ~
$ cd git-course/

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course
$ git init
Initialized empty Git repository in C:/Users/Lucas/git-course/.git/

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ ls-la
bash: ls-la: command not found

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ ls -la
total 16
drwxr-xr-x 1 Lucas 197121 0 Dec  6 21:47 ./
drwxr-xr-x 1 Lucas 197121 0 Dec  6 21:45 ../
drwxr-xr-x 1 Lucas 197121 0 Dec  6 21:47 .git/

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ cd .git/

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course/.git (GIT_DIR!)
$ ls
HEAD  config  description  hooks/  info/  objects/  refs/

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course/.git (GIT_DIR!)
$ cd ..

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ vi Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ ls
Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ vi Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Readme.md

nothing added to commit but untracked files present (use "git add" to track)

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ vi Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Readme.md

nothing added to commit but untracked files present (use "git add" to track)

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git add Readme.md
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git add Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Readme.md


Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ vim Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Readme.md

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Readme.md


Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git add Readme.md
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git add Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Readme.md


Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git commit -m "Add Readme.md"
[master (root-commit) ae28046] Add Readme.md
 1 file changed, 6 insertions(+)
 create mode 100644 Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git log
commit ae280460a2406e187044ba4355c33e93ab73dc51 (HEAD -> master)
Author: Lucas Luciano Pires <lucas.fbueno@aluno.faculdadeimpacta.com.br>
Date:   Mon Dec 6 22:41:43 2021 -0300

    Add Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git log --author="Lucas"
commit ae280460a2406e187044ba4355c33e93ab73dc51 (HEAD -> master)
Author: Lucas Luciano Pires <lucas.fbueno@aluno.faculdadeimpacta.com.br>
Date:   Mon Dec 6 22:41:43 2021 -0300

    Add Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git shortlog
Lucas Luciano Pires (1):
      Add Readme.md


Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ vim Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git diff
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory
diff --git a/Readme.md b/Readme.md
index 0d478e7..3b77c23 100644
--- a/Readme.md
+++ b/Readme.md
@@ -4,3 +4,5 @@

 Arquivo da aula de Git e Github para iniciantes.
 Este é um repositorio teste para ensinar como o Git funciona.
+
+Gostou do curso? Quer mais? Ajude com uma doação, até um café é válido =)

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git diff --name-only
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory
Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ g s
bash: g: command not found

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git commit -am "Edit Readme"
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory
[master 6ec9eb5] Edit Readme
 1 file changed, 2 insertions(+)

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git log
commit 6ec9eb57b1dad061acc9d0e903e53476b4c33b93 (HEAD -> master)
Author: Lucas Luciano Pires <lucas.fbueno@aluno.faculdadeimpacta.com.br>
Date:   Tue Dec 7 09:59:27 2021 -0300

    Edit Readme

commit ae280460a2406e187044ba4355c33e93ab73dc51
Author: Lucas Luciano Pires <lucas.fbueno@aluno.faculdadeimpacta.com.br>
Date:   Mon Dec 6 22:41:43 2021 -0300

    Add Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git log
commit 6ec9eb57b1dad061acc9d0e903e53476b4c33b93 (HEAD -> master)
Author: Lucas Luciano Pires <lucas.fbueno@aluno.faculdadeimpacta.com.br>
Date:   Tue Dec 7 09:59:27 2021 -0300

    Edit Readme

commit ae280460a2406e187044ba4355c33e93ab73dc51
Author: Lucas Luciano Pires <lucas.fbueno@aluno.faculdadeimpacta.com.br>
Date:   Mon Dec 6 22:41:43 2021 -0300

    Add Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ vim Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Readme.md

no changes added to commit (use "git add" and/or "git commit -a")

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git diff
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory
diff --git a/Readme.md b/Readme.md
index 3b77c23..39d4dce 100644
--- a/Readme.md
+++ b/Readme.md
@@ -6,3 +6,4 @@ Arquivo da aula de Git e Github para iniciantes.
 Este é um repositorio teste para ensinar como o Git funciona.

 Gostou do curso? Quer mais? Ajude com uma doação, até um café é válido =)
+kkkk

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git checkout Readme.md
Updated 1 path from the index

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git diff

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ vim Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git add Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   Readme.md


Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git diff

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git reset HEAD Readme.md
Unstaged changes after reset:
M       Readme.md

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git diff
diff --git a/Readme.md b/Readme.md
index 3b77c23..c503507 100644
--- a/Readme.md
+++ b/Readme.md
@@ -6,3 +6,5 @@ Arquivo da aula de Git e Github para iniciantes.
 Este é um repositorio teste para ensinar como o Git funciona.

 Gostou do curso? Quer mais? Ajude com uma doação, até um café é válido =)
+
+uhsaduhasudasuhd

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git checkout Readme.md
Updated 1 path from the index

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git status
On branch master
nothing to commit, working tree clean

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ ssh-keygen -t ed25519 -C "lucas.fbueno@aluno.faculdadeimpacta.com.br"
bash: $'\302\226ssh-keygen': command not found

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ ssh-keygen -t rsa -b 4096 -C "lucas.fbueno@aluno.faculdadeimpacta.com.br"
bash: $'\302\226ssh-keygen': command not found

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ ssh-keygen -t rsa -b 4096 -C "lucas.fbueno@aluno.faculdadeimpacta.com.br"
bash: $'\302\226ssh-keygen': command not found

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ $ ssh-keygen -t rsa -b 4096 -C "lucas.fbueno@aluno.faculdadeimpacta.com.br"
bash: $'$\302\226ssh-keygen': command not found

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ ssh-keygen -t ed25519 - C "lucas.fbueno@aluno.faculdadeimpacta.com.br"
bash: $'\302\226ssh-keygen': command not found

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ ssh-keygen -t rsa -b 4096 -C "lucas.fbueno@aluno.faculdade.com.br"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/Lucas/.ssh/id_rsa):
Created directory '/c/Users/Lucas/.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/Lucas/.ssh/id_rsa
Your public key has been saved in /c/Users/Lucas/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:S8Y2T0ZjuyGv17kPEu2cvz+TTaIoCD2IdnHKgwEP1Qw lucas.fbueno@aluno.faculdade.com.br
The key's randomart image is:
+---[RSA 4096]----+
| .E+             |
|o   o            |
| +        +      |
|  o . .. o +     |
|   = *  S * .    |
|  + B o+ O * .. .|
| . . o o. =o=o oo|
|      . ..o.+o +.|
|        .o  .o+o+|
+----[SHA256]-----+

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ cd ~/.ssh/

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/.ssh
$ ls
id_rsa  id_rsa.pub

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/.ssh
$ cat id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQC6ZhgUb3A/K9w1c4fndp5FM0TlFCWs07hSILhSSB0pmn7j0kJ5N92rbOGqf0EOAX5lKp64Edi5bgBjfpJdWe/5IKFtuPa9pGK7+T2aVMzvdSRNOIfRLIwkGUMl85PFgmucsiol4lV8LiGE7q5dWCdryVNyNfSs8Y/dLqWvSMmruj7yIJsi1wHu/A62KIwh/W+ELoFjBsCgmD+5eEaLgglPjS24CDnjqxjweuJUj7Mno3Y2Mzjo98dls+C6IAwdN2Pw0Vo9epaJUp5ebpcmxvyQRj2+w+jQczi86y3AeXgTuFlmIGyvRW3klXC7NTrdLkSxyixbMnF/xyw7a+13jjlXGwZa2olV/OIlsVbA3RXg2z0WXBvzkYwmlCtmG4py7hp6bg+XK6LZlJT18+1QnbEsme9y/ZCyctP5rrcn3fjMS5JWY8UVD6jMNKVJlZFp0DSfXnUjg97DF4M2HZjPsr817pl1rSdnOQMrJlxGLW36QYpQG1icYjAzKoS3g8XMOHnB7rRDYMGVwOezwKRl0HmJxVvA/f4C1t4RlCmJLH2T58oqa/bFeAPZyUqdmzZOReUFmwYY8mrgvYcrySKBvCVEMiPMB/UaXafIujPRzo7WV4M5u0WuqGpyJmGauVDUi4Ly3bKtRksiarDFrlacQt3Zd9TIcsq5Sef/3Pi8SVo0QQ== lucas.fbueno@aluno.faculdade.com.br

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/.ssh
$ git remote add origin https://github.com/LucasLucianoP/github-course.git
fatal: not a git repository (or any of the parent directories): .git

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/.ssh
$ cd ~/git-course/

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git remote add origin https://github.com/LucasLucianoP/github-course.git

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git remote
origin

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git remote -v
origin  https://github.com/LucasLucianoP/github-course.git (fetch)
origin  https://github.com/LucasLucianoP/github-course.git (push)

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/LucasLucianoP/github-course.git'

Lucas@DESKTOP-FKNE1T1 MINGW64 ~/git-course (master)
$ git push -u origin master
fatal: helper error (-1): User cancelled dialog.

git push -u origin main
git remote
git diff
git push -u origin main
$ cd ~/git-course/

