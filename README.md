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



#### Agregando archivos al repositorio local

```git

```
