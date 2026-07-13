# poster-evalution-metrics-for-qom-esp-mt

Póster para presentar en la [segunda edición de la Escuela de NLP de Sudamérica](https://south-american-nlp-school.dc.uba.ar/).

**Título:** Métricas de evaluación para traducción automática qom ↔ español: líneas de base, limitaciones y una hoja de ruta
**Autora:** Macarena Fernández Urquiza — Directora: Viviana Cotik — Codirectora: Paola Cúneo

## Archivos

```
poster.tex        # póster (beamerposter, estilo bloques, en español) — DRAFT con placeholders
figures/          # logos (uba.eps, master.eps)
```

## Cómo compilar

- **Overleaf:** subí la carpeta, abrí `poster.tex` y en *Menu → Compiler* elegí **pdfLaTeX**.
- **Local:** `pdflatex poster.tex` (dos corridas).

El póster es A0 vertical. Está basado en `beamerposter` con bloques al estilo del
template de TU Dublin, adaptado al español.

## Estado: DRAFT

El contenido está marcado con placeholders en gris y cursiva (texto entre corchetes,
p. ej. *[acá va la tabla de BLEU/ChrF++]*). Cada bloque indica qué información va.
Reemplazá los placeholders por el contenido real a medida que esté disponible.

Los logos están como cajas placeholder. Para activarlos, convertí los `.eps` a
`.pdf`/`.png` y descomentá las líneas `\includegraphics` en el encabezado (pdfLaTeX
no incluye `.eps` directamente).
