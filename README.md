# Clase 15

## Configuración inicial.

git config --global user.name "Hernan Bianchimano"
git config --global user.email "hernanbianchimano@gmail.com"

## Verificar si todo quedo bien o si hice estas configuraciones

git config --get-regexp user

## Crear un repositorio.

git init

## Areas del repositorio de GIT

* Working Directory (WD) <!-- Directorio de trabajo donde se van agregando o quitando los archivos durante el desarrollo-->

* Staging Area (SA) <!-- Area de control de cambios. Area temporal intermedia, lugar donde se saca la foto -->

* Local Repo (LR) <!-- Caja donde voy a ir teniendo todas las fotos que vaya sacando -->

## El estado de los archivos

* untracked: (Archivos que estan en el WD pero GIT no les está dando seguimiento)
* unmodified: (Archivos que GIT ya está siguiendo y con respecto al WD, no fueron modificados)
* modified: Archivos que se encuentran en el repo, seguidos por GIT, pero difieren con lo que se encuentra actualmente en el WD.
* staged: Archivos que están en el área temporal/intermedia

## Saber estado actual de los archivos

git status

## Voy a poder mover los archivos del WD al SA

git add <nombre-archivo>
git add index.html
git add README.md css/estilos.css
git add . <!-- agrego todos los archivos que están (UNTRACKED, MODIFIED) -->

## Para ver la historia de commits (La caja de fotos)

git log (La historia de commit detallada)
git log --oneline (La historia resumida)

Nota: si la consola queda bloqueada y no puedo salir del listado tengo que apretar la tecla q (quit)

## Si quiero ver los cambios que tengo entre el WD y LR

git diff


## Clase 16

## .gitignore
Este archivo me sirve para ignorar carpetas o archivos que no quiero que sean parte del repositorio. Normalmente va sobre la raíz del proyecto.

Necesito crear el archivo **.gitignore**

" " "  sh
touch .gitignore

## Ayuda de GIT 

""" sh
git restore --help
"""

## Agrego a mi repo local la url del repo remoto

"""sh
git remote add origin https://github.com/HernanB65/bootcamp-lu-jue.git
"""

### Visualizar si se agregó o qué url tengo agregada

""" sh
git remote -v
"""

### Crear una rama

"""sh
git branch <nombre-rama>
git branch ramas
"""

