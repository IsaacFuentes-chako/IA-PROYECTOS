---
---
# Felicidad vs Riqueza

¿El dinero compra felicidad? Un modelo de regresión lineal simple y múltiple sobre datos de felicidad y producto interno bruto (GDP) de 141 países.

## Sobre el proyecto

Desde 2012, el *World Happiness Report* (WHR) propone una metodología para estimar el nivel de felicidad promedio de distintos países del mundo. Este proyecto explora la relación entre la felicidad reportada y el GDP de un país, evaluando primero un modelo simple, y después extendiéndolo con variables adicionales (GDP per cápita, esperanza de vida, edad mediana) para comparar el poder explicativo de cada especificación.

## Base de datos

- **Fuente (datos originales):** *World Happiness Report* 2022 (Helliwell et al., 2022).
- **Fuente (datos de extensión):** panel de indicadores por país de [Our World in Data](https://github.com/owid/covid-19-data) (2024), descargado directamente desde [`owid-covid-latest.csv`](https://raw.githubusercontent.com/owid/covid-19-data/master/public/data/latest/owid-covid-latest.csv) — a pesar del nombre del repositorio, este archivo incluye un panel general de indicadores socioeconómicos por país (no solo datos de COVID-19), del cual se tomaron las tres variables adicionales.
- **Observaciones:** 141 países (conjunto base); 140 países en el análisis extendido (Kosovo quedó fuera por falta de información en el panel de OWID).
- **Variables principales:**
  - `Felicidad` — nivel de felicidad promedio reportado en el WHR 2022 (escala aproximada de 2 a 8)
  - `GDP` — producto interno bruto total en dólares (2020)
  - `GDP per cápita` (`gdp_per_capita`) — GDP por persona, en dólares (fuente: OWID)
  - `Esperanza de vida` (`life_expectancy`) — esperanza de vida al nacer, en años (fuente: OWID)
  - `Edad mediana` (`median_age`) — edad mediana de la población de cada país (fuente: OWID)

## Contenido

- <a href="./analisis.ipynb" download>Reporte en formato ipynb</a>
- [Reporte en formato html](./analisis.html)
- <a href="./datos.csv" download>Base de datos</a>
