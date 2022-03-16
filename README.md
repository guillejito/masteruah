guill@DESKTOP-46J0L3Q MINGW64 ~ (master)
$ cd desktop																					// Ubicacion de la copia en local

guill@DESKTOP-46J0L3Q MINGW64 ~/desktop (master)
$ git clone https://github.com/guillejito/masteruah.git		   // Comando para clonar
Cloning into 'masteruah'...
warning: You appear to have cloned an empty repository.



![image-20220309194520418](C:\Users\guill\AppData\Roaming\Typora\typora-user-images\image-20220309194520418.png)



guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (main)
$ git commit -m "commit inicial"
[main (root-commit) fb0b60d] commit inicial											// Añadir mensaje
 1 file changed, 11 insertions(+)
 create mode 100644 README.md



guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (main)
$ git push https://github.com/guillejito/masteruah.git
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.															// Subir a github
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 494 bytes | 494.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/guillejito/masteruah.git
 * [new branch]      main -> main



guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (main)
$ git tag v0.1																										//Creado tag
fatal: tag 'v0.1' already exists



guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (main)
$ git branch v0.2

guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (main)					//Creada rama
$ git checkout v0.2
Switched to branch 'v0.2'
M       README.md



guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (v0.2)
$ git push --tag origin v0.1
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.															//Subbir tag
Writing objects: 100% (1/1), 160 bytes | 160.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/guillejito/masteruah.git

 * [new tag]         v0.1 -> v0.1



guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (v0.2)
$ touch 2.txt

guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (v0.2)					//Añadir un fichero 2.txt en la rama v0.2.
$ git add .

guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (v0.2)
$ git commit -m "añadido 2.txt"
[v0.2 bafc61b] añadido 2.txt
 3 files changed, 49 insertions(+), 1 deletion(-)
 create mode 100644 1.txt
 create mode 100644 2.txt



guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (v0.2)
$ git push origin v0.2
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads															//Crear rama remota v0.2
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 999 bytes | 999.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'v0.2' on GitHub by visiting:
remote:      https://github.com/guillejito/masteruah/pull/new/v0.2
remote:
To https://github.com/guillejito/masteruah.git

 * [new branch]      v0.2 -> v0.2



guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (v0.2)
$ git branch master

guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (v0.2)						//Merge directo
$ git checkout master
Switched to branch 'master'
M       README.md

guill@DESKTOP-46J0L3Q MINGW64 ~/desktop/masteruah (master)
$ git merge v0.2 -m "merge v0.2 directo"
Already up to date.
