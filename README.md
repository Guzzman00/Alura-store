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

🎨 Vista Previa

1. Análisis de facturación

Objetivo:En este primer análisis, debes calcular el ingreso total de cada tienda. Sumando los valores de la columna Precio de cada conjunto de datos de la tienda para estimar los ingresos.

![1. Análisis de facturación](1.%20An%C3%A1lisis%20de%20facturaci%C3%B3n.png)

Notas del Análisis de facturación:

-Ingresos Totales:

La facturación combinada de las cuatro tiendas asciende aproximadamente a $4,403 Millones de dolares (suma de USD 1,151M + USD 1,116M + USD 1,098M + USD 1,038M)

-Ranking por Tienda basado en ingreso generado:

1°)Tienda 1: Lidera con aprox. USD 1,151M

2°)Tienda 2: Sigue con aprox. USD 1,116M

3°)Tienda 3: Ocupa el tercer lugar con aprox. USD 1,098M

4°)Tienda 4: Registra los menores ingresos con aprox. USD 1,038M

-Diferencias Notables:

Aunque todas las tiendas superan los USD 1 Millón en ingresos, la diferencia entre la tienda de mayor rendimiento, la Tienda 1 y la de menor rendimiento, la Tienda 4 es significativa, alcanzando aproximadamente USD 113 Millones. Las Tiendas 2 y 3 presentan ingresos bastante similares entre sí

2. Ventas por categoría

Objetivo:En este debes calcular la cantidad de productos vendidos por categoría en cada tienda. La idea es agrupar los datos por categoría y contar el número de ventas de cada tipo, mostrando las categorías más populares de cada tienda.

--- Conteo Categorías Tienda 1 --- 
 Categoría del Producto
Muebles                    465
Electrónicos               448
Juguetes                   324
Electrodomésticos          312
Deportes y diversión       284
Instrumentos musicales     182
Libros                     173
Artículos para el hogar    171

--- Conteo Categorías Tienda 2 --- 
 Categoría del Producto
Muebles                    442
Electrónicos               422
Juguetes                   313
Electrodomésticos          305
Deportes y diversión       275
Instrumentos musicales     224
Libros                     197
Artículos para el hogar    181

--- Conteo Categorías Tienda 3 --- 
 Categoría del Producto
Muebles                    499
Electrónicos               451
Juguetes                   315
Electrodomésticos          278
Deportes y diversión       277
Libros                     185
Instrumentos musicales     177
Artículos para el hogar    177

--- Conteo Categorías Tienda 4 --- 
 Categoría del Producto
Muebles                    480
Electrónicos               451
Juguetes                   338
Deportes y diversión       277
Electrodomésticos          254
Artículos para el hogar    201
Libros                     187
Instrumentos musicales     170

![2-1. Ventas por categoría](2-1.%20Ventas%20por%20categoría.png)

![2-2. Ventas por categoría](2-2.%20Ventas%20por%20categoría.png)

![2-3. Ventas por categoría](2-3.%20Ventas%20por%20categoría.png)

![2-4. Ventas por categoría](2-4.%20Ventas%20por%20categoría.png)

Notas de las Ventas por categoría:

-Ventas Totales:

El número total de ventas acumuladas en las cuatro tiendas, sumando todas las categorías, es de 9,435 unidades

-Ranking por Categoría basado en las ventas generadas:

1°) Muebles: Lidera con un total de 1,886 ventas

2°) Electrónicos: Sigue con 1,772 ventas

3°) Juguetes: Ocupa el tercer lugar con 1,290 ventas

4°) Electrodomésticos: Registra 1,149 ventas

5°) Deportes y diversión: Suma 1,113 ventas

6°) Instrumentos musicales: Alcanza 753 ventas

7°) Libros: Llega a 742 ventas

8°) Artículos para el hogar: Cierra la lista con 730 ventas

-Diferencias Notables:

Las categorías "Muebles", "Electrónicos" y "Juguetes" son consistentemente las más populares en términos de números de ventas en las cuatro tiendas, ocupando los tres primeros lugares respectivamente en todas ellas. El patrón de igualdad de los puestos se rompe a causa de la Tienda 4, ya que en el cuarto lugar en ventas es la única tienda que no tiene "Electrodomésticos" sino "Deportes y diversión", en consecuencia la Tienda 4 es también la única tienda que tiene en el quinto lugar en ventas "Electrodomésticos" en vez de "Deportes y diversión". Para el sexto lugar en ventas las tiendas 1 y 2 tienen la categoría de "Instrumentos musicales", mientras que en las tiendas 3 y 4 tienen "Libros" y "Articulos para el hogar" respectivamente, en el séptimo lugar en ventas las tiendas 1 y 2 tienen la categoría de "Libros", mientras que en las tiendas 3 y 4 tienen "Instrumentos musicales" y "Libros" respectivamente, ya en el último lugar en ventas las tiendas 1, 2 y 3 tienen la categoría de "Articulos para el hogar", mientras que en la Tienda 4 rompe el patrón de igualdad en los puestos por última vez teniendo la categoría de "Instrumentos musicales"

3. Calificación promedio de la tienda

Objetivo:En este paso, debes calcular las calificaciones promedio de los clientes para cada tienda. El objetivo es conocer la satisfacción del cliente con los productos vendidos.

![3. Calificación promedio de la tienda](3.%20Calificación%20promedio%20de%20la%20tienda.png)

Notas de la Calificación promedio de la tienda:

-Calificaciones Totales:

La calificación promedio general, considerando las cuatro tiendas, es de aproximadamente 4.02 puntos (promedio de 3.98, 4.04, 4.05 y 4.00)

-Ranking por Tienda basado en calificación promedio:

1°) Tienda 3: Lidera con una calificación promedio de 4.05 puntos

2°) Tienda 2: Sigue muy de cerca con 4.04 puntos

3°) Tienda 4: Ocupa el tercer lugar con 4.00 puntos

4°) Tienda 1: Registra la menor calificación promedio con 3.98 puntos

-Diferencias Notables:

Las calificaciones promedio entre las tiendas son extremadamente similares, todas rondando los 4.0 puntos sobre 5. La diferencia entre la tienda con la calificación más alta, la Tienda 3 y la más baja, la Tienda 1 es mínima (solo 0.07 puntos). Esto sugiere un nivel de satisfacción del cliente bastante homogéneo y generalmente positivo en las cuatro tiendas
