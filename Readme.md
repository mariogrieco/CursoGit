# Commandos
 ##  global conf
   - git config --global user.name <"name">
   - git config --global user.email <"emai">

 ## Agregando, quitando y viendo el estado de archivos (git add | rm | status)
  - git status
  - git add -A (track)
  - git add <file|.> (track)
  - git rm -f <file> (fuerza la eliminacion de un archivo del staging y del working directory)
  - git add -n <file> (simula que agrega un archivo al staging, valida que existe un archivo, y si esta en .gitignore)
  - git rm --cached <file> (elimina un archivo solo del staging area, unstage)

 ## git commit (Confirmando cambios)
  - git log (nos muestra la historia de todos los commits que hemos realizados.)
  - git commit -m 'msg'
  - git commit -m 'msg' --amend (concatenar cambios o confirmaciones)
      git commit --amend = Modificar la última confirmación de cambios (commit). Dos suelen ser los cambios básicos a realizar: cambiar el mensaje o cambiar los archivos añadidos, modificados o borrados. 
      git commit --amend (solo sin -m)

 ## git tag (Etiquetando confirmaciones, control de versiones del proyecto)
  - ligeras 
    - git tag 0.5
  - anotadas
    - git tag -a 0.5 -m 'anotation'
  
  - git tag -l (ver lista de tags)

  - se pueden etiquetar versiones pasadas ( sha1 )
    git tag x.x <sha1>
    
  - git tag -d <name> (delete)
  - git tag -f ... <sha1> (no borra)

  ## Revisando la historia de nuestro proyecto (git log) [argumento encadenables] me permite ver ref a commits pasados
   - git log --stat
   - git log --oneline --graph 
   - git log -1 (ver contando desde el ultimo commit 1, puedo cambiar o limitar la cantidad a mostar)

# Working directory
  untracked files, modificaiones y sin confirmar
# Staging Area
  archivos con seguimiento
# Repo
  cambios confirmados
