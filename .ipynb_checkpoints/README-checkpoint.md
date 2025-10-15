# Mini Pipeline de Datos – Fase 1: Python aplicado a Datos

## Objetivo
Este proyecto tiene como objetivo construir un **pipeline básico de datos** e **introductorio** usando Python y pandas, aplicando técnicas de limpieza, transformación y filtrado de datos. Es el primer paso práctico en mi formación como **Data Engineer junior**.

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
- `df_raw.csv` → Datos originales sin limpieza.
- `df_raw.parquet` → Datos originales en formato Parquet.

### CLEAN_DATA
- `df_completo.csv` → Datos limpios, sin valores nulos y con columna derivada `valor_log`.
- `df_completo.parquet` → Mismo dataset en formato Parquet.
- `df_filtrado.csv` → Subconjunto filtrado (valor > 50).
- `df_filtrado.parquet` → Mismo subconjunto en formato Parquet.

## Pasos realizados

1. **Creación del DataFrame raw**: se cargaron los datos originales sin modificaciones.  
2. **Exploración de datos**: revisión de información general, estadísticas descriptivas y valores nulos.  
3. **Limpieza de datos**: se rellenaron valores nulos y se creó una nueva columna `valor_log` aplicando logaritmo.  
4. **Agrupación por categoría**: cálculo de métricas de interés como la media y el conteo por grupo.  
5. **Filtrado de filas**: selección de subconjuntos específicos (`valor > 50`).  
6. **Guardado de archivos**: exportación a CSV y Parquet de todos los DataFrames (`raw`, `limpio` y `filtrado`).

## Herramientas utilizadas
- **Python** 3
- **Pandas** y **NumPy**
- **Matplotlib / Seaborn** (no se realizó por ser un proceso opcional)
- **JupyterLab** (para la realización de toda la práctica)
- **PyArrow** (para Parquet)
- **Git** (control de versiones opcional)

## Notas
- Se mantuvo una copia de los datos raw para asegurar la reproducibilidad.  
- Los archivos filtrados y limpios se encuentran en `CLEAN_DATA`.  
- Este proyecto sirve como primer mini-pipeline de datos práctico, listo para ampliar con pipelines ETL más complejos y conectividad con bases de datos.