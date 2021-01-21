# 1-Beginner

## ¿Quieres participar?
Necesitamos _4 participantes_ 👩‍💻 para contribuir en este ejercicio.
- Comparte tu nombre y **usuario de Github** por el chat del workshop cuando la _coach_ lo solicite.
- Participarán lxs 4 primerxs

## Empecemos
El proyecto consiste en crear un _banner_ para este taller y el requerimiento es que cada participante coloque su nombre y foto en donde corresponde.
![preview](https://user-images.githubusercontent.com/25912796/90475795-d134f080-e0ed-11ea-9ce0-5bbeaa3411de.png)

## Instrucciones

### Preparándonos para colaborar en un repositorio remoto (Participante 1)

- Hacer _fork_ de este [repositorio](https://github.com/MeryCardenas23/Workshop-Git-and-Github)
- Agregar al resto de las participantes como colaboradoras de tu repositorio (ir a _configuraciones_ y luego _administrar acceso_)
- Clonar tu repositorio
- Crear una rama `develop` en base a `master`
- Ejecutar `git push origin develop`

### Usando comandos de Git - Parte I (Participante 2)

- Clonar el repositorio de _participante 1_
- Crear una rama ejecutando `git checkout -b participante-2`
- Ir al archivo _index.html_ y en la línea [73](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L73) cambiar la url de _source_ con tu usuario de Github, esto mostrará tu foto en el banner.
- Ir a la línea [77](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L77) y reemplazar el texto de `H5` por tu nombre
- Ejecutar `git status`
- Ejecutar `git diff`
- Ejecutar `git add`
- Ejecutar `git commit -m 'add participant 2 info'`
- Ejecutar `git push origin participante-2`

### Usando comandos de Git - Parte II (Participante 3)

- Clonar el repositorio de _participante 1_
- Crear una rama ejecutando `git checkout -b participante-3`
- Ir al archivo _index.html_ y en la línea [86](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L86)
- Ir a la línea [90](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L90) y reemplazar el texto de `H5` por tu nombre
- Ejecutar `git stash`
- Ejecutar `git stash pop`
- Ejecutar `git add -p`
- Seleccionar los cambios realizados el la línea [86](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L86)
- Ejecutar `git commit -m 'add photo of participant 3'`
- Seleccionar los cambios realizados el la línea [90](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L90)
- Ejecutar `git commit -m 'add name of participant 3'`
- Ejecutar `git push origin participante-3`

### Siguiendo los cambios y fusionando ramas (Participante 1)
- Ejecutar `git remote add upstream [repositorio]`
- Ejecutar `git remote -v`
- Ejecutar `git fetch`
- Ejecutar `git fetch upstream`
- Crear rama local ejecutando `git checkout -b participante-2` y luego `git pull origin participante-2`
- Regresar a la rama `master` ejecutando `git checkout master`
- Crear rama local ejecutando `git checkout -b participante-3` y luego `git pull origin participante-3`
- Regresar a la rama `develop` ejecutando `git checkout develop`
- Fusionar la rama `develop` con `participante-2` ejecutando `git merge participante-2`
- Fusionar la rama `develop` con `participante-3` ejecutando `git rebase participante-3`
- Ir al archivo _index.html_ y en la línea [60](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L60)
- Ir a la línea [64](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L64) y reemplazar el texto de `H5` por tu nombre
- Ejecutar `git add`
- Ejecutar `git commit -m 'add participant 1 info'`
- Ejecutar `git fetch`
- Ejecutar `git fetch upstream`
- Ir a la rama `master` y ejecutar `git pull upstream master`
- Ir a la rama `develop` y ejecutar `git rebase master`
- Ejecutar `git push origin develop`

###  Reescribiendo la historia y enviando un pull request (Participante 4)
- Clonar el repositorio de _participante 1_
- Crear rama local `develop` ejecutando `git checkout -b develop origin/develop`
- Ejecutar `git log` o `git log --oneline -[cantidad_de_commits_a_visualizar]`
- Ejecutar `git rebase -i HEAD~[cantidad_de_commits_a_modificar]`
- Ordenar la historia de manera que el commit realizado por _participante 1_ vaya adelante del commit de _participante 2_
- Ir al archivo _index.html_ y en la línea [99](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L99)
- Ir a la línea [103](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L103) y reemplazar el texto de `H5` por tu nombre
- Ejecutar `git add`
- Ejecutar `git commit -m 'add participant 4 info'`
- Ejecutar `git push origin +develop` o `git push origin --force develop`