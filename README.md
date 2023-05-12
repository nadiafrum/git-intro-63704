# Clase 15

```sh
git config --global user.name "Maximiliano Principe"
git config --global user.email "mlapeducacionit@gmail.com"
```

## Verificamos que todo haya salido bien

```sh
git config --get-regexp user
```

## Creamos un repositorio (Inicializamos un repo)

```sh
git init
```
Nota: esto crea en la raíz del proyect la carpeta .git

## Areas del repositorio de GIT

* Working directory (WD): Directorio de trabajo donde se van agregar o quitar los archivos durante el desarrollo.
* Staging Area (SA): Area de control de cambios. Área temporal/intermedia.
* Local Repo (LR): Es una caja donde voy a ir teniendo todas las fotos que vaya sacando de mi código.

## El estado de los archivos

* untracked: Archivos que están en el WD pero GIT no les esta dando seguimiento. Sabe que existen pero no sabe lo que tienen dentro.)
* unmodified: Archivos que GIT ya está siguiendo y con respecto al WD, no fueron modificados
* modified: Archivos que se encuentran en el respositorio (están siendo seguidos por GIT) pero difieren con lo que se encuentra actualmente en el WD
* staged: Archivos que están en el area temporal/intermedia.

## Saber estado actual de los archivos

```sh
git status
```

## Voy a poder mover los archivos de WD al SA

```sh
git add <nombre-archivo>
git add README.md
git add README.md css/estilos.css index.html
git add . # Agrego todos los archivos que están (UNTRACKED, MODIFIED)
```

## La historia commits (La caja de fotos)


```sh
git log # La historia de commit detallada
git log --oneline # Historia resumida
```

**IMPORTANTE**: si la consola queda bloqueda y no puedo salir del listado tengo que apretar la tecla q (quit).

## Si quiero ver los cambios que tengo entre el WD y LR

```sh
git diff
```

## .GITIGNORE
Este archivo me sirve para ignorar carpetas o archivos que no quiero que sean parte del repositorio (LR). normalmente va sobre la raiz del proyecto

Necesito crear el archivo **.gitignore**

## Si quiero seguir una carpeta vacia
tengo que crear un archivo con el nombre **gitkeep** porque git no versiona carpetas vacias

```sh
touch images/.gitkeep
```


## Para subir el repositorio local al remoto

1. tengo que crear un repositorio remoto
2. seguir las instrucciobnes que correspondan para el caso
3. Agrego la url del remoto a mi repo local
4. Hago el push


# Clase 16

## Git Ramas (Branches)

### Crear una rama en el repo

```sh
git branch <nombre-que-quiero-que-tenga-la-rama>
```
### Verificar las ramas que tengo

```sh
git branch

```

### Cambiar entre ramas

```sh
git switch <nombre rama>

```



