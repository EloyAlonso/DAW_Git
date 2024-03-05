# Guía de GIT

Aquí veremos una guía resumen de los comandos más importantes y utilizados en GIT, para qué funcionan y cómo se usan.
## 1. Inicio.
  - Para empezar necesitamos establecer las variables de configuración global, que son muy importantes, especialmente si estás trabajando con otros desarrolladores. La principal ventaja de esto es que es más fácil averiguar quién ha hecho un commit de      determinado bloque de código:
      ~~~
      git config --global user.name “ Tu Nombre ”
      git config --global user.email “tucorreo@correo”
      ~~~
  - Por temas de compatibilidad podemos comprobar la version antes de nada con:
    ~~~
    git --version
    ~~~
  - Una vez hecha la configuración básica de git lo iniciamos:
    ~~~
    git init
    ~~~
  - O en caso de ya existir lo clonamos:
    ~~~
    git clone {repositorio}
    ~~~
## 2. ¿Donde estoy?
   - Este comando enumerará las ubicaciones de donde el repositorio local obtendrá los cambios realizados externamente y a dónde serán enviadas tus confirmaciones o cambios que realices al repositorio remoto:
     ~~~
     git remote -v
     ~~~
   - Con este comando verás todas las ramas que se encuentran en el repositorio, tanto local como remotamente:
     ~~~
     git branch -a
     ~~~
## 3. ¿Commit?
   - Antes de hacer un commit, que sería para guardar los cambios, se puede comprobar el estado:
     ~~~
     git status
     ~~~
   - Puedes consultar en el propio git por comandos que no recuerdes pidiendo ayuda:
     ~~~
     git help {opcional comando especifico}
     ~~~
   - Agregas lo que quieras añadir nuevo al repositorio para realizar el commit (con -A añades todo):
     ~~~
     git add {-A o archivo(s)}
     ~~~
   - Si quieres volver a la anterior versión antes de que se haga un commit, es decir borrar algun cambio en algún archivo y volver a la version inicial en la que estaba:
     ~~~
     git reset {archivo(s)}
     ~~~
     o para borrar los cambios en todos los archivos en el repositorio:
     ~~~
     git reset
     ~~~
     
   - Si quieres ver todos los cambios que se han hecho a los archivos:
     ~~~
     git diff
     ~~~
