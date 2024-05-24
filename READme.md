# Comandos útiles de Git

1. git init
Va a inicializar mi repositorio, crea un nuevo repositorio local.
* git status: Muestra lista de archivos nuevos o no modificados.
2. git add . 
Va a tomar todos los archivos desde el último commit o desde el git init y los va a preparar (los sube en el stage) para el commit. 
*git add <file> : Agrega cambios específicos de un archivo al staging area. 

3. git reset .
   Revierte lo que hace el git add. Por ejemplo si nos dimos cuenta que hay archivos que no queremos subir al commit, etc.

4. git commit -m ""
"Fotografía" de mi proyecto. Guarda cambios preparados con mensaje descriptivo.

5. git checkout -- .
Para reconstruir los archivos al último commit que hice. 

6. git log
Listado de todos los commit. Apretar letra q para salir del mensaje en consola

7. git commit --amend
Arregla el mensaje del último commit. 
Te permite cambiar el último commit.
Apretar letra i para insertar nuevos textos. Para salir, apretar escape + : + wq!   ..(w:write, q: salir, ! para que lo haga inmediatamente.).
git log para ver el arreglo del commit.

8.git checkout -b nueva-rama (ó) git checkout nueva-rama  
Para agregar una nueva rama. (b de branch).
Toma lo del último commit y a partir de ahí crea una nueva rama. 
git branch para verificar las ramas existentes

9. git checkout main
main o nombre de la rama a la cual quiera cambiarme.

10. git merge nueva-rama  
Para fusionar los cambios de mi nueva rama con la rama main
+enter +escape + :wq!

11. git branch -d nueva-rama
Para eliminar una rama, por ejemplo si ya cumplió su objetivo.

12. git remote  add origin https://github.com/...
Hacer el despliegue a un repositorio externo en github por ejemplo.

13. git commit -am "mensaje"    +   git push
Para ahorrar los pasos del git add, git commit. En un archivo que ya le estabamos haciendo seguimiento. (a: agregar, m: mensaje) 

14. git diff: Diferencias entre el último commit y los cambios que no están en el staging area.

15. git fetch remote: Obtiene todas las ramas del repositorio.

16. git pull remote branch: Obtiene cambios remotos y los fusiona en la rama local.

17. git push remote branch: Envia cambios locales al repositorio remoto.

18. git merge remote: Combina los cambios remotos con la rama local actual. 

19. git rebase <branch>: Reorganiza tu rama actual para basarse en la rama especificada.

20. git revert <branch>: Deshace cambios de un commit específico sin eliminar historial de cambios.