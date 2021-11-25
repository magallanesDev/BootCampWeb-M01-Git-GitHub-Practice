
# FULL STACK WEB BOOTCAMP - XII Edition - KeepCoding

## PRACTICE M01 - Git & GitHub

### Mario Filgueiras - magallanesdeveloper@gmail.com


### ***EJERCICIO 1:***

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
`git reset --hard HEAD~1`  añadiendo --hard conseguimos modificar el workingCopy al estado anterior al commit que estamos deshaciendo. El stagingArea queda vacío con y sin --hard.

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
`git reflog` y localizamos el hash del commit al que queremos volver (92984ea).
`git reset 92984ea` para rehacer el último commit, es decir, nos movemos hasta el citado commit (puntero HEAD y rama styled).
Como se me olvidó poner --hard para rehacer el workingCopy también, añado el siguiente comando:
`git restore git-nuestro.md`

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
`git merge master` no causó ningún conflicto porque el merge no produce ningún efecto, nos quedamos en el mismo commit porque no hay nada que absorber, estamos al día ("already up to date").

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
`git merge htmlify` causa un conflicto en el archivo git-nuestro.md porque es un merge no-fast-forward y tenemos dos versiones distintas del mismo en las ramas que queremos mergear (styled y htmlify).

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
`git merge styled` no causa ningún conflicto porque es un merge fast-forward.

- ¿Qué comando o comandos utilizaste en el paso 25?
`git graph` porque ya había creado anteriormente el alias global con el comando `git config --global alias.graph "log --graph --pretty=oneline"

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
`git merge --no-ff title`
En este caso el merge podría ser fast-forward porque las dos ramas a mergear (master y title) tienen un origen común.

- ¿Qué comando o comandos utilizaste en el paso 27?
`git reset HEAD~1`

- ¿Qué comando o comandos utilizaste en el paso 28?
`git restore git-nuestro.md` 

- ¿Qué comando o comandos utilizaste en el paso 29?
`git branch -D title` 

- ¿Qué comando o comandos utilizaste en el paso 30?
`git reflog` y localizamos el hash del commit al que queremos volver (8843904) para rehacer el merge.
`git reset --hard 8843904` y vamos al citado commit.

- ¿Qué comando o comandos usaste en el paso 32?
`git reflog` y localizamos el hash del commit inicial (1fc5e07).
`git checkout 1fc5e07` y vamos al commit en cuestión (estaríamos en 'detached HEAD' state).

- ¿Qué comando o comandos usaste en el punto 33?
`git reflog` y localizamos el hash del commit del estado final al que queremos volver (8843904).
`git checkout 8843904` y vamos a ese commit.



