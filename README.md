# beacademy-devstart-gitegithub
Git e GitHub

# conhecendo o git e o gitHub.


# Como saber a versão do git
Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub <br>
	$ git version
git version 2.39.0.windows.2


# Configurando o git com o nome e com e-mail
Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub <br>
	$ git config --global user.name "geiza-moreira"

Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub <br>
	$ Git config --global user.email "geizaphm2021@gmail.com"




# Clone do repositório do github

Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub <br>
	$ git clone git@github.com:geiza-moreira/beacademy-devstart-gitegithub.git
Cloning into 'beacademy-devstart-gitegithub'...
Enter passphrase for key '/c/Users/Adair & Geisa/.ssh/id_ed25519':
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.


# Para acessar o diretório 

	$ cd beacademy-devstart-gitegithub

Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub/beacademy-devstart-gitegithub (main)
	$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean


# Visualizar o repositório remoto
Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub/beacademy-devstart-gitegithub (main) <br>
	$ git remote -v
origin  git@github.com:geiza-moreira/beacademy-devstart-gitegithub.git (fetch)
origin  git@github.com:geiza-moreira/beacademy-devstart-gitegithub.git (push)

# Fazendo alteração no readme
Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub/beacademy-devstart-gitegithub (main) <br>
	$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md


# Preparando a alteração para ser commitada
Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub/beacademy-devstart-gitegithub (main) <br>
	$ git add .

Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub/beacademy-devstart-gitegithub (main) <br>
	$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


# Fazendo o Commit
Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub/beacademy-devstart-gitegithub (main) <br>
	$ git commit -m "Ajustes no readme"
[main e6052b5] Ajustes no readme
 1 file changed, 2 insertions(+)


# Enviando alterações para o repositório remote
Geisa@Adair-PC MINGW32 ~/Desktop/beacademy-devstart-gitegithub/beacademy-devstart-gitegithub (main) <br>
	$ git push
Enter passphrase for key '/c/Users/Adair & Geisa/.ssh/id_ed25519':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 314 bytes | 314.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:geiza-moreira/beacademy-devstart-gitegithub.git
   ce6c414..e6052b5  main -> main
