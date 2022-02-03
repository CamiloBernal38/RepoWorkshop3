# Ejercicio de Release Process
## Setup

Necesitará realizar un Fork y clonar localmente este proyecto.

Siga los pasos a continuación.

### Realiza Fork al Repositorio Origen

   1. Visita https://github.com/christianbernal38/RepoWorkshop3
   2. Click en el botón "Fork" y elija su cuenta personal de GitHub si le solicita.

### Clona tu Fork

Clona este proyecto en tu máquina:
```sh
$ cd ~/my/parent/directory
# clona el repositorio
$ git clone https://github.com/christianbernal38/RepoWorkshop3.git

# cambia el directorio de trabajo al repositorio clonado
$ cd repo-name
```

Ver controles remotos existentes:
```sh
$ git remote
origin

$ git remote -v
origin https://github.com/username-source/repository-name.git (fetch)
origin https://github.com/username-source/repository-name.git (push)
```

## Ejercicio
### Verificar PR's a incluir en el Release
Chequea que todos los PR's que se encuentran mergueados tengan un milestone asignado, si no es así asignele el milestone correspondiente.

Crear rama de release 1.0 desde master

```sh
$ git checkout -b "release/1.0"
```

Actualizar CHANGELOG.md con los cambios que se publican.

Subir los cambios a la rama release

Generar PR para enviar los cambios del cambio de version a master

Crear el milestone para el siguiente release







