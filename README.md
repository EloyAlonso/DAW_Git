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

[Aquí tienes una guía básica de git-flow](/git_flow.md)

# Integración continua (CI)
La integración continua (CI) es una práctica en desarrollo de software donde los cambios de código se combinan automáticamente. 
Se ejecutan pruebas automáticas y se realiza un análisis del código para detectar errores tempranos. La retroalimentación rápida ayuda a los desarrolladores a corregir problemas de inmediato. 
También establece una base para la entrega continua, facilitando despliegues automáticos y contribuyendo a la mejora continua del proceso de desarrollo.
Es una práctica fundamental en el desarrollo ágil de software, permitiendo la detección temprana de problemas, mejorando la calidad del código y facilitando la entrega continua de software confiable.
## Herramientas de Integración Continua:
  Existen varias herramientas que pueden implementar la integración continua
  - **Jenkins:**  Una plataforma de automatización de código abierto que admite la construcción, prueba y despliegue de proyectos.
  - **Travis CI:** Una herramienta basada en la nube que integra con GitHub y realiza CI automáticamente para proyectos alojados en GitHub.
  - **CircleCI:** Proporciona integración continua y despliegue continuo en la nube, con soporte para varias plataformas y lenguajes.
  - **GitLab CI/CD:** Integrado directamente con repositorios GitLab, ofrece funcionalidades CI/CD completas con configuración basada en archivos.
  - **TeamCity:** Una herramienta de CI/CD de JetBrains con amplias capacidades de integración y personalización.
## Runners (Ejecutores)
  - Los "runners" son componentes que ejecutan trabajos de CI/CD. Pueden ser máquinas virtuales, contenedores o incluso instancias compartidas.
## Pipelines
  - Una pipeline es un conjunto de pasos o trabajos que se ejecutan en secuencia o de manera paralela. Define el flujo de trabajo de CI/CD, desde la construcción hasta el despliegue.
## Stages (Etapas)
  - Las etapas son fases dentro de una pipeline que agrupan trabajos relacionados. Pueden incluir pasos como compilación, pruebas, y despliegue.

En resumen, las herramientas gestionan los flujos de trabajo de CI/CD, los runners ejecutan los trabajos, las pipelines definen la secuencia de tareas, y las stages agrupan trabajos relacionados en etapas específicas del proceso. 
Estas herramientas y conceptos forman la base de la automatización de la integración continua y la entrega continua en proyectos de desarrollo de software.
