---
---
# Acceso a educación superior en los municipios de Oaxaca

## Sobre el proyecto

Este proyecto estudia la desigualdad en la continuidad educativa entre los 570 municipios de Oaxaca:
qué porcentaje de la población de 18 a 24 años sigue asistiendo a la escuela (un proxy de acceso y
continuidad a la educación superior) y con qué factores se asocia esa continuidad. Une tres fuentes
oficiales de datos, prepara y explora la información, selecciona un conjunto de predictores, construye
y compara un modelo lineal (regresión OLS) y uno no lineal (KNN), evalúa su desempeño sobre municipios
que ninguno de los dos modelos vio durante su construcción, y cierra con un análisis de inferencia
sobre los factores que más se asocian con la continuidad educativa: marginación social, intensidad
migratoria, composición étnica y aislamiento geográfico.

El modelo final (regresión lineal, elegido por interpretabilidad frente a un desempeño casi idéntico
al de KNN) alcanza un R² de 0.66 sobre municipios de prueba nunca vistos, con un error típico de
predicción de alrededor de 8 puntos porcentuales. El hallazgo más fuerte es que la falta de educación
básica completa en adultos es, por un margen amplio, el predictor más asociado con la baja continuidad
educativa de los jóvenes del municipio; la intensidad migratoria hacia Estados Unidos también se asocia
negativamente, en línea con lo reportado por McKenzie y Rapoport (2011) para México rural.

## Base de datos

El análisis une tres fuentes públicas oficiales a nivel municipio:

| Fuente | Qué aporta |
|---|---|
| [INEGI — Censo de Población y Vivienda 2020 (ITER)](https://www.inegi.org.mx/programas/ccpv/2020/) | Variable de interés: asistencia escolar de 18 a 24 años |
| [CONEVAL — Índice de Rezago Social 2020](https://www.coneval.org.mx/Medicion/IRS/Paginas/Indice_Rezago_Social_2020.aspx) | 11 indicadores desagregados de rezago social (vivienda, servicios, educación básica) |
| [CONAPO — Índice de Intensidad Migratoria 2020](https://www.gob.mx/conapo/documentos/indices-de-intensidad-migratoria-mexico-estados-unidos-2020) | Índice de intensidad migratoria hacia Estados Unidos |

El archivo `datos.csv` de este repositorio **no es ninguna de las tres fuentes originales**: es el
conjunto de datos ya unido, limpio y con las 13 variables finalmente seleccionadas (570 municipios ×
16 columnas), tal como queda al terminar la sección de selección de características del notebook.
Se comparte así para que el análisis sea reproducible sin necesidad de descargar y procesar las tres
fuentes desde cero; todo el proceso de unión, limpieza y preparación de los datos originales está
documentado paso a paso dentro del notebook.

## Contenido

- <a href="./analisis.ipynb" download>Notebook completo (.ipynb)</a>
- [Reporte en formato html](./analisis.html)
- <a href="./datos.csv" download>Datos ya preparados (.csv)</a>
