# Curso de mecánica de motos — Guía de repaso

Web: **https://santimaestri.github.io/curso-moto/**

Resumen por tema de las 29 clases del curso, con datos clave y preguntas para chequearse. No incluye videos ni transcripciones.

## Cómo actualizarla

Todo el contenido está en `docs/`, en Markdown: un archivo por bloque en `docs/bloques/`, la portada en `docs/index.md` y el plan en `docs/plan.md`. Cada vez que se sube un cambio a `main`, GitHub Actions reconstruye y publica la web sola, en uno o dos minutos.

Tres formas de cambiar algo:

1. **Desde GitHub:** abrí el archivo, tocá el lápiz, editá y apretá *Commit changes*. Cada página de la web tiene un lápiz arriba a la derecha que lleva directo a editarla.
2. **Desde la compu:** `git pull`, editá los `.md`, `git commit` y `git push`.
3. **Con Claude:** pedile, por ejemplo, "agregá a la web del curso de motos lo de la clase 30".

### Agregar una clase o un bloque nuevo

1. Si es un tema nuevo, creá `docs/bloques/15-tema.md` con la misma estructura: *Qué se vio*, *Datos que hay que saber* y *Preguntas para chequearte*.
2. Sumalo al `nav` de `mkdocs.yml`.
3. Agregá la fila de la clase en la tabla de `docs/index.md`.

### Probarla en la compu antes de subir

```bash
pip install -r requirements.txt
mkdocs serve
```

y abrí http://127.0.0.1:8000.
