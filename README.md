# Crear proyecto en GIT
### Inicializar proyecto

```git
# saber la ruta donde estamos posicionados
TechSupport@ti-admin MINGW64 /d/LAB
$ pwd
/d/LAB

# crear la carpeta
TechSupport@ti-admin MINGW64 /d/LAB
$ mkdir front-bedu-test

# ir a la carpeta creada
TechSupport@ti-admin MINGW64 /d/LAB
$ cd front-bedu-test/

# iniciar el repositorio
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test
$ git init
Initialized empty Git repository in D:/LAB/front-bedu-test/.git/

# cambiar nombre de la rama principal master a main
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test (master)
$ git branch -M main
```

#### Configuracion de usuario y correo

```git
# establecer el correo electronico
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test (main)
$ git config --global user.email "loredojuanamaria@gmail.com"

# establecer el nombre de usuario
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test (main)
$ git config --global user.name "Juana Maria Loredo Vazquez"

# comprobar la configuracion
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test (main)
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=D:/Programas/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager-core
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.email=loredojuanamaria@gmail.com
user.name=Juana Maria Loredo Vazquez
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true


```

#### Creando el primer commit

```git
# listar contenido de la carpeta del proyecto
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test (main)
$ ls
README.md  index.html

# agregar todos los archivos modificados
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test (main)
$ git add .

# comprobar el estado del repositorio
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
        new file:   index.html

# realizar el commit
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test (main)
$ git commit -m "S01 -> E01"
[main (root-commit) 7891b27] S01 -> E01
 2 files changed, 73 insertions(+)
 create mode 100644 README.md
 create mode 100644 index.html


```

### Enviando los archivos del repositorio local al repositorio remoto

```git
# crear un paquete para enviar al repositorio remoto
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test (main)
$ git remote add origin https://github.com/jym-tech/front-bedu-test.git

# enviar los archivos al repositorio remoto
TechSupport@ti-admin MINGW64 /d/LAB/front-bedu-test (main)
$ git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 990 bytes | 247.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/jym-tech/front-bedu-test.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.


```

### Estructura de carpetas

```bash
D/
└── LAB/
    └── front-bedu-test
        └── index.html
```
