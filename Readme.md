¿Qué comando utilizaste en el paso 11? ¿Por qué?

comando   $git reset --hard head~1

Porque nos indican que se desea poner el workingcopy como
estaba antes de hacer los cambios del ultimo commit.

Los cambios del working copy se pierden y el Staging Area queda en blanco.


- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

comando  $git reset --hard d59e7ed 

Previmente obtenemos el SHA con el comando $git reflog,
Identificamos el commit con los cambios echos al archivo como se indica el punto 9 del ejercicio.
d59e7ed HEAD@{8}: commit: modificaciones al archivo git-nuestro.md

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

$git Merge master
sin conflictos
Porque el workingcopy esta igual que el del repository.



- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

 Si causo conflicto
 la version del archivo de la rama styles es distinto a la de la rama 
htmlify, existe conflicto al hacer el merge.

>>Auto-merging git-nuestro.md
>>CONFLICT (content): Merge conflict in git-nuestro.md
>>Automatic merge failed; fix conflicts and then commit the result.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
no hubo conflicto
Fue un fat forward

 >>Updating 11a7266..d92dd8b
 >>Fast-forward
 >>git-nuestro.md | 20 ++++++++++----------
 >>1 file changed, 10 insertions(+), 10 deletions(-)


- ¿Qué comando o comandos utilizaste en el paso 25?
   git log --graph


- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
   $ git merge --no-ff title

   el objetivo principal de un merge no ff es que HEAD no paunte a la rama a la
   que se esta absorviendo, en est caso como el master y title no
   tienen ningun commit , creo que no hay problema que fuese un 
   fast forward hastaeste punto.
   si hubieran mas commits en la rama title tal vez no fuese buena idea.


- ¿Qué comando o comandos utilizaste en el paso 27?
Trate de usar el comando $ git merge --abort
pero mesalio este mensaje (no comprendi que fue lo que paso)
>>fatal: There is no merge to abort (MERGE_HEAD missing).

- ¿Qué comando o comandos utilizaste en el paso 28?
comando git reset --hard HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 29?
COMANDO $git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30?
COMANDO $git reset --hard d92dd8b

- ¿Qué comando o comandos usaste en el paso 32?
COMANDO $ git reset --hard 11a7266

¿Qué comando o comandos usaste en el punto 33?
COMANDO $ git reset --hard 768fc6b