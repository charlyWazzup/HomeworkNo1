###### Tarea No. 1 -- `Carlos Emmanuel Botello Ovalle`

###### Diferencias entre `git reset --mixed <commit>` y `git reset --soft <commit>`

Primero que nada, `git reset` resetea la _branch_ en la que nos encontramos y haremos _commit_. Posiblemente actualize la rama principal o el árbol completo dependiendo el modo en que utilicemos el `reset`.

- Git Reset `--mixed`:

	Resetea el _index_, o rama principal, pero no el árbol completo en el que trabajamos. Los archivos modificados se conservan pero no son marcados para hacer _commit_ y nos avisa que fue lo que no se actualizó. Esta opción está por _default_.

- Git Reset `--soft`:

	En este no se toca el _index_ ni el árbol por completo, pero reseteal el _Head_ para poder hacer _commit_. Esta opción deja todos los archivos modificados como `Changes to be commited`, como _git status_ lo haría. 

Por otro lado, si hablamos de un `git reset --hard`, se resetea el index y el árbol completo. Todos los cambios antes del _commit_ seran descartados.

