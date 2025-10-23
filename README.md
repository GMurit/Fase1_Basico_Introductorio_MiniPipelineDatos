# Mini Pipeline de Datos – Fase 1: Python aplicado a Datos

## Objetivo
Este proyecto tiene como objetivo construir un **pipelines básicos de datos** e **introductorio** usando Python, pandas, numpy, entre otras librerías, aplicando técnicas de limpieza, transformación y filtrado de datos.

## Estructura del directorio de carpetas

FASE_1_DATA_ENG/
├── DATA/
│ ├── RAW_DATA/ # Datos originales sin limpiar
│ └── CLEAN_DATA/ # Datos limpios y filtrados listos para análisis
├── NOTEBOOKS/ # Notebooks de prácticas y ejercicios
├── SRC/ # Código fuente opcional (scripts .py)
└── README.md # Este archivo

## Archivos generados

### RAW_DATA
Datos originales sin limpieza.

### CLEAN_DATA
Datos limpios o trasformados.

## Herramientas utilizadas
- **Python** 3
- **Pandas** y **NumPy**
- **Matplotlib / Seaborn** (no se realizó por ser un proceso opcional)
- **JupyterLab** (para la realización de toda la práctica)
- **requests** Para obtener datos de internet.
- **logging** Para manejor de información.
- **PyArrow** (para Parquet)
- **Git**

## Notas
- Se mantuvo una copia de los datos raw para asegurar la reproducibilidad.  
- Los archivos filtrados y limpios se encuentran en `CLEAN_DATA`.  
- Este proyecto sirve como primer mini-pipeline de datos práctico, listo para ampliar con pipelines ETL más complejos y conectividad con bases de datos.

## Notebook 01: Basico y manipulación de datos
- Conceptos de listas, diccionarios, sets y tuplas
- Creación de DataFrames
- Filtrado y agrupación
- Guardado en CSV/Parquet
- [Link al notebook](NOTEBOOKS/01_basico_ejercicio.ipynb)

## Notebook 02: Datos desde internet + logging
- Descarga de datasets desde URL
- Manejo de errores y logging
- Limpieza y columnas derivadas
- Guardado en CSV/Parquet
- [Link al notebook](NOTEBOOKS/02_basico_ejercicio_api_logging.ipynb)

## Notebook 03: Filtrado, agrupación y visualización
- Filtrado de países y casos
- Agrupación y cálculo de métricas
- Visualizaciones con Matplotlib y Seaborn
- Guardado de resultados filtrados
- [Link al notebook](NOTEBOOKS/03_filtrado_agrupado_visualización_datos_covid.ipynb)

## Notebook 04: Repaso Python + Mini-pipeline de ventas

- Creación de DataFrame desde lista de diccionarios
- Limpieza de datos (dropna, reset_index)
- Columnas derivadas (total)
- Filtrado y agrupación por producto (groupby, agg)
- Visualización de totales por producto (gráfico de barras con Matplotlib/Seaborn)
- Guardado de resultados en CSV/Parquet en CLEAN_DATA
- Propósito: repaso de conceptos de Python aplicados a datos, consolidación de pipeline básico y comprobación de resultados.
- [Link al notebook](NOTEBOOKS/04_repaso01.ipynb)

## Notebook 05: Extracción de datos desde API
- Conexión a la API de CoinGecko usando requests
- Conversión de datos JSON a DataFrame
- Creación de columnas derivadas (precio en EUR)
- Filtrado por capitalización de mercado
- Agregación de datos con groupby y cálculo de precio medio
- Guardado de resultados en CSV y Parquet
- Link al notebook: [05_repaso_api.ipynb](NOTEBOOKS/05_repaso_api.ipynb)
