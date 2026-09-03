---
---
# Felicidad vs Riqueza

¿El dinero compra felicidad? Un modelo de regresión lineal simple y múltiple sobre datos de felicidad y producto interno bruto (GDP) de 141 países.

## Sobre el proyecto

Desde 2012, el *World Happiness Report* (WHR) propone una metodología para estimar el nivel de felicidad promedio de distintos países del mundo. Este proyecto explora la relación entre la felicidad reportada y el GDP de un país, evaluando primero un modelo simple, y después extendiéndolo con variables adicionales (GDP per cápita, esperanza de vida, edad mediana) para comparar el poder explicativo de cada especificación.

## Base de datos

- **Fuente:** *World Happiness Report* 2022 (Helliwell et al., 2022), complementado con datos de GDP, esperanza de vida y edad mediana por país.
- **Observaciones:** 141 países (conjunto base); 140 países en el análisis extendido.
- **Variables principales:**
  - `Felicidad` — nivel de felicidad promedio reportado en el WHR 2022 (escala aproximada de 2 a 8)
  - `GDP` — producto interno bruto total en dólares (2020)
  - `GDP per cápita`, `Esperanza de vida`, `Edad mediana` — variables adicionales usadas en el modelo extendido

## Contenido

- [Reporte en formato ipynb](./analisis.ipynb)
- [Reporte en formato html](./analisis.html)
- [Base de datos](./datos.csv)
