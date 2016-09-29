Windows PowerShell
Copyright (C) 2015 Microsoft Corporation. Todos los derechos reservados.

C:\Users\carlillos tole\Documents\GitHub> ssh-keygen -t rsa -C "carliyostole@gmail.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/carlillos tole/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Saving key "/c/Users/carlillos tole/.ssh/id_rsa" failed: passphrase is too short (minimum five characters)
C:\Users\carlillos tole\Documents\GitHub> ssh-keygen -t rsa -C "carliyostole@gmail.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/carlillos tole/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/carlillos tole/.ssh/id_rsa.
Your public key has been saved in /c/Users/carlillos tole/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:4sH0O+vkdHqmLUxXAusOdh+ObMra8pL+UJexlVI/FDU carliyostole@gmail.com
The key's randomart image is:
+---[RSA 2048]----+
|          . ooE  |
|        .. +   . |
|      . ooo o    |
|     o ..*. ..   |
|      =.S  o     |
|     oo++.o      |
|    .o.B==..     |
|    ++ +B*=      |
|   .o**+*=.      |
+----[SHA256]-----+
C:\Users\carlillos tole\Documents\GitHub> sudo apt-get install xclip
sudo : El término 'sudo' no se reconoce como nombre de un cmdlet, función, archivo de script o programa ejecutable.
Compruebe si escribió correctamente el nombre o, si incluyó una ruta de acceso, compruebe que dicha ruta es correcta e
inténtelo de nuevo.
En línea: 1 Carácter: 1
+ sudo apt-get install xclip
+ ~~~~
    + CategoryInfo          : ObjectNotFound: (sudo:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

C:\Users\carlillos tole\Documents\GitHub> apt-get install xclip
apt-get : El término 'apt-get' no se reconoce como nombre de un cmdlet, función, archivo de script o programa
ejecutable. Compruebe si escribió correctamente el nombre o, si incluyó una ruta de acceso, compruebe que dicha ruta
es correcta e inténtelo de nuevo.
En línea: 1 Carácter: 1
+ apt-get install xclip
+ ~~~~~~~
    + CategoryInfo          : ObjectNotFound: (apt-get:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub> git clone https://github.com/carlillostole/proyecto_IV
fatal: destination path 'proyecto_IV' already exists and is not an empty directory.
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub>
C:\Users\carlillos tole\Documents\GitHub> ls


    Directorio: C:\Users\carlillos tole\Documents\GitHub


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----       08/06/2016     17:08                Carlillostole-swap
d-----       29/09/2016      9:25                IV16-17
d-----       29/09/2016      9:25                proyecto_IV


C:\Users\carlillos tole\Documents\GitHub> cd proyecto_IV
C:\Users\carlillos tole\Documents\GitHub\proyecto_IV [master ≡ +0 ~1 -0 !]> ls


    Directorio: C:\Users\carlillos tole\Documents\GitHub\proyecto_IV


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
-a----       29/09/2016      9:25            412 .gitignore
-a----       29/09/2016      9:25          35815 LICENSE
-a----       29/09/2016      9:41             84 README.md


C:\Users\carlillos tole\Documents\GitHub\proyecto_IV [master ≡ +0 ~1 -0 !]> git add README.md
C:\Users\carlillos tole\Documents\GitHub\proyecto_IV [master ≡ +0 ~1 -0 ~]> git commit -m "Archivo README actualizado close #1"
[master e3f74fc] Archivo README actualizado close #1
 1 file changed, 2 insertions(+)
C:\Users\carlillos tole\Documents\GitHub\proyecto_IV [master ↑]> git push origin master
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 353 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local objects.
To https://github.com/carlillostole/proyecto_IV.git
   e41ddc2..e3f74fc  master -> master
C:\Users\carlillos tole\Documents\GitHub\proyecto_IV [master ≡]> git checkout -b hito0
Switched to a new branch 'hito0'
C:\Users\carlillos tole\Documents\GitHub\proyecto_IV [hito0]> git push origin hito0
Total 0 (delta 0), reused 0 (delta 0)
To https://github.com/carlillostole/proyecto_IV.git
 * [new branch]      hito0 -> hito0
C:\Users\carlillos tole\Documents\GitHub\proyecto_IV [hito0]> git branch
* hito0
  master
C:\Users\carlillos tole\Documents\GitHub\proyecto_IV [hito0]>