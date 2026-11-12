# TA-IND-01 — Facebook en Android 16

**Estudiante:** FUERTES CALVO LANDY LORENA.

Informe de análisis de requisitos para la aplicación Facebook (Samsung, Android 16).

## Archivos

- `main.tex`: documento fuente LaTeX reproducible.
- `main.pdf`: PDF generado directamente desde `main.tex`.
- `referencias.bib`: bibliografía con estilo IEEE.
- `figuras/F1.png` … `figuras/F6.png`: seis capturas auténticas de la app, recortadas/anonimizadas.
- `hoja_SGA.tex`: hoja informativa para SGA. Su URL está pendiente.

## Compilar desde cero

Requiere TeX Live con `pdflatex`, `bibtex8`, los paquetes `babel-spanish`, `booktabs`, `longtable`, `tabularx`, `geometry`, `lmodern`, `microtype`, `graphicx`, `fancyhdr`, `hyperref` y `IEEEtran.bst`.

Desde esta carpeta:

```sh
pdflatex -interaction=nonstopmode -halt-on-error main.tex
bibtex8 main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

El PDF final contiene **7 páginas**. Para comprobar: `pdfinfo main.pdf`.

## Alcance y referencias

- La bibliografía contiene cuatro fuentes verificables: ISO/IEC/IEEE 29148:2018, ISO/IEC 25010:2023, SWEBOK v4.0 y la guía de accesibilidad de Android.
- Los valores de velocidad, tamaño táctil y frecuencia de fallos son **umbrales propuestos**, no resultados de pruebas ejecutadas.
- El apartado 2 incorpora el análisis de 5.2.4 a 5.2.8; las correcciones de autoevaluación son propuestas para revisión de la estudiante.

## Antes de la entrega

Revisar que la reflexión corresponda a la experiencia real; verificar cláusulas, capturas y clasificación de requisitos; documentar el uso de asistentes según la experiencia efectiva; y crear un repositorio público. El trabajo contiene **umbrales propuestos**, no resultados de ensayos ejecutados. No alterar fechas del historial de commits.

En la tarea del SGA se entrega **solamente una hoja PDF de una página**, NO `main.pdf`. Primero reemplazar la URL pendiente del repositorio en `hoja_SGA.tex` y compilarla (`pdflatex hoja_SGA.tex`). Verificar que la URL completa quede en una sola línea.
