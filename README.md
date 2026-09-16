# FinZen — Documentación del Proyecto Parcial

Repositorio de **documentación y evidencia** del proyecto **FinZen** (aplicación de
finanzas personales con asistente de IA), elaborado para el curso **Cloud Computing
(MCD8007)** de la Escuela de Posgrado de la **Universidad de Ingeniería y Tecnología
(UTEC)** — CDIA V5.

Reúne el informe LaTeX, los diagramas, las capturas de evidencia, la colección de
Postman, el catálogo de APIs y el material del prototipo.

## Contenido

| Ruta | Descripción |
|---|---|
| `Proyecto_Parcial.tex` | Informe fuente (LaTeX). |
| `Proyecto_Parcial.pdf` | Informe compilado (38 páginas). |
| `figures/` | Imágenes: logo UTEC, diagramas y capturas de evidencia. |
| `figures/capturas_postman/` | Evidencia de las peticiones a la API (Postman/Newman). |
| `figures/capturas_frontend/` | Evidencia del frontend (dashboard, gastos, asistente). |
| `figures/capturas_aws/` | Evidencia del despliegue en AWS (EC2, Security Group, contenedores, app). |
| `figures/capturas_openai/` | Creación y configuración de la clave de OpenAI. |
| `postman/` | Colección de Postman, entornos y evidencia de las peticiones. |
| `CATALOGO_DE_APIS.md` | Catálogo completo de los endpoints. |
| `frontend-prompt/` | Prompt y mockup del prototipo del frontend. |
| `diagram-sources/` | Fuentes editables de los diagramas (draw.io, Excalidraw) y el esquema de base de datos (`schema.dbml`). |

## Compilación

Requiere una distribución de TeX (TeX Live o MacTeX). El documento se compila con
`pdflatex`:

```bash
pdflatex Proyecto_Parcial.tex
pdflatex Proyecto_Parcial.tex   # segunda pasada para el índice
```

Las imágenes se resuelven desde `figures/` mediante `\graphicspath`.

## Puesta en marcha (resumen)

El proyecto se compone de **tres repositorios**. Para ejecutarlo de extremo a extremo:

1. **Backend** ([finzen-app](https://github.com/UTEC-AII/finzen-app)): clonar, configurar
   el archivo `.env` y levantar los microservicios con `docker compose up -d --build`.
2. **Frontend** ([finzen-webui](https://github.com/UTEC-AII/finzen-webui)): clonar,
   construir la imagen y ejecutarla conectada a la red del backend.
3. **Abrir** la aplicación en `http://localhost` (servida por Nginx).

Cada repositorio incluye su guía detallada:

| Repositorio | Guía local | Guía AWS |
|---|---|---|
| Backend | [Inicio rápido](https://github.com/UTEC-AII/finzen-app#inicio-rápido-local-con-docker) | [Despliegue en AWS](https://github.com/UTEC-AII/finzen-app#despliegue-en-aws-ec2) |
| Frontend | [Ejecutar con Docker](https://github.com/UTEC-AII/finzen-webui#ejecutar-con-docker) | [Despliegue en AWS](https://github.com/UTEC-AII/finzen-webui#despliegue-en-aws-ec2) |

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
