# TrabajoFinal_FrancoOrtega
Trabajo Final DMC
# Diagnóstico Comercial y Desaceleración en Ventas del Sector Automotriz (2024 - 2026)

## 📌 Descripción del Proyecto
Este proyecto desarrolla un análisis exploratorio de datos (EDA), visualizaciones interactivas y consultas analíticas estructuradas en SQL sobre un dataset consolidado de 450 transacciones comerciales del sector automotriz. El estudio evalúa el comportamiento de las ventas, la evolución de los precios, la presión de los descuentos comerciales, la penetración de seguros vehiculares y la colocación de financiamiento a lo largo del periodo 2024–2026.

---

## 📊 Descripción del Dataset
* **Tamaño:** 450 filas y 12 columnas.
* **Periodo temporal:** 2024 a 2026.
* **Variables principales:**
  * `id`: Identificador único de transacción.
  * `marca` / `modelo`: Clasificación vehicular (Toyota, Hyundai, Kia).
  * `Año`: Año comercial de la operación.
  * `tipo_vehiculo`: Segmentación de uso (Particular, Taxi, Negocio).
  * `tienda`: Sede regional de venta (Lima, Arequipa, Chiclayo, Huancayo).
  * `precio` / `descuento` / `precio_final`: Estructura de precios y margen comercial en USD.
  * `Seguro`: Indicador de contratación de póliza vehicular (Sí / No).
  * `Monto_financiado`: Capital financiado otorgado al cliente en USD.

---

## 🎯 Objetivo del Análisis
Identificar, cuantificar y diagnosticar las causas de la contracción comercial que experimenta el negocio automotriz entre 2024 y 2026, analizando la efectividad de las promociones (descuentos), la colocación de productos de valor agregado (seguros) y la evolución del crédito automotriz por sede regional.

---

## 📂 Fuente del Dataset
* **Tipo de Fuente:** Dataset Propio (Registro de transacciones comerciales del sector automotriz).
* **Enlace:** No aplica link a Kaggle al tratarse de un conjunto de datos propio estructurado para fines académicos y analíticos.

---

## 🛠️ Principales Etapas Realizadas
1. **Carga y Configuración:** Lectura del archivo Excel estructurado mediante Pandas e importación de librerías analíticas.
2. **Exploración Inicial (EDA) y Calidad de Datos:** Verificación de dimensiones, tipos de datos, control de nulos y duplicados, e ingeniería de variables (`cuota_inicial`, `% financiamiento LTV` y `% descuento`).
3. **Estadística Descriptiva:** Métricas de tendencia central y dispersión para variables numéricas, frecuencias de variables categóricas y comparativo interanual (2024 vs 2025 vs 2026).
4. **Visualizaciones con Plotly:** Gráficos interactivos de líneas (tendencia temporal), barras agrupadas por sede regional, boxplots de precios por marca, gráfico de dona para seguros y scatter plot de dispersión financiera.
5. **Consultas SQL con DuckDB:** Ejecución de 5 consultas analíticas sobre DataFrames aplicando `SELECT`, `LIMIT`, `WHERE`, `GROUP BY`, `ORDER BY`, `HAVING` y lógica condicional con `CASE WHEN`.
6. **Hallazgos y Conclusiones:** Diagnóstico cuantitativo sobre la caída del -33.3% en unidades vendidas, el impacto del sobre-descuento en 2025 y la reducción en montos de colocación crediticia en 2026.

---

## 💻 Tecnologías Utilizadas
* **Lenguaje:** Python 3.10+
* **Manipulación de Datos:** Pandas, NumPy
* **Motor SQL en Memoria:** DuckDB
* **Visualización Interactiva:** Plotly Express / Plotly Graph Objects
* **Entornos de Desarrollo:** Google Colab / Jupyter Notebook
* **Control de Versiones y Alojamiento:** Git y GitHub

---

## 🚀 Instrucciones para Abrir o Ejecutar el Notebook

### Opción 1: En Google Colab (Recomendada)
1. Ingresa a [Google Colab](https://colab.research.google.com/).
2. Haz clic en **Archivo** > **Subir notebook** y selecciona `notebook_analisis_sql_python.ipynb`.
3. Sube el archivo Excel `DATASET_AUTOMOTRIZ_450_REGISTROS_2024_2026.xlsx` al panel lateral izquierdo de archivos en Colab.
4. Ejecuta las celdas secuencialmente presionando `Shift + Enter` o desde **Entorno de ejecución** > **Ejecutar todas**.


