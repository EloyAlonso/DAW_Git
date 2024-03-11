# Git flow
El flujo de trabajo Git-flow es una extensión del flujo de trabajo de Git que establece una estructura y un conjunto de reglas para gestionar el desarrollo de software. 
Aquí veremos un resumen del funcionamiento de Git-flow:

## Iniciar
   - Para iniciar Git-flow en tu repositorio:
   ~~~
    git flow init
   ~~~
   Esto establece las ramas principales (master y develop) y configura la estructura del flujo de trabajo.
## Desarrollo de funcionalidades
  - Crear una nueva rama para cada nueva funcionalidad o característica:
  ~~~
    git flow feature start nombre_feature
  ~~~
  - Puedes realizar commits en la rama de la feature y para finalizar la funcionalidad cuando esté completa:
  ~~~
    git flow feature finish nombre_feature
  ~~~
  Esto fusionará la rama de la característica con la rama develop.
## Correcciones Rápidas (Hotfix)
  - Crear una rama de hotfix para solucionar problemas críticos en producción:
  ~~~
    git flow hotfix start nombre_hotfix
  ~~~
  - Puedes realizar los cambios que quieras y finalizar el hotfix con:
  ~~~
    git flow hotfix finish nombre_hotfix
  ~~~
  Esto aplicará los cambios tanto a master como a develop.
## Lanzamientos (Releases)
  - Crear una rama de release para preparar una nueva versión:
  ~~~
    git flow release start nombre_release
  ~~~
  - Puedes realizar los ajustes finales y finalizar el lanzamiento con:
  ~~~
    git flow release finish nombre_release
  ~~~
  Esto fusionará la rama de release con master y develop, y aplicará un nuevo tag.
## Integración Continua:
  - La rama develop siempre refleja la versión en desarrollo.
  - La rama master refleja la versión estable actual.
