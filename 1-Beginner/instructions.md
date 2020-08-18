# 1-Beginner

## ¿Quieres participar?
Necesitamos _4 participantes_ :raising_hand: para contribuir en este proyecto.
- Busca y únete al canal `workshop-git-and-github` en slack
- Y comparte en el canal tu **usuario de Github**

## Empecemos
El código de este proyecto deberá crear un _banner_ para este taller, el requerimiento es que cada participante coloque su nombre y foto en donde corresponde.
![preview](https://user-images.githubusercontent.com/25912796/90475795-d134f080-e0ed-11ea-9ce0-5bbeaa3411de.png)

### Participante 1 (Primera colaboración)
- Haz _fork_ de este repositorio
- Revisa si hay cambios en el repositorio remoto ejecutando `git fetch` y `git merge FETCH_HEAD`
- Crea tu rama ejecutando `git checkout -b feat/banner-participant1`
- Ve al archivo `index.html` y haz los cambios requeridos
  - Comenta la línea [60](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L60)
  - Descomenta la línea [59](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L59)
  - Reemplaza esto `[github-username]` por tu usuario de Github
  - En la línea [64](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L64) reemplaza el texto de `H5` por tu nombre
- Revisa tus cambios locales usando `git status` y `git diff [file]`
- Prepara tus cambios ejecutando `git add index.html`
- Luego `git commit -m 'feat(banner): Update data of participant 1`
- Y por último `git push origin feat/banner-participant1`

### Participante 2 (Seguimiento de los cambios)
- Clona este repositorio
- Revisa si hay cambios en el repositorio remoto ejecutando `git pull origin master`
- Crea tu rama ejecutando `git checkout -b feat/banner-participant2`
- Ve al archivo `index.html` y haz los cambios requeridos
  - Comenta la línea [73](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L73)
  - Descomenta la línea [72](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L72)
  - Reemplaza esto `[github-username]` por tu usuario de Github
  - En la línea [77](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L77) reemplaza el texto de `H5` por tu nombre
- Antes de subir tus cambios revisa otra vez si hay cambios en el repositorio remoto ejecutando `git fetch`
- Revisa tus cambios locales usando `git status` y `git diff [file]`
- Ahora ejecuta `git stash` para registrar el estado actual del directorio de trabajo y el índice
- Luego `git checkout master` y `git pull origin master`
- Y `git checkout feat/banner-participant2` y `git rebase master` para actualizar tu rama con los últimos cambios
- Ahora `git stash pop` y `git add index.html` para recuperar tus cambios locales
- Luego `git commit -m 'feat(banner): Update data of participant 2`
- Y por último `git push origin feat/banner-participant2`

### Participante 3 (Enviando un Pull Request)
- Haz un _fork_ este repositorio
- Clona tu repositorio
- Ejecuta `git remote -v` para visualizar la lista de remotos de tu proyecto
- Crea un nuevo _remote_ ejecutando `git remote add upstream [original-repository-url]`
- Revisa si hay cambios en el repositorio remoto original ejecutando `git fetch upstream`
- Usa `git pull upstream master` para actualizar tu rama local `master`
- Crea tu rama ejecutando `git checkout -b feat/banner-participant3`
- Ve al archivo `index.html` y haz los cambios requeridos
  - Comenta la línea [86](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L86)
  - Descomenta la línea [85](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L85)
  - Reemplaza esto `[github-username]` por tu usuario de Github
  - En la línea [90](https://github.com/MeryCardenas23/Workshop-Git-and-Github/blob/master/index.html#L90) reemplaza el texto de `H5` por tu nombre
- En tu terminal ejecuta `git fetch upstream`
- Revisa tus cambios locales usando `git status` y `git diff [file]`
- Ejecuta `git checkout feat/banner-participant3` y `git rebase master`
- Prepara tus cambios ejecutando `git add -p index.html`
- Luego `git commit -m 'feat(banner): Update photo of participant 3`
- Y `git commit -m 'feat(banner): Update name of participant 3`
- Para terminar ejecuta `git push origin feat/banner-participant3`

### Participante 4 (Fusionando ramas)
- Clona este repositorio
- Revisa si hay cambios en el repositorio remoto ejecutando `git pull origin master`
- Haz los mismos pasos que participante 1
- Ejecuta `git checkout -b develop` y `git log --oneline`
- Luego `git checkout -b feat/banner-participant1` y `git pull feat/banner-participant1`
- También `git checkout -b feat/banner-participant2 origin/feat/banner-participant2`
- Ve a la rama `develop` y fusiona las ramas de lxs participantes 1, 2
- Acepta el _pull request_ de participante 3
- Ve otra vez a la rama `develop` y ejecutar `git pull origin develop`
- Fusiona tu rama `feat/banner-participant4`