# Configuración de Despliegue Automático en GitHub Pages

## 1. Configuración del Repositorio

- Ve a la configuración de tu repositorio en GitHub.
- Desplázate hasta la sección "GitHub Pages".

## 2. Seleccionar la Rama para el Despliegue

- En la opción "Source", elige la rama desde la cual deseas desplegar tu sitio.
- Puedes seleccionar la rama principal (`main` o `master`) u otra rama específica donde tengas el código listo para desplegar.

## 3. Habilitar GitHub Actions (Opcional)

- Si deseas automatizar el despliegue, puedes configurar GitHub Actions.
- Crea un archivo `.github/workflows/pages.yml` en tu repositorio con la configuración para la acción de despliegue.

```yaml
name: Deploy to GitHub Pages

on:
  push:
    branches:
      - main  # o la rama desde la cual deseas desplegar

jobs:
  deploy:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2

      - name: Deploy to GitHub Pages
        run: |
          # Comandos para construir o preparar el sitio
          # Comandos para desplegar el sitio
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

- Este archivo ejecutará la acción de despliegue automáticamente cada vez que hagas un push a la rama especificada.

## 4. Despliegue Manual (Opcional)

- También puedes realizar un despliegue manualmente ejecutando los comandos necesarios en tu máquina local y luego haciendo push a la rama seleccionada.

## 5. Verificar el Despliegue

- Una vez configurado, verifica que tu sitio se haya desplegado correctamente en la URL proporcionada por GitHub Pages.
