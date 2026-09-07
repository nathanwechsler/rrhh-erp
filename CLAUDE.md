# CLAUDE.md

Reglas para trabajar en este repositorio (Prime Chef · RRHH).

## Flujo de trabajo
- Al terminar cualquier cambio solicitado, automáticamente hacer `git add`, `git commit` (mensaje corto en español) y `git push` a `main`, salvo que el usuario indique lo contrario explícitamente.
- Antes de realizar cualquier cambio grande, resumir brevemente qué se va a modificar antes de hacerlo.

## Identidad visual (Prime Chef)
- Respetar siempre los colores de marca:
  - Naranjo: `#FE5E19`
  - Gris: `#DCDCDC`
  - Blanco: `#FFFFFF`
- Tipografía: **Inter**.

## Arquitectura
- Mantener la arquitectura existente, no introducir frameworks ni build steps:
  - `index.html` único (HTML + CSS + JS vanilla).
  - Google Apps Script como API.
  - Google Sheets como base de datos.

## Backend Apps Script
- El código del backend vive en la carpeta `apps-script-backend/`, sincronizado con Google Apps Script vía clasp.
- Puedes editar los archivos `.gs` y `.json` de esa carpeta libremente.
- Puedes correr `clasp push` desde esa carpeta para subir cambios de código a Apps Script.
- NUNCA corras `clasp deploy` bajo ninguna circunstancia. Ese paso lo hace Nathan manualmente desde el editor web de Apps Script, porque puede generar una nueva URL de despliegue y romper la conexión con el frontend.
- `apps-script-backend/` está en `.gitignore` y no se sube a GitHub — se sincroniza solo con clasp.
