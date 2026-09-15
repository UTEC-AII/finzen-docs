# FinZen — Documento LaTeX del Proyecto Parcial

Informe técnico del proyecto **FinZen** (aplicación de finanzas personales con
asistente de IA), elaborado para el curso **Cloud Computing (MCD8007)** de la Escuela
de Posgrado de la **Universidad de Ingeniería y Tecnología (UTEC)** — CDIA V5.

Este repositorio contiene únicamente el **documento LaTeX** del proyecto y sus
recursos gráficos.

## Contenido

| Ruta | Descripción |
|---|---|
| `Proyecto_Parcial.tex` | Documento fuente (LaTeX). |
| `Proyecto_Parcial.pdf` | Documento compilado (34 páginas). |
| `figures/` | Imágenes: logo UTEC, diagramas y capturas de evidencia. |
| `figures/capturas_postman/` | Evidencia de las peticiones a la API (Postman). |
| `figures/capturas_frontend/` | Evidencia del frontend (dashboard, gastos, asistente). |
| `diagram-sources/` | Fuentes editables de los diagramas (draw.io, Excalidraw) y el esquema de base de datos (`schema.dbml`). |

## Compilación

Requiere una distribución de TeX (TeX Live o MacTeX). El documento se compila con
`pdflatex`:

```bash
pdflatex Proyecto_Parcial.tex
pdflatex Proyecto_Parcial.tex   # segunda pasada para el índice
```

Las imágenes se resuelven desde `figures/` mediante `\graphicspath`.

## Repositorios relacionados

- Backend: <https://github.com/UTEC-AII/finzen-app>
- Frontend: <https://github.com/UTEC-AII/finzen-webui>

## Autores

- Sebastian Rodrigo García Villacorta
- Dante Guillermo Barreto Daza
- Clinton Michael Chulluncuy Reynoso
- Ronald Ramiro Hilario Orihuela

**Docente:** Mejia Fernandez, Oscar Rodolfo

## Licencia

MIT (ver `LICENSE`).
