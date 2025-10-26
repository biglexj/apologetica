# Contexto del Proyecto: Libro de Apologética Católica

## Descripción General del Proyecto

Estoy escribiendo una serie de libros de **apologética católica** con las siguientes características:

### Especificaciones del Libro

- **Formato**: A5 (148 × 210 mm)
- **Tipo**: Didáctico, estilo catecismo
- **Estructura**: Máximo 5 capítulos por libro
- **Extensión**: Pocos páginas por libro (conciso y directo)
- **Serie**: Será dividido en varios libros temáticos
- **Público**: Católicos que buscan profundizar en su fe y defender sus creencias

### Temas a Cubrir

Los libros abordarán temas de apologética católica como:
- Fundamentos de la fe
- Escritura y Tradición
- Sacramentos
- Doctrina de la Iglesia
- Respuestas a objeciones comunes
- Autoridad de la Iglesia
- María y los santos
- Entre otros temas apologéticos

### Estilo de Escritura

- **Didáctico**: Fácil de entender y seguir
- **Formato pregunta-respuesta**: Similar a catecismos tradicionales
- **Fundamentado**: Con referencias bíblicas, documentos de la Iglesia, y enseñanzas de los santos
- **Conciso**: Directo al punto, sin rodeos innecesarios
- **Accesible**: Para católicos de diferentes niveles de formación

---

## Flujo de Trabajo Técnico

### Herramientas

1. **Escritura**: Markdown (.md) en Obsidian o VS Code
2. **Organización**: Cada libro en una carpeta separada
3. **Conversión**: Pandoc para generar PDF/Word/EPUB
4. **Maquetación final** (opcional): Affinity Publisher

### Estructura de Archivos

```
📁 Libro-01-Fundamentos-Fe/
  ├── capitulo-01-que-es-apologetica
  ├── capitulo-02-escritura-sagrada
  ├── capitulo-03-tradicion-apostolica
  ├── capitulo-04-magisterio-iglesia
  └── capitulo-05-sintesis-fundamentos

📁 Libro-02-Sacramentos/
  └── ...
```

### Formato Markdown Usado

```markdown
# Capítulo 1: Título del Capítulo

## Introducción

Texto introductorio del capítulo...

## Pregunta 1: ¿Pregunta específica?

**Respuesta:** Respuesta concisa y clara...

**Fundamento Bíblico:**
> "Cita bíblica textual"
> — Libro capítulo:versículo

**Enseñanza de la Iglesia:**
Referencia a documentos oficiales (Catecismo, Concilios, Encíclicas, etc.)

**Profundización:**
Explicación más detallada si es necesario...

---

## Pregunta 2: ¿Siguiente pregunta?

[Mismo formato...]
```

---

## Comandos Pandoc para Conversión

### Generar PDF en formato A5

```bash
pandoc *.md -o libro-apologetica-01.pdf \
  --toc \
  --number-sections \
  -V geometry:a5paper \
  -V geometry:margin=1.5cm \
  -V documentclass=book \
  -V lang=es \
  -V fontsize=11pt
```

### Generar Word (para revisiones)

```bash
pandoc *.md -o libro-apologetica-01.docx \
  --toc \
  --number-sections
```

### Generar EPUB (versión digital)

```bash
pandoc *.md -o libro-apologetica-01.epub \
  --toc \
  --epub-cover-image=portada.jpg
```

---

## Objetivos del Proyecto

1. ✅ Crear material accesible para formación católica
2. ✅ Responder objeciones comunes contra la fe católica
3. ✅ Fundamentar respuestas en Escritura, Tradición y Magisterio
4. ✅ Formato portable y fácil de consultar (A5)
5. ✅ Serie de libros temáticos para estudio progresivo
