# Práctica Git, GitHub y SourceTree
## Juan A. Caballero
------------------------------------------
Paso 11: 	
git reset --hard HEAD~1 
Para volver al commit anterior y con el atributo hard actualizo mi Working Area con el contenido de este commit
			
Paso 12:	
git reflog
git reset --hard b426368
También podría hacerse volviendo a hacer los cambios en el fichero y ejecutando add + commit, o sea, volviendo a hacer el commit
 
Paso 13: 
No ha habido conflicto porque el sistema no ha necesitado ejecutar el comando merge, ya que la rama styled tiene la última actualización respecto del ultimo commit de master y la rama master no ha evolucionado. De hecho, el intento de merge nos devuelve el mensaje de que ya está actualizado.

Paso 19:
Hay conflicto, ya que ambas ramas han modificado las mismas lineas del archivo git-nuestro.md.
Resolvemos el conflicto editando el archivo git-nuestro.md para dejar las lineas indicadas y ejecutamos commit.

Paso 21:
No hay conflico al ser un fast forward, y el fichero se queda con el contenido del fichero modificado en la rama styled por ser la última y única modificación desde master, rama que no ha evolucionado.

Paso 25: 
git log --graph --decorate --pretty=oneline

Paso 26:
Si podía haber sido un fast forward, porque el merge lo que ha hecho ha sido mover el puntero al último commit de la rama title, ya que desde que creamos la rama title solo avanzó esta rama y la master no.

Paso 27:
git reset HEAD~1

Paso 28:
git checkout -- git-nuestro.md

Paso 29:
git branch -D title

Paso 30:
git reflog
git reset --hard 5280bda
Siendo 5280bda el hash abreviado del commit en el que añadimos el título en la rama title
Podría haberse hecho también con reflog + checkout + branch -b + merge, pero hubiera requerido más comandos.

Paso 32:
git reflog
git reset --hard 365a58a
Siendo 365a58a el hash abreviado del primer commit.

Paso 33:
git reflog
git reset --hard 5280bda
Siendo 5280bda el hash abreviado del commit en el que añadimos el título en la rama title.
