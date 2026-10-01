# 🛒 NovaRetail+ - Análisis de Comportamiento y Correlación de Clientes

Este repositorio contiene el análisis estadístico y exploratorio realizado para el caso **NovaRetail+** (2024). El proyecto se centra en entender qué factores operativos, demográficos y de interacción están estadísticamente asociados con la generación de ingresos anuales, separando el ruido de las métricas que realmente impactan al negocio.

## 📂 Contenido del repositorio

- `notebooks/novaretail_analisis.ipynb`
  → Notebook principal que integra el flujo completo: limpieza de datos (corrección de tipos en variables demográficas), análisis exploratorio (EDA), visualización diagnóstica (heatmaps y scatterplots), y cálculo de coeficientes estadísticos.
- `datasets/novaretail_comportamiento_clientes_2024.csv`
  → Dataset base con 15,000 registros de comportamiento y métricas de consumo.

## 📘 Cómo reproducir el análisis

1. Abre el archivo `notebooks/novaretail_analisis.ipynb`[cite: 22].
2. Ejecuta las celdas en orden secuencial para replicar el pipeline de limpieza, las matrices de correlación y los cálculos estadísticos[cite: 22].
3. El notebook carga automáticamente el dataset desde la ruta `/datasets/` o su enlace público correspondiente[cite: 22].

## 🧠 Objetivo y Alcance del análisis

- **Calidad de Datos:** Identificar y limpiar inconsistencias en la base de datos para preparar el modelado matemático[cite: 22].
- **Visualización Diagnóstica:** Mapear la dispersión real de los datos para confirmar tendencias lineales y descartar patrones ocultos.
- **Evaluación Estadística Rigurosa:** Aplicación de coeficientes específicos para medir la fuerza de las relaciones (sin asumir causalidad):
  - **Pearson y Spearman:** Evaluación de linealidad y consistencia en el comportamiento de compra (ingresos vs. transacciones).
  - **Punto-Biserial:** Medición de asociación en variables binarias (estado de suscripción premium y abandono).
  - **V de Cramér:** Análisis de asociación entre dimensiones categóricas (región y dispositivo).
- **Traducción a Negocios:** Convertir coeficientes matemáticos en recomendaciones ejecutivas y accionables para los equipos de Growth y Marketing[cite: 22].
