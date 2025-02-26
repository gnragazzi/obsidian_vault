Es un VCS ([[Sistema de Contros de Versiones]]) que, a diferencia de los [[CVCSs]], es un sistema distribuido, donde cada cliente tiene una copia local del repositorio (es decir, no solo los archivos, sino toda la historia de los mismos)
***
- Git tiene un sistema de ramas (*branchs*) que permite el desarrollo no-lineal (paralelo)
- Git no piensa en los distintos commits en términos de cambios a un archivo, sino que guarda una instantanea de todos los archivos: si un archivo cambió, lo guarda en su totalidad; si no cambió guarda un puntero a la versión del commit anterior. ![[Pasted image 20250204084729.png]]
- Cambios en el area local, que luego se pueden subir al repositorio-externo/servidor
- Tres estados de un archivo en git (y cada uno de las secciones donde trabajan)
	- Modificado (Working Tree)
	- Staged (Staging Area)
	- Commit (Repository)
	![[Pasted image 20250204090153.png]]
- The basic Git workflow goes something like this:
	1. You modify files in your working tree.
	2. You selectively stage just those changes you want to be part of your next commit, which adds only those changes to the staging area.
	3. You do a commit, which takes the files as they are in the staging area and stores that snapshot permanently to your Git directory.
If a particular version of a file is in the Git directory, it’s considered committed. 
***
![[Pasted image 20250204084213.png]]