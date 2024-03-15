# Implementación de la Integración Continua con Hugo en GitLab

## 1. Configuración de GitLab Pages:

- Ve a la página de configuración de tu proyecto en GitLab.
- Navega hasta la sección "Pages" y habilita las GitLab Pages para tu proyecto.
- Configura la rama fuente y la carpeta pública (`public`) donde Hugo generará el sitio estático.

## 2. Creación de un Archivo `.gitlab-ci.yml`:

- En la raíz de tu repositorio, crea un archivo llamado `.gitlab-ci.yml`.
- Este archivo contendrá las instrucciones para la integración continua con GitLab CI.

## 3. Configuración del Archivo `.gitlab-ci.yml`:

```yaml
image: registry.gitlab.com/pages/hugo:latest

variables:
  GIT_SUBMODULE_STRATEGY: recursive

pages:
  script:
    - hugo
  artifacts:
    paths:
      - public
  only:
    - main  # o la rama desde la cual deseas desplegar
```

- Este archivo utiliza la imagen oficial de GitLab Pages para Hugo.
- Especifica que se debe ejecutar Hugo para generar el sitio estático.
- Configura que solo se ejecute en la rama principal (`main`), pero puedes ajustarlo según tus necesidades.

## 4. Guarda y Sube los Cambios:

- Guarda los cambios en el archivo `.gitlab-ci.yml`.
- Haz un commit y haz push de tus cambios al repositorio en GitLab.

## 5. Verificación:

- GitLab CI ahora ejecutará automáticamente la compilación del sitio Hugo cada vez que se realice un commit en la rama especificada.
- Una vez que se complete la compilación, el sitio estático se desplegará en GitLab Pages.
