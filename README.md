# Git - Comandos y Alias

## Comandos
#### Basico
`git log --all --oneline --decorate --graph`: Muestra la historia y una grafica visual para ver el curso que ha tomado el repositorio. 

`git log --stat`: Detalle de las modificaciones de los commits.

`git diff "hash-commit-A" "hash-commit-B" `: Compara los cambios entre los dos commits, para un archivo especifico, seguido de los hash se agrega el nombre del archivo.

`git show`: Muestra los cambios del ultimo commit.

`git reset "hash-commit" --hard | --soft | --mixed`: Elimina los commits posteriores.
**hard** - elimina los cambios del stage y en los archivos.
**soft** - conserva los cambios en el stage y en los archivos.
**mixed** - elimina los cambios del stage y conserva los cambios en los archivos.

`git branch "name-branch"`: Crea una nueva rama.

`git checkout "hash-commit"`: Navegamos entre la historia de los cambios del repositorio, oara un archivo especifico agregamos el nombre del mismo.

`git checkout "name-branch"`: Nos permite cambiar de rama.

`git stash`: Si olvidaste cambiar de rama, este permite guardar los cambios en memoria para que cambies a la rama correcta para hacer el commit.

`git stash list`: Muestra los cambios que hay en memoria.

#### Configuracion basica local

`git config --global user.name "Name"`: Configura el nombre del autor.

`git config --global user.email "Email"`: Configura el correo del autor.

#### Repositorio remoto

`git clone "url-repo"`: Clonamos el repositorio que se encuentra en GitHub o GitLab. Si es privado nos pedira credenciales para autenticarnos, el propietario debe de añadirnos como colaboradores para hacerlo.

`git remote add origin "url-repo"`: Creamos la conexion entre el repositorio local y el remoto.

`git pull origin master`: Actualiza la base de datos de los cambios y las modificaciones de los archivos con los que se encuentran en el repositorio remoto. `--allow-unrelated-histories` permite fucionar los archivos de los repositorios.

`git push origin master`: Envia al repositorio remoto los cambios de los archivos que se hicieron.
