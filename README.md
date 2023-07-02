# Práctica Git

## 1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?
*git reset HEAD~1* para que el puntero HEAD y el puntero de la rama styled apunten al commit anterior 
git restore git-nuestro.md para volver a la versión anterior del archivo git-nuestro.md (borrar los cambios)
Podría haber usado *git reset --hard HEAD~1* pero es más peligroso y he preferido ir por pasos. 

## 2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
*git reflog* para buscar en qué commit aparecía por última vez el último cambio (el que quiero recuperar)
*git reset --hard 20cb489* para mover la rama styled y head a esa rama

## 3. El merge del paso 13. ¿Causó algún conflicto? ¿Por qué?
He hecho un merge No fast forward para que se cree un nuevo commit y quede constancia de este merge. 
Con el comando git merge main no se hace merge porque en realidad ya están "merged" las dos ramas, es decir, Styled ya puede acceder a todos los commits de la rama main.
No ha habido conflictos porque el último commit de la rama main es un git parent del último commit de la rama styled. 

## 4. El merge del paso 19. ¿Causó algún conflicto? ¿Por qué?
Sí, porque ambas ramas tienen commits con cambios en el mismo archivo. 

## 5. El merge del paso 21. ¿Causó algún conflicto? ¿Por qué?
No, porque no hay cambios distintos en el archivo para cada rama. 

## 6. ¿Qué comando o comandos utilizaste en el paso 25?
*git log --graph --branches --oneline*

## 7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Sí, porque al hacer el merge y pasar la rama main hasta el commit donde está la rama title, ningún commit queda innaccesible. 

## 8. ¿Qué comando o comandos utilizaste en el paso 27?
Para deshacer el merge sin perder los cambios he usado *git reset HEAD~1*.

## 9. ¿Qué comando o comandos utilizaste en el paso 28?
Para descartar los cambios he usado git restore git-nuestro.md.

## 10. ¿Qué comando o comandos utilizaste en el paso 29?
*git branch -D title*

## 11. ¿Qué comando o comandos utilizaste en el paso 30?
*git reset --hard f0e7b1d*

## 12. ¿Qué comando o comandos utilizaste en el paso 32?
*git reset 0c7b75b*

## 13. ¿Qué comando o comandos utilizaste en el paso 33?
*git reset a303d09*
