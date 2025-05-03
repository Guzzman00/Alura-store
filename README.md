# README

📊 **Proyecto Análisis de Tiendas Alura | Challenge Alura Latam**

Un análisis exploratorio de datos y visualización interactiva desarrollado como parte del Challenge de Data Science de Alura Latam. Permite comprender el rendimiento de cuatro tiendas ficticias (Tienda 1, Tienda 2, Tienda 3, Tienda 4) a través de diversas métricas de ventas y satisfacción.

👥 **Autor**

* **nombre:** Felipe Guillermo Guzmán De La Fuente
* **mail:** guzzman00@hotmail.com
* **GitHub:** Guzzman00

📋 **Descripción del Proyecto**

Este proyecto, contenido en un notebook de Jupyter (`AluraStoreLatam.ipynb`), realiza un análisis detallado de datos de ventas simulados para cuatro tiendas. El objetivo es extraer insights sobre:
* Rendimiento financiero (Ingresos).
* Popularidad de categorías y productos específicos.
* Nivel de satisfacción del cliente (Calificaciones).
* Costos operativos (Envíos).
* Patrones geográficos de ventas.
* Finalmente, sintetiza los hallazgos para ofrecer una recomendación estratégica.

⚙️ **Características Técnicas del Análisis**

* Carga y combinación de datos desde múltiples fuentes (CSV).
* Limpieza y preprocesamiento de datos (conversión de tipos, manejo de nulos).
* Cálculo de métricas agregadas (sumas, promedios, conteos).
* Análisis de rankings (Top/Bottom).
* Visualización de datos estática con Matplotlib (gráficos de barras).
* Visualización de datos geoespaciales con Folium (Heatmaps sobre mapa de Colombia).
* Análisis cualitativo y cuantitativo integrado.
* Informe final estructurado con recomendaciones basadas en datos.

🛠️ **Tecnologías Utilizadas**

* Python 3
* Pandas (Manipulación y análisis de datos)
* Matplotlib (Visualización de datos estática)
* NumPy (Cálculos numéricos)
* Folium (Visualización de datos geoespaciales interactiva)
* IPython.display (Para mostrar mapas Folium en el notebook)
* Jupyter Notebook / Google Colab (Entorno de desarrollo)

✅ **Requisitos del Challenge Cumplidos**

Este proyecto cumple con todos los requisitos de análisis solicitados en el challenge:
* **1. Análisis de facturación:** Se calculó y visualizó el ingreso total por tienda sumando la columna 'Precio'.
* **2. Ventas por categoría:** Se agruparon los datos por categoría y se contaron las ventas por tipo en cada tienda, mostrando las más populares.
* **3. Calificación promedio:** Se calculó y visualizó la calificación promedio de clientes por tienda para medir satisfacción.
* **4. Productos más y menos vendidos:** Se identificaron y visualizaron los 5 productos con más ventas y los 5 con menos ventas en cada tienda.
* **5. Envío promedio:** Se calculó y visualizó el costo de envío promedio para cada tienda.
* **6. Análisis Geográfico (Extra):** Se realizó la exploración opcional de datos de latitud/longitud, generando scatter plots y heatmaps para analizar patrones geográficos de ventas y su posible influencia.
*  **7. Informe Final:** Síntesis de análisis y recomendación justificada de tienda a vender.

🔍 **Estructura del Proyecto (Notebook)**

El notebook `AluraStoreLatam.ipynb` está organizado en las siguientes secciones principales:
* Importación de datos (carga de CSVs desde URLs)
* 1. Análisis de facturación (Ingresos por tienda)
* 2. Ventas por categoría (Conteos y gráficos por tienda)
* 3. Calificación promedio de la tienda (Cálculo y gráfico)
* 4. Productos más y menos vendidos (Identificación Top/Anti Top 5 y gráficos)
* 5. Envío promedio por tienda (Cálculo y gráfico)
* 6. ¡Extra! Análisis del desempeño geográfico (Limpieza de coordenadas, Scatter plots, Heatmaps Folium, Análisis de influencia)
* 7. Informe Final (Síntesis y recomendación)

📦 **Guía de Instalación y Ejecución**

1.  **Entorno:** Este notebook de Jupyter (`AluraStoreLatam.ipynb`) está diseñado para ejecutarse en Google Colab.
2.  **Librerías:** Las librerías principales (`pandas`, `matplotlib`, `numpy`, `ipython`) suelen estar preinstaladas en Colab. `Folium` también suele estarlo, pero si encuentras un error de importación para `folium`, ejecuta `!pip install folium` en una celda de código al inicio del notebook.
3.  **Abrir Notebook:** Sube o abre el archivo `AluraStoreLatam.ipynb` en Google Colab.
4.  **Ejecutar Celdas:** Ejecuta las celdas de código en orden secuencial (de arriba abajo, usando Shift+Enter o el botón de Play). Es **crucial** ejecutar la primera celda de importación de datos para que las variables `tienda1`, `tienda2`, etc., estén definidas. Ejecuta también la celda de preparación de `df_geo` antes de los análisis geográficos.

💻 **Cómo Utilizar**

* Ejecuta todas las celdas del notebook desde la primera hasta la última en ese orden para replicar el análisis completo.
* Observa las salidas de cada celda: tablas de datos, gráficos y textos de análisis.
* Interactúa con los mapas de Folium (zoom, paneo) para explorar la distribución geográfica.
* Lee el informe final para entender la inclinación de venta basada en los datos.
* Puedes modificar parámetros en el código (ej. colores de gráficos, parámetros de heatmap, número de productos en Top/Anti Top) y re-ejecutar para explorar variaciones.

📺 **Vista**

* Las visualizaciones generadas (gráficos de barras, mapas de calor) se muestran directamente en las celdas de salida del notebook `AluraStoreLatam.ipynb` después de ejecutar el código correspondiente.

![Análisis de Facturación](1.%20An%C3%A1lisis%20de%20facturaci%C3%B3n.png)
