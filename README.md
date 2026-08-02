# Métricas de evaluación para traducción automática qom $\leftrightarrow$ español

[![Trabajo final (PDF)](https://img.shields.io/badge/Trabajo_final-PDF-b31b1b?logo=adobeacrobatreader&logoColor=white)](https://macfernandez.github.io/poster-evaluation-metrics-for-qom-esp-mt/poster.pdf)
[![Build poster PDF](https://img.shields.io/github/actions/workflow/status/macfernandez/poster-evaluation-metrics-for-qom-esp-mt/build-poster.yml?branch=main&label=build%20poster&logo=githubactions&logoColor=white)](https://github.com/macfernandez/poster-evaluation-metrics-for-qom-esp-mt/actions/workflows/build-poster.yml)
![Python](https://img.shields.io/badge/python-3.13-blue?logo=python&logoColor=white)

> **Título:** Métricas de evaluación para traducción automática qom ↔ español. _Baselines_, limitaciones y unahoja de ruta
>
> **Autora:** Macarena Fernández Urquiza
>
> **Supervisoras:** Viviana Cotik y Paola Cúneo
>
> **Póster compilado**: https://macfernandez.github.io/poster-evaluation-metric/
>
> **Bibliografía**: https://www.zotero.org/groups/6623490/nd-school-nlp-qom-mt-eval/library


## Estructura del repositorio

```
├── data/                 # datos (no inluidos en este repo)*
├── models/               # modelos (no inluidos en este repo)*
├── notebooks/            # flujo de trabajo paso a paso (01 … 06)
│   ├── 00-….ipynb        # traducciones para test de qom-mt-v1-estrat
│   ├── 01-….ipynb        # checkeo de evaluación de modelos, IC y permutación
│   └── 02-….ipynb        # comparación con juicios humanos
└── poster                # póster en LaTeX, gráficos y bibliografía
```

\* Al momento de presentar este póster, los datos y modelos se encuentran alojados en un
repositorio privado de [HugginFace](https://huggingface.co/). Las _notebooks_ contenidas
en este proyecto permiten realizar la descarga siempre que se cuente con un token que permita
el acceso a dicho repositorio. El mismo debe almacenarse en un archivo `.env` en la raíz del
proyecto y con el nombre `HF_TOKEN`.

```
# En archivo .env
HF_TOKEN=...
```

## Reproducción del flujo de trabajo

Crear un entorno con Python 3.13 (por ejemplo con [`uv`](https://docs.astral.sh/uv/)).

```bash
uv sync
```

Ejecutar las _notebooks_ en orden (`00`, `01`, `02`, `03`).
