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
git add . <!-- agrego todos los archivos que están (UNTRACKED -->