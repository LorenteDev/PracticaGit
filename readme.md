#Preguntas y respuestas

##¿Qué comando utilizaste en el paso 11? ¿Por qué?
`git reset --hard HEAD~1`

Deshace el último commit, volviendo al anterior. Con la instruccion `--hard` también deshace físicamente los cambios realizados en el commit más reciente.


##¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Primero utilicé `git reflog` para ver la identificación del commit al que quiero apuntar.
Tras ello, `git reset --hard 609ef50`, teniendo en cuenta que no para todos será el mismo hash.
No se puede volver a dicho commit de otra forma, porque se pueden acceder a los padres con `HEAD~n`, pero nunca a los hijos.


##El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
Un conflicto no. Al estar ambas ramas en el mismo commit, las dos están en un mismo estado, por lo que no hay cambios a la hora de hacer merge.


##El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Sí, ya que las dos ramas tienen el mismo archivo, pero con diferentes líneas. Por lo que hay que modificar el archivo resolviendo las diferecias para poder completar el merge.


##El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
No. No puede haber conflictos cuando no existe una bifurcación entre ambas ramas. La rama se ha actualizado hasta la más actual siguiendo los cambios que se han realizado.


##¿Qué comando o comandos utilizaste en el paso 25?
Utilicé un alias global. El comando que realiza es `git log --graph --oneline`


##El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Sí, porque se el commit en el que se encontraba master era accesible desde el commit en el que se encontraba la rama title.


##¿Qué comando o comandos utilizaste en el paso 27?
`git reset --soft HEAD~1`


##¿Qué comando o comandos utilizaste e el paso 28?
`git checkout master`


##¿Qué comando o comandos utilizaste en el paso 29?
`git branch -D title`


##¿Qué comando o comandos utilizaste en el paso 30?
`git reflog` para revisar los cambios, y luego `git reset 062e038`

##¿Qué comando o comandos usaste en el paso 32?
`git reflog` para revisar los cambios, y luego `git reset --hard 43fca95` 


##¿Qué comando o comandos utilizaste en el punto 33?
`git reflog` para revisar los cambios, y luego `git reset --hard b791570`
