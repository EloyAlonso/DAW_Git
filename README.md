# GIT

## ¿Qué es un Sistema de Control de Versiones?

Un Sistema de Control de Versiones (VCS) es una herramienta que registra y gestiona cambios en archivos a lo largo del tiempo. Permite rastrear las modificaciones, revertir a versiones anteriores, colaborar en proyectos y coordinar el trabajo entre múltiples personas. Dos tipos principales son los VCS centralizados (como SVN) y los distribuidos (como Git), siendo Git ampliamente utilizado debido a su eficiencia y capacidad descentralizada.

## Git es la mejor alternativa
  1. **Git como la mejor alternativa**
    Git es preferido por su descentralización, permitiendo a los desarrolladores trabajar sin conexión, su eficiente manejo de ramas facilitando la colaboración y experimentación, y su rápida velocidad en operaciones locales.
  2. **Funcionamiento externo de git**
    Permite trabajar localmente en tu máquina y conectarte externamente a repositorios remotos. Los desarrolladores pueden descargar (pull) y enviar (push) cambios a estos repositorios. Git facilita la colaboración mediante la creación de ramas para trabajar en funciones específicas y la posibilidad de fusionar cambios. 
  3. **Estructura interna de git**
    Git tiene tres áreas principales: el directorio de trabajo para archivos, el área de preparación para organizar cambios, y el repositorio local para almacenar versiones confirmadas. Los objetos internos incluyen blobs para contenido, trees para directorios, y commits para conjuntos de cambios. Git registra la historia eficientemente, permitiendo ramificar y fusionar fácilmente.

[Aquí tienes una guía de GIT](/GuiaGIT.md)


# Git-Flow: Ventajas, Necesidades y Motivos

## Ventajas
1. **Estructura Clara:** Define un esquema claro para el desarrollo con ramas específicas.
2. **Facilita la Colaboración:** Reglas y convenciones que simplifican la colaboración en proyectos grandes.
3. **Manejo de Versiones:** Permite una gestión efectiva de las versiones y desarrollo concurrente.

## Necesidades
1. **Proyectos a Largo Plazo:** Ideal para proyectos extensos que requieren gestión estructurada de versiones.
2. **Equipos Grandes:** Útil en entornos con equipos numerosos y necesidad de coordinación.
3. **Releases Frecuentes:** Beneficioso para proyectos con lanzamientos frecuentes.

## Motivos para Utilizar Git-Flow
1. **Flujo Estandarizado:** Ofrece un flujo de trabajo estándar para una adopción y comprensión más sencillas.
2. **Seguimiento de Funcionalidades:** Facilita el seguimiento de nuevas funciones mediante ramas específicas.
3. **Gestión de Versiones Simplificada:** Estructura organizativa y procedimientos claros para una gestión de versiones simplificada.

Existen Workflows alternativos como:
### GitHub Flow

- **Características:**
  - Simple y efectivo.
  - Enfocado en despliegues continuos.
  - Usa principalmente la rama `main` y ramas de características.

- **Pasos Clave:**
  1. **Branch:** Crea una rama para cada función o corrección.
  2. **Commit:** Realiza commits en la rama.
  3. **Pull Request (PR):** Abre un PR para revisar y discutir cambios.
  4. **Merge:** Fusiona la rama en `main` después de la revisión.

### GitLab Flow

- **Características:**
  - Similar a GitHub Flow pero con etapas adicionales.
  - Orientado a la gestión de releases.

- **Pasos Clave:**
  1. **Branch:** Crea una rama para cada función o corrección.
  2. **Commit:** Realiza commits en la rama.
  3. **PR/Merge Request (MR):** Abre un MR para revisar y discutir cambios.
  4. **Review:** Revisa y aprueba el MR.
  5. **Merge:** Fusiona la rama en `main`.
  6. **Release:** Crea una rama de release desde `main`.
  7. **Preparación de Release:** Realiza correcciones y pruebas finales.
  8. **Merge a Main:** Fusiona la rama de release en `main`.
  9. **Tag:** Crea un tag para la versión.

Poner aqui link de git-flow tutorial
