# Titanic — Análisis Exploratorio de Datos

**Autores:** Bautista Lence y Tobías Motta

**Curso:** Herramientas Básicas para el Análisis de Datos

**Cohorte:** 999201625

## Objetivo

El objetivo de este proyecto es analizar los factores asociados a la supervivencia de los pasajeros del Titanic mediante técnicas de preparación, limpieza y análisis exploratorio de datos (EDA). Se busca responder tres preguntas principales: si existen diferencias en la tasa de supervivencia según la clase del pasajero; si la edad se relaciona con la probabilidad de supervivencia; y si viajar solo o acompañado, junto con el nivel de tarifa, presenta diferencias en dicha probabilidad.

## Dataset

Se utilizó el dataset **Titanic**, compuesto por información demográfica, socioeconómica y de viaje de los pasajeros. El archivo utilizado contiene **891 registros y 15 variables**. La estructura corresponde al dataset Titanic disponible en Seaborn.
**Fuente:** [Seaborn – Titanic Dataset](https://github.com/mwaskom/seaborn-data/blob/master/titanic.csv)

* [CSV fuente del proyecto](./titanic.csv)
* [Notebook de análisis](./TITANIC_TP.ipynb)
* [Notebook en Nbviewer](https://nbviewer.org/github/USUARIO/REPOSITORIO/blob/main/TITANIC_TP.ipynb)
* Power BI: (https://github.com/tobiasmottabittencourt/CursoHerramientasBasicas999201625-LenceMotta-BautistaTobias/blob/main/Dashboard/Graficos%20y%20KPI%20Titanic.pbix)

## Pasos realizados

1. **Carga y exploración inicial:** importación del CSV mediante Pandas y revisión de dimensiones, tipos de datos, estadísticas descriptivas y valores nulos.
2. **Limpieza:** imputación de valores faltantes en `age`, `embarked` y `embark_town`; eliminación de `deck`, `sex` y `alive` por redundancia o elevada cantidad de datos faltantes.
3. **Estandarización:** conversión de `age` a entero y redondeo de `fare` a un decimal.
4. **Control de duplicados:** identificación y eliminación de registros duplicados.
5. **EDA:** análisis de supervivencia por clase, grupos etarios y combinación entre condición de viaje y clase.
6. **Visualización:** utilización de Matplotlib, Seaborn y Plotly para comunicar los principales hallazgos. La documentación oficial de Seaborn respalda el uso de visualizaciones categóricas para analizar este tipo de variables. [Seaborn – Categorical Data](https://seaborn.pydata.org/tutorial/categorical.html)

## Conclusiones

El análisis realizado muestra diferencias en la supervivencia según la clase del pasajero, con mejores resultados para primera clase. También se observan diferencias entre grupos de edad y entre pasajeros que viajaban solos o acompañados, especialmente al considerar la clase y la tarifa abonada. Los resultados permiten identificar patrones relevantes del dataset y constituyen una base para posteriores análisis predictivos.

**Nota:** Las visualizaciones incluidas fueron generadas a partir de los datos del proyecto; no se utilizaron imágenes externas.
