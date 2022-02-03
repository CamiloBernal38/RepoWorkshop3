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

1. Chequea que todos los PR's que se encuentran mergueados tengan un milestone asignado, si no es así asignele el milestone correspondiente.

2. Crear rama de release 1.0 desde master

```sh
$ git checkout -b "release/1.0"
```

3. Actualizar CHANGELOG.md con los cambios que se publican.

4. Subir los cambios a la rama release

5. Generar PR para enviar los cambios del cambio de version a master

6. Crear el milestone para el siguiente release

7. Publicar el release. Como no podemos ejecutar el comando ``` fury create-version ``` para dejar publicada la version de la lib, procederemos de la siguiente manera:

- Ve al repositorio en github y en el panel derecho veras un apartado que dice "Release" y presionaremos sobre "create a new Release".
- En la seccion de tag añadiremos uno con el numero de la version de la lib.
- En la seccion de target seleccionaremos la rama release que se creo anteriormente.
- Añadimos una descripcion del release (normalmente fury añade los cambios que incluimos en el CHANGELOG.md) 
- Publicamos el release

