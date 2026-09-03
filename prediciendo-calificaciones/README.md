---
---
# Prediciendo Calificaciones

Selección de características y regresión lineal múltiple aplicada a la predicción del desempeño académico de estudiantes.

## Sobre el proyecto

Este proyecto construye un modelo de regresión lineal múltiple que predice la calificación final (`G3`) de un estudiante a partir de variables demográficas y académicas. Incluye limpieza de datos, revisión de valores atípicos, análisis de colinealidad, y comparación de métodos de selección de características (selección hacia adelante y búsqueda exhaustiva) validados sobre conjuntos independientes de entrenamiento, validación y prueba.

## Base de datos

- **Fuente:** subconjunto de 10 variables del dataset público *Student Performance* (Cortez & Silva, 2008), disponible en el [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/320/student+performance). El análisis también contrasta este subconjunto contra el [dataset original de 33 variables](https://archive.ics.uci.edu/dataset/320/student+performance) para verificar si un par de registros idénticos en las 10 columnas reducidas correspondían al mismo estudiante o a estudiantes distintos.
- **Observaciones:** 395 estudiantes.
- **Variables (10):**
  - `Escuela` — escuela del estudiante (GP / MS)
  - `Sexo` — F / M
  - `Edad` — en años (15 a 22)
  - `Internet` — acceso a internet en casa (yes/no)
  - `HorasDeEstudio`, `Reprobadas`, `Faltas` — variables académicas
  - `G1`, `G2`, `G3` — calificaciones de primer periodo, segundo periodo, y final (0 a 20)

## Contenido

- [Reporte en formato ipynb](./analisis.ipynb)
- [Reporte en formato html](./analisis.html)
- [Base de datos](./datos.csv)
