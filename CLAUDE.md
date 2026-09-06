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
