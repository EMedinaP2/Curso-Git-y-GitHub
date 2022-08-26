
## **Como se organizan los paramétros de los comandos**
- abreviaturas
-- palabras completas


### Principales comandos de Git 

#### git --version 
* Ver la version de git
#### git help 
* Ayuda en git
#### git clone  
* Clona los repositorios de git
#### git help <comando> 
* ver ayuda de un comando en git
#### git config --global user.name 
* Define el nombre del usuario
#### git config --global user.email 
* Define el email del usuario
#### git config --global -e 
* Abre una pantalla para configurar al usuario
#### git init 
* Inicializa un repositorio en esta carpeta.El comando init crea una carpeta oculta .git Nunca borrar.
#### git config --global init.defaultBranch <name> 
* Lo mismo que init pero se asigna un nombre a la rama principal.
#### git status 
* Da información sobre el repositorio, rama, version, etc.
#### git add 
* Añade el archivo al Staged 
#### git add .
* Añade todos los archivos
#### git reset  
* Remueve un archivo del Staged
#### git commit  
* Realiza un commit , mueve los archivos del Staged al repositorio
#### git checkout -- .
* Regresa los archivos del working area a lo subido en el ultimo commit
#### git checkout -- nombre 
*   Regresa a lo guardado en el ultimo commit del repositorio de un arhico
#### git branch 
* Nos dice en que rama nos  encontramos trabajando
#### git branch -m 
* Cambiar nombre de la rama
#### git add *.extension  
* Agrega al Stage todos los archivos de una extension
#### .gitkeep 
* Archivo especial de git para mantener un folder vacio
#### git diff 
* Se ve la diferencia de un archivo en el working area con el repositorio
#### git commit --amend -m "" 
* Corrige el mensaje del commit
#### git reset --soft HEAD^ 
* Regresa al ultimo commit hecho en el repositorio                                                                                                
#### git reset --Hard HEAD^ 
* Elimina los  commit hecho en el repositorio  hasta la referencia dada, tambien sirve para moverse a otra otra referencia de Commit recuperando
todo los comits hasta ese.
#### git reflog 
* Muestra los hashes de todos los commits hechos aunque se hayan borrado
#### .gitignore 
* Los nombres de archivos que esten aqui son ignorados por git
#### git tag 
* Crea una tag para el commit actual
#### git tag -d 
* Eliminar una etiqueta
#### git show tag-name 
* Muestra infromacion de la tag y alcommit al que esta relacionado
#### git stash 
* Almacenar cambios del working area en un stash y los elimina del working area
#### git stash list 
* Lista todos los stash
#### git stash clear 
* Borra todos los stash
#### git stash show "stash@{2}" 
* Ves lo que hace el stash
#### git stash drop "stash@{2}" 
* Borra el stash con ese nombre
#### git stash pop 
* Borra el primer stash, el del numero 0
#### git stash save "Agregamos a loki en villanos" // agrega mas informacion al stash
* git stash list --stat // mas informacion de cada stash
#### git rebase  
* Pone adelante de los commits de una rama los de otro
#### git rebase -i HEAD~4 
* Abre el modo de edicion de rebase
    * squash // unedos commits adyacentes
    * reword // editar el mensaje de los commits
    * edit // permite editar commitsgir   
#### git Fetch 
* Permite ver los cambios que recibido una rama sin hacer merg
#### git remote prune origin  
* Elimina las referencias de las ramas del repositorio remoto en el repositorio local 
    