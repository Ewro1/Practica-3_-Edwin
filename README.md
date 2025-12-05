# Practica-3_-Edwin Martínez
Práctica 3: Análisis Exploratorio y Librería de Visualización CTG

Este repositorio documenta el desarrollo completo de la Práctica 3 del diplomado, enfocada en el Análisis Exploratorio de Datos (EDA) avanzado y la Ingeniería de Software para Ciencia de Datos.

El objetivo principal fue transformar el proceso de EDA en un módulo Python reutilizable (ctg_viz), garantizando la calidad del código mediante tipado estático, documentación exhaustiva y pruebas unitarias.
Dataset: Cardiotocography (CTG)

El proyecto utiliza el conjunto de datos Cardiotocography (CTG) de Kaggle, que contiene variables predictoras para clasificar el estado de salud fetal.
Características y Desarrollo Clave

    Limpieza de Datos Rigurosa: Implementación de manejo de valores nulos (eliminación de columnas con más del 20% de nulos e imputación adecuada) y detección y tratamiento de valores atípicos (outliers) (IQR/Z-score).

    Librería Modular (ctg_viz): Estructura organizada en submódulos para funciones de preprocesamiento, categorización de variables y un amplio conjunto de gráficos avanzados.

    Visualizaciones Avanzadas: Implementación de gráficos estadísticos complejos que incluyen:

        Histogramas con línea de densidad (KDE) y personalización por grupo.

        Boxplots desagregados por clase objetivo.

        Mapas de Calor (Heatmaps) de correlación con anotaciones y selección de métodos.

    Calidad de Código: Uso de Tipado Estático (ej. def func(x: pd.DataFrame) -> pd.DataFrame), documentación con Docstrings (estilo NumPy/Google) y validación de la lógica con Pruebas Unitarias (pytest).

Estructura del Repositorio

El proyecto sigue una estructura profesional de desarrollo de librerías Python:

practica3-ctg/
├─ README.md
├─ requirements.txt
├─ data/
│   └─ CTG.csv
├─ notebooks/
│   └─ main.ipynb   # Notebook de demostración del uso de la librería y el EDA
├─ src/
│   └─ ctg_viz/
│       ├─ __init__.py
│       ├─ preprocessing.py
│       ├─ categorization.py
│       ├─ utils.py
│       └─ plots/
│           ├─ __init__.py
│           ├─ histograms.py
│           ├─ boxplots.py
│           └─ ...
└─ tests/
  
