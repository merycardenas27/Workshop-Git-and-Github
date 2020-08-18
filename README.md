# Workshop Git y Github
En este taller :nerd_face: aprenderás o recordarás los comandos básicos de **Git** y cómo es un flujo de colaboración asíncrona en **Github**.

## Duración
1h 30min

## ¿Qué harás?
Simular el flujo de colaboración asíncrona usando Git, Github y el código implementado en este repositorio :point_up:.

## ¿Qué necesitas?
- Tener instalado Git
- Tener una cuenta en Github
- Tener instalado un editor de código y
  - Si usas _Visual Studio Code_ instala esta extensión ![Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
  - Si usas _Sublime_ instala este paquete ![Browser Sync](https://packagecontrol.io/packages/Browser%20Sync)
  - Si usas _Atom_ instala este paquete ![Live Server](https://atom.io/packages/atom-live-server)
  
## ¿Quieres participar?
Necesitamos _4 participantes_ :raising_hand: para contribuir en este proyecto.
- Busca y únete al canal `workshop-git-and-github` en slack
- Y comparte en el canal tu **usuario de Github**

## Empecemos
El código de este proyecto deberá crear un _banner_ para este taller, el requerimiento es que cada participante coloque su nombre y foto en donde corresponde.
![preview](https://user-images.githubusercontent.com/25912796/90475795-d134f080-e0ed-11ea-9ce0-5bbeaa3411de.png)


### Participante 1 (Primera colaboración)
- Clona este repositorio
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

## Coach
<img src="https://avatars3.githubusercontent.com/u/25912796?v=4" width="100px;" alt="Mery Cardenas"/>

![Mery Cardenas](https://github.com/MeryCardenas23)
