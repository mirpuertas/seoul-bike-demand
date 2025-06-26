# 🚲 Predicción de la Demanda de Bicicletas en Seúl

Este proyecto analiza patrones temporales y climáticos que afectan la **demanda de bicicletas públicas en Seúl**, utilizando modelos de regresión lineal y Lasso con **codificación cíclica de la variable horaria**. Es el trabajo final de la materia **Introducción al Aprendizaje Automático (2.º Cuatrimestre 2024)**.

## Objetivo
Predecir **en qué momentos del día y bajo qué condiciones climáticas la demanda de bicicletas es mayor**, utilizando un enfoque de regresión.

## Contenido

- `notebooks/bicicletas-en-seul.ipynb` — análisis exploratorio, ingeniería de variables y ajuste de modelos
- `docs/Presentación - Bicicletas en Seúl.pdf` — presentación expositiva del trabajo
- `data/SeoulBikeData.csv` — dataset original (licenciado bajo CC BY 4.0)

## Dataset

El dataset utilizado es [Seoul Bike Sharing Demand](https://archive.ics.uci.edu/dataset/560/seoul+bike+sharing+demand), proporcionado por el UCI Machine Learning Repository.

> **Licencia:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)  
> Este dataset permite su uso y adaptación para cualquier propósito, siempre que se otorgue el crédito adecuado a los autores originales.

## Modelos incluidos

- Regresión lineal con codificación cíclica horaria (seno/coseno)
- Regresión con transformación cúbica de la temperatura
- Lasso para selección automática de variables

## Variables destacadas
- `Hour` — transformada con funciones seno y coseno (codificación cíclica)
- `Temperature` — modelada con un término cúbico
- `Seasons`, `Holiday`, `Functioning Day` — variables categóricas/dummies
- `Rainfall`, `Solar Radiation` — variables meteorológicas continuas

## Autor
Miguel Ignacio Rodríguez Puertas · [@mirpuertas](https://github.com/mirpuertas)

## Nota sobre el desarrollo

Si bien este trabajo fue presentado en el marco de una entrega grupal, el análisis, modelado, codificación y documentación fueron realizados en su totalidad por Miguel Ignacio Rodríguez Puertas.
