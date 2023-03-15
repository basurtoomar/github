# github
Documentacion de Github


# Comandos

```c#
git --version                       Se utiliza para ver la version del git en consola
git help                            Para ver la ayuda de git
git clone urlservidor               Para clonar el repositorio en mi maquina local 
git add .                           Para agregar todos los cambio del repositorio al stage
git commit -m "Titulo del commit"   Este comando sca la foto del como esta el repositorio para subirla al head
git push origin                     Sube el commit o la foto al main 
git checkout -- .                   Toma todos los archivos del ultimo commit
git branch                          Para ver en que rama esta
git branch nombrenuevarama          Para crear una rama nueva
git checkout nombredelarama         Para cambiar entre ramas
git checkout -b nombredelarama      Crea la rama y nois mueve a ella en un solo paso
git branch -d nombrenuevarama       Borrar una Rama
git branch -d nombrenuevarama -f    Forza el borrado de la rama no importando si nunca se hizo un commit, solo en caso de estar seguros de borrar 
git commit -am "Titulo del commit"  Agrega y hace commit en un solo paso sin necesidad de git add .
git commit --amend -m "Titulo"      Actualiza el titulo del ultimo commit
git reset --soft HEAD^              Elimina el ultimo commit para poder colocar los cambios a stage
git reflog                          Muestra todos los commits en orden cronologico
git merge nombredelarama            Une la rama main o master con la rama personalizada
git pull                            Actualiza al commit mas reciente

Tecla ESC :wq!
```


# Para un alias mejorado y muy util

git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
