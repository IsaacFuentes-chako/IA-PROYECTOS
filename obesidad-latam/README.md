---
---
# Obesidad en Latinoamérica

Análisis exploratorio e inferencial de los niveles de obesidad en Colombia, Perú y México, a partir de datos de hábitos alimenticios y condición física.

## Sobre el proyecto

Los niveles de obesidad representan un problema de salud pública de gran relevancia en América Latina. Este proyecto explora un conjunto de datos con información de individuos de Colombia, Perú y México, buscando identificar patrones asociados a distintos niveles de obesidad (clasificados a partir del índice de masa corporal), y reflexiona sobre las limitaciones del diseño del estudio original.

## Base de datos

- **Fuente:** versión simplificada de la base de datos del [UCI Machine Learning Repository — Estimation of Obesity Levels Based On Eating Habits and Physical Condition](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition), recopilada originalmente por investigadores de la Universidad de la Costa (Colombia).
- **Observaciones:** 2,111 individuos.
- **Variables (10):**
  - `Sexo` — femenino (Female) o masculino (Male)
  - `Edad` — en años (14 a 61)
  - `Estatura` — en metros
  - `Peso` — en kilogramos
  - `FamiliarConSobrepeso` — antecedentes familiares de sobrepeso (yes/no)
  - `ComeMuchasCalorias` — consumo frecuente de comida alta en calorías (yes/no)
  - `ComeVegetales` — frecuencia de consumo de vegetales (1 = nunca, 2 = a veces, 3 = siempre)
  - `Fumador` — fumador activo (yes/no)
  - `ConsumoDeAgua` — litros de agua al día (1 = menos de 1L, 2 = entre 1 y 2L, 3 = más de 2L)
  - `NivelDeObesidad` — categoría calculada a partir del IMC (bajo peso, normal, sobrepeso I/II, obesidad tipo I/II/III)

## Contenido

- [Reporte en formato ipynb](./analisis.ipynb)
- [Reporte en formato html](./analisis.html)
- [Base de datos](./datos.csv)
