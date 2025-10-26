# Libro (Vault de Obsidian)

## Descripción

Este repositorio contiene un vault de Obsidian pensado como borrador/compilación de un libro sobre apologética y defensa de la fe católica. Aquí se almacenan notas, capítulos y materiales de referencia en formato Markdown.

Contenido principal:

- Apologética.md — notas y capítulos sobre apologética.
- GEMINI.md — (archivo de referencia / nota temática).

## Objetivo

Mantener un repositorio organizado con las notas del libro para:

- Facilitar edición, versión y colaboración mediante Git.
- Mantener copias de seguridad y un historial de cambios.
- Generar versiones (exportar) cuando se desee compilar el libro.

## Estructura recomendada

- `Apologética.md` — capítulo(s) o sección principal(es) sobre apologética.
- `assets/` — (opcional) imágenes, gráficos y recursos.
- `drafts/` — (opcional) borradores que no formen parte del manuscrito principal.

Actual: los archivos en este repo al momento son los listados arriba.

## Cómo usar

1. Abrir esta carpeta como Vault en Obsidian: Archivo → Abrir carpeta como vault (selecciona la carpeta del repositorio).
2. Editar las notas en Obsidian o en cualquier editor de texto (Markdown).
3. Hacer commits frecuentes para preservar el historial:

	- Recomendación mínima de flujo con Git:

```powershell
git add .
git commit -m "Actualiza Apologética: sección X"
git push origin main
```

4. Hacer copias de seguridad periódicas (por ejemplo, usando GitHub, un disco externo o servicios en la nube).

## Recomendaciones de Obsidian

- Plugins sugeridos: "YAML Frontmatter", "Markdown Table Formatter", "Pandoc Plugin" (si quieres exportar a DOCX/PDF) y "Templater".
- Usa Frontmatter en la parte superior de cada nota para metadatos (título, fecha, estado):

```yaml
---
title: "Título de la nota"
date: 2025-10-26
status: draft
---
```

## Convenciones de escritura

- Mantén títulos y subtítulos consistentes (usar #, ##, ###).
- Usa enlaces internos de Obsidian [[Nombre de nota]] para referencias cruzadas.
- Mantén imágenes en `assets/` y referencia mediante rutas relativas.

## Contribuir

1. Haz un fork o crea una rama nueva para tus cambios:

```powershell
git checkout -b feature/nueva-seccion
```

2. Haz commits pequeños y descriptivos.
3. Abre un pull request para revisión.

Si colaboras directamente con el autor, comenta o crea issues para discutir grandes cambios.

## Licencia

Añadir una licencia si corresponde. Por defecto, este repositorio no incluye una licencia explícita. Si quieres una recomendación, se puede añadir MIT o CC-BY para contenidos textuales.

## Contacto

Autor / repositorio: `biglexj` (GitHub).

## Notas finales

Este README es una plantilla inicial pensada para ser ampliada. Si quieres, puedo:

- Añadir una plantilla de capítulo en `drafts/`.
- Crear un archivo `CONTRIBUTING.md` con normas más detalladas.
- Añadir un script de exportación con Pandoc para generar PDF/EPUB.

---

Fecha de última actualización: 2025-10-26
