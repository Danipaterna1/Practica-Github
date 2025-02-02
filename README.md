# Practica-Github
1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?
Utilicé el comando:
git reset --hard HEAD~1
Lo usé porque necesitaba deshacer el último compromiso y además quería perder los cambios realizados en el área de trabajo.

2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
git reflog
git reset --hard IDENTIFICADOR_DEL_COMMIT
Primero, con git reflog, localicé el hash del commit que había deshecho en el paso anterior. Luego, con git reset --hard, lo recuperé.

3. La fusión del paso 13, ¿Causó algún conflicto? ¿Por qué?
No, no causó conflictos porque en ese momento las ramas mainy styledno tenían modificaciones en común que pudieran entrar en conflicto.

4. La fusión del paso 19, ¿Causó algún conflicto? ¿Por qué?
Sí, provocó conflictos porque tanto la rama styledcomo htmlifyhabían modificado las mismas líneas del archivo git-nuestro.md.

5. La fusión del paso 21, ¿Causó algún conflicto? ¿Por qué?
No, no hubo conflictos porque la rama styledya había absorbido los cambios de htmlifypreviamente, y no había modificaciones adicionales en main.

6. ¿Qué comando o comandos utilizaste en el paso 25?
En este paso no utilicé comandos, ya que se trataba de dibujar un diagrama. Utilicé una herramienta visual para representar el flujo de trabajo.

7. El merge del paso 26, ¿Podría ser avance rápido? ¿Por qué?
No, no podría ser un avance rápido porque forcé la creación de un commit de merge explícito con la opción --no-ff.

8. ¿Qué comando o comandos utilizaste en el paso 27?
git reset --soft HEAD~1
Esto me permitió deshacer el último commit sin perder los cambios del área de trabajo.

9. ¿Qué comando o comandos utilizaste en el paso 28?
git reset --hard
Esto descartó los cambios pendientes y restauró el estado del último compromiso confirmado.

10. ¿Qué comando o comandos utilizaste en el paso 29?
git branch -d title
Este comando eliminó la rama titleporque ya no la necesitaba.

11. ¿Qué comando o comandos utilizaste en el paso 30?
git merge --no-ff title -m "Rehacer merge de la rama title en main"
Rehice el merge para asegurarme de que el historial reflejará un merge explícito.

12. ¿Qué comando o comandos usaste en el paso 32?
git checkout HASH_DEL_COMMIT_INICIAL
Esto me permitió volver al commit inicial utilizando su hash.

13. ¿Qué comando o comandos usaste en el paso 33?
git checkout main
Con este comando, regresó al estado final de la rama main.
