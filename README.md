# github
Documentación de Github

# Configuraciones globales

```
git config --global user.name       Configuramos el usuario que estara trabajando la rama
git config --global user.mail       Configuramos el correo de email que estara trabajando la rama
git config --global init.defaultBranch main       Configuramos la rama por default main o podemos cambiarla a la rama que querramos solo cambiando el nombre de main por        cualquiera
git config --global -e              Muestra la configuracion global del repositorio
:q!                                 Para salir de pantalla bloqueada
```

# Comandos

| Command | Description |
| --- | --- |
| git --version | Se utiliza para ver la version del git en consola |
| git help | Para ver la ayuda de git |
| <span style="background-color:green;">git init</span> | Inicializa el git  |                            
| <span style="background-color:green;">git clone urlservidor</span> |             Para clonar el repositorio en mi maquina local | 
|<span style="background-color:green;">git add .</span>|                           Para agregar todos los cambio del repositorio al stage|
|<span style="background-color:green;">git commit -m "Titulo del commit"</span>|   Este comando sca la foto del como esta el repositorio para subirla al head|
|<span style="background-color:green;">git push origin</span>|                     Sube el commit o la foto al main| 
|git checkout -- . |                  Toma todos los archivos del ultimo commit |
|git branch |                         Para ver en que rama esta|
|git branch nombrenuevarama|          Para crear una rama nueva|
|git checkout nombredelarama|         Para cambiar entre ramas|
|git checkout -b nombredelarama |     Crea la rama y nois mueve a ella en un solo paso|
|git checkout -- . |
|git branch -m master main  |         Este comando cambia el nombre de la Rama master a main|
|git branch -d nombrenuevarama|       Borrar una Rama|
|git branch -d nombrenuevarama -f |   Forza el borrado de la rama no importando si nunca se hizo un commit, solo en caso de estar seguros de borrar |
|git commit -am Titulo del commit |   Agrega y hace commit en un solo paso sin necesidad de git add .|
|git commit --amend -m Titulo |       Actualiza el titulo del ultimo commit |
|git reset --soft HEAD^    |          Elimina el ultimo commit para poder colocar los cambios a stage |
|git reflog    |                      Muestra todos los commits en orden cronologico |
|git merge nombredelarama   |         Une la rama main o master con la rama personalizada |
|git pull   |                         Actualiza al commit mas reciente |
|git tag      |                       Muestra los tag en el repositorio |
|git tag nombredeltag      |          Una etiqueta para el commit  |
|git tag -d nombredeltag   |          Para boorar el tag de los commit |
|git tag -a v1.0.0 -m "Ver 1.0.0"  |  Va al ultimo commit y agrega un tag para identificar la version |
|git tag -a v0.1.0 701c885 -m "Anota"| Si queremos colocar un tag a un commit especifico copiamos el hash del commit |
|git show v0.1.0   |                  Para ver mas informacion del tag |
|git stash       |                    Graba todo el directotio y lo indexa sin hacer un commit |
|git stash list  |                    Muestra el listado de Stash |
|git stash pop   |                    Recupera el ultimo stash para continuar trabajando |
|git stash clear |                    Borra todos los stage |
|git stash show nombrestash  |        Visualizar que cambio en el stash |
|git stash save "Agregamos MSG" |     Se guarda el stash con una descripcion de los archivos |
|git stash list --stat  |             Muestra el listado de stash con sus descripciones |

Tecla ESC :wq!




El stash es una boveda de los archivos que no han hecho un commit 

# Para un alias mejorado y muy util

git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
