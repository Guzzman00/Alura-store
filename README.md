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

🎨 **Vista Previa**

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

4. Productos más y menos vendidos

Objetivo:En este paso, debes identificar qué productos fueron los más vendidos y los menos vendidos en cada tienda. Visualiza los resultados para que quede claro qué productos destacaron en ventas en cada tienda.

![4-1. Productos más y menos vendidos](4-1.%20Productos%20más%20y%20menos%20vendidos.png)

![4-2. Productos más y menos vendidos](4-2.%20Productos%20más%20y%20menos%20vendidos.png)

Notas de los Productos más y menos vendidos:

-Ventas Totales de los productos más vendidos:

El número total de ventas acumuladas en las cuatro tiendas, sumando todos los productos más vendidos, es de 1165 unidades

-Ventas Totales de los productos menos vendidos:

El número total de ventas acumuladas en las cuatro tiendas, sumando todos los productos menos vendidos, es de 709 unidades

-Ranking de los Productos más vendidos basado en las ventas generadas:

1°) Iniciado en programación en Tienda 2: Lidera con un total de 65 ventas

2°) Microondas en Tienda 2 y Cama box en Tienda 4: Siguen con 62 ventas

3°) Batería en Tienda 2: Ocupa el tercer lugar con 61 ventas

4°) Microondas, TV LED UHD 4K, Armario en Tienda 1: Registran 60 ventas

5°) Cubetería en Tienda 4: Suma 59 ventas

-Ranking de los Productos menos vendidos basado en las ventas generadas:

1°) Juego de mesa en Tienda 2: Lidera con un total de 32 ventas

2°) Auriculares con micrófono y Celular ABXY en Tienda 1 y Guitarra en Tienda 4: Siguen con 33 ventas

3°) Impresora y Mesa de comedor en Tienda 2 y Armario en Tienda 4: Ocupan el tercer lugar con 34 ventas

4°) Olla a presión en Tienda 1, Sillón en Tienda 2 y Bloques de construcción en Tienda 3: Registran 35 ventas

5°) Pandereta en Tienda 1 y Set de vasos, Microondas y Mochila en Tienda 3: Suman 36 ventas

-Diferencias Notables:

El producto "Iniciado en programación" de la Tienda 2 se destaca como el más vendido en general, liderando con 65 unidades. El segundo lugar en ventas es compartido por dos productos distintos en tiendas diferentes: "Microondas" en Tienda 2 y "Cama box" en Tienda 4, ambos con 62 ventas. La Tienda 2 también alberga el tercer producto más vendido, "Batería", con 61 unidades. Curiosamente, el cuarto puesto lo comparten tres productos exclusivos de la Tienda 1 "Microondas", "TV LED UHD 4K", "Armario", todos con 60 ventas. Finalmente el quinto lugar pertenece a "Cubetería" en la Tienda 4 con 59 ventas

El producto "Juego de mesa" de la Tienda 2 se destaca como el menos vendido en general, registrando solo 32 unidades. El segundo lugar con menos ventas es compartido por tres productos distintos en dos tiendas diferentes: "Auriculares con micrófono" y "Celular ABXY" en Tienda 1 y "Guitarra" en Tienda 4, todos con 33 ventas. El tercer puesto entre los menos vendidos lo comparten también tres productos, ubicados en Tienda 2 "Impresora" y "Mesa de comedor" y Tienda 4 "Armario", con 34 unidades cada uno. Curiosamente, el cuarto puesto con menos ventas lo comparten tres productos distribuidos en tres tiendas distintas: "Olla a presión" en Tienda 1, "Sillón" en Tienda 2 y "Bloques de construcción" en Tienda 3, todos con 35 ventas. Finalmente, el quinto lugar con menos ventas pertenece a cuatro productos repartidos entre Tienda 1 "Pandereta" y Tienda 3 "Set de vasos", "Microondas" y "Mochila", con 36 ventas por cada producto

Rendimiento de tiendas según sistema de puntuación

Reglas del sistema de puntuación:

Se evaluó el rendimiento de cada tienda asignando puntos basados en la presencia de sus productos en los rankings generales del top 5 más vendidos y anti-top 5 menos vendidos:

Productos más vendidos: Puntos positivos asignados por ranking (1°: +11, 2°: +7, 3°: +5, 4°: +3, 5°: +1).
Productos menos vendidos: Puntos negativos asignados por ranking (1°: -11, 2°: -7, 3°: -5, 4°: -3, 5°: -1).
Puntaje final: Suma de todos los puntos positivos y negativos obtenidos por cada tienda

Análisis de rendimiento por tienda según puntuación:

Tienda 2:

Obtuvo +23 puntos por sus productos top 5, pero -24 puntos por sus productos anti-top 5
Puntaje final: -1 punto
Tienda 4:

Sumó +8 puntos por sus productos top 5 y restó -12 puntos por sus productos anti-top 5
Puntaje final: -4 puntos
Tienda 3:

No obtuvo puntos positivos (sin productos top 5) y restó -6 puntos por sus productos anti-top 5
Puntaje final: -6 puntos
Tienda 1:

Consiguió +9 puntos por sus productos top 5 y acumuló la mayor penalización -18 puntos por sus productos anti-top 5
Puntaje final: -9 puntos

Ranking (mayor a menor puntaje):

1). Tienda 2 (-1 punto)
2). Tienda 4 (-4 puntos)
3). Tienda 3 (-6 puntos)
4). Tienda 1 (-9 puntos)

5. Envío promedio por tienda

Objetivo:En este paso, debes calcular el costo de envío promedio para cada tienda. El objetivo es comprender cuánto se gasta, en promedio, en el envío de cada tienda.

![5. Envío promedio por tienda](5.%20Envío%20promedio%20por%20tienda.png)

Notas del Envío promedio por tienda:

-Envios Totales:

El costo de envío promedio general, considerando las cuatro tiendas, es de aproximadamente $24.875 de dolares (promedio de USD 26.019, USD 25.216, USD 24.806 y USD 23.459)

-Ranking por Tienda basado en costo de envío promedio:

1°) Tienda 1: Lidera con el costo de envío promedio más alto USD 26.019

2°) Tienda 2: Sigue con un costo promedio de USD 25.216

3°) Tienda 3: Ocupa el tercer lugar con USD 24.806

4°) Tienda 4: Registra el costo de envío promedio más bajo con USD 23.459

-Diferencias Notables:

Se observa una tendencia decreciente en el costo de envío promedio desde la Tienda 1 hasta la Tienda 4. La diferencia entre la tienda con el costo más alto, la Tienda 1 y la de costo más bajo, la Tienda 4 es de aproximadamente de USD 2.560 dolares. Si bien hay una clara jerarquía, las diferencias entre tiendas consecutivas no son drásticas, sugiriendo políticas de envío o destinos con costos relativamente escalonados entre las tiendas

6. ¡Extra! Análisis del desempeño geográfico

Esta actividad es un extra, por lo tanto es OPCIONAL.

En este extra, tendrás el desafío de explorar las coordenadas geográficas de los datos de ventas e identificar patrones relacionados con la ubicación de las compras. Al utilizar las columnas de latitud y longitud, puede generar visualizaciones para comprender cómo varían las ventas según la ubicación geográfica.

Desafío:

Utilice los datos de latitud (lat) y longitud (lon) para mapear las ventas de cada tienda y analizar la distribución geográfica de los productos vendidos.

Genere gráficos de dispersión o mapas de calor (Heatmaps) para visualizar datos e identificar áreas con la mayor concentración de ventas.

Explore si algunas tiendas tienen un rendimiento superior o inferior al esperado en determinadas regiones e identifique si existen patrones geográficos que puedan influir en el rendimiento de las tiendas.

Sugerencias:

Puede utilizar la biblioteca Matplotlib para gráficos de dispersión o incluso integrarla con otras bibliotecas como Folium para generar mapas interactivos si desea ir más allá.

Analice cómo las variables geográficas influyen en los ingresos y las calificaciones de las tiendas.

![6-1. ¡Extra! Análisis del desempeño geográfico](6-1.%20¡Extra!%20Análisis%20del%20desempeño%20geográfico.png)

![6-2. ¡Extra! Análisis del desempeño geográfico](6-2.%20¡Extra!%20Análisis%20del%20desempeño%20geográfico.png)

![6-3. ¡Extra! Análisis del desempeño geográfico](6-3.%20¡Extra!%20Análisis%20del%20desempeño%20geográfico.png)

![6-4. ¡Extra! Análisis del desempeño geográfico](6-4.%20¡Extra!%20Análisis%20del%20desempeño%20geográfico.png)

![6-5. ¡Extra! Análisis del desempeño geográfico](6-5.%20¡Extra!%20Análisis%20del%20desempeño%20geográfico.png)

![6-6. ¡Extra! Análisis del desempeño geográfico](6-6.%20¡Extra!%20Análisis%20del%20desempeño%20geográfico.png)

Influencia Geográfica en Rendimiento

Influencia en Ingresos:

Tienda 1: Aunque registra el mayor ingreso total, su liderazgo no proviene de dominar los mercados más grandes (es superada ligeramente en Bogotá por T4 y T2, y es la más baja en Medellín con 563 ventas). Su fortaleza radica en ser la tienda con el mayor volumen de ventas en Cali (283) y mantener una presencia consistente, aunque no siempre líder, en casi todas las ciudades de menor tamaño listadas (ej: Pereira 133, Cúcuta 51, Armenia 14, Inírida 5), sumando un volumen significativo a través de esta amplia cobertura geográfica

Tienda 2: Su segundo lugar en ingresos se explica por su excelente desempeño en los dos principales mercados: es la tienda con más ventas en Medellín (594) y la segunda en Bogotá (985). También lidera en Cartagena (70) y Cúcuta (59). Su fuerte concentración en estos puntos de alto volumen compensa su menor presencia en las ciudades más pequeñas

Tienda 3: Similar a Tienda 2, su tercer puesto en ingresos se basa en un rendimiento sólido en Bogotá (983) y Medellín (580). Logra liderar marginalmente en Pereira (134) y Neiva (10). Al igual que la Tienda 2, su impacto en las ciudades más pequeñas es menor que el de la Tienda 1

Tienda 4: A pesar de tener el mayor número de ventas en Bogotá (991) y Barranquilla (80), su cuarto lugar en ingresos totales sugiere que su rendimiento comparativamente más bajo en el segundo mercado más grande (Medellín, 577) y su desempeño variable sin claro liderazgo en ciudades medianas (ej: Cali 254, Pereira 122, Cartagena 63) limitan su facturación general
Influencia en Calificaciones:

La ubicación geográfica no parece ser un factor determinante para las calificaciones promedio. Como se observó antes, todas las tiendas tienen calificaciones muy similares (entre 3.98 y 4.05). Los datos numéricos por ciudad no revelan un patrón que conecte altos volúmenes de venta en ciertas ciudades (ej: Bogotá, Medellín) o el liderazgo en ciudades específicas con una calificación promedio consistentemente más alta o más baja. Esto refuerza la idea de que la satisfacción del cliente es homogénea y probablemente depende más de otros factores (calidad del producto, políticas generales, experiencia de compra global, etc.)

7. Informe Final

1-Introducción

Se realizó un análisis comparativo de Tienda 1, Tienda 2, Tienda 3 y Tienda 4, evaluando múltiples factores de rendimiento: ingresos totales, ventas por categoría, calificaciones promedio de clientes, rendimiento de productos individuales (más y menos vendidos, y un sistema de puntuación derivado), costo de envío promedio y distribución geográfica de las ventas. El objetivo es identificar la tienda cuyo perfil general la convierte en la candidata más lógica para una desinversión o venta, considerando tanto fortalezas como debilidades.

2-Resumen Comparativo por Tienda

Tienda 1: Es la líder indiscutible en ingresos totales (aprox. USD 1,151M), lográndolo a través de una amplia cobertura geográfica y buen desempeño en ciudades medianas/pequeñas. Sin embargo, presenta la calificación promedio más baja (3.98, aunque la diferencia es mínima), el costo de envío promedio más alto (USD 26.019) y el peor puntaje en el ranking de productos (-9), indicando una posible acumulación de inventario de baja rotación o "flops".

Tienda 2: Ocupa el segundo lugar en ingresos (aprox. USD 1,116M) y calificaciones (4.04), sustentado por un fuerte desempeño en los mercados más grandes (Bogotá y Medellín) y por tener los productos individuales más vendidos (1° y 2° lugar). Obtuvo el mejor puntaje en el ranking de productos (-1), reflejando el éxito de sus "hits". Sus puntos débiles son tener también el producto menos vendido absoluto y el segundo costo de envío más alto (USD 25.216).

Tienda 3: Presenta la calificación promedio más alta (4.05), costos de envío competitivos (USD 24.806 - 3° lugar) y un puntaje de productos aceptable (-6) al evitar los productos de ventas extremadamente bajas. Sin embargo, ocupa el tercer lugar en ingresos (aprox. USD $1,098M) y es la única sin productos en el Top 5 de más vendidos, dependiendo fuertemente de Bogotá y Medellín.

Tienda 4: Registra los ingresos más bajos (aprox. USD $1,038M) y un rendimiento geográfico generalmente inferior, aunque lidera puntualmente en Bogotá y Barranquilla. Sus puntos fuertes son el costo de envío promedio más bajo (USD 23.459), una calificación aceptable (4.00 - 3° lugar) y un buen puntaje de productos (-4) gracias a tener artículos en el 2° y 5° puesto de los más vendidos.

3-Análisis para la Decisión de Venta

La decisión sobre qué tienda vender depende de la estrategia a seguir:

Vender la de menor rendimiento (Tienda 4) liberaría recursos, pero se perdería la operación con menores costos de envío.

Vender la más estable y con mejor satisfacción (Tienda 3) podría ser un error si se valora la lealtad del cliente y el bajo riesgo, aunque carece de productos estrella.

Vender la más dinámica (Tienda 2) sacrificaría el mayor potencial de "hits" y una buena combinación de ingresos/satisfacción.

Vender la líder en ingresos (Tienda 1) podría parecer contraintuitivo, pero permite capitalizar su valor actual mientras se evitan posibles problemas futuros derivados de sus altos costos de envío, baja eficiencia de inventario (peor puntaje de productos) y la calificación marginalmente inferior.

4-Conclusión

Considerando todos los factores, la venta se inclina hacia la Tienda 1.

Justificación: Si bien es la que genera mayores ingresos actualmente, también presenta las señales de alerta más significativas en términos de eficiencia operativa y satisfacción relativa. Su alto costo de envío, su bajo rendimiento en el puntaje de productos (sugiriendo problemas de inventario o marketing para una parte de su catálogo) y su calificación, aunque alta, siendo la más baja del grupo, indican áreas que requerirían inversión y esfuerzo para optimizar. Venderla ahora permitiría al Sr. Juan obtener potencialmente el mayor valor por su activo principal, mientras concentra recursos en las otras tiendas (especialmente la Tienda 2 con su dinamismo y la Tienda 3 con su estabilidad y satisfacción) que, aunque facturan menos, presentan perfiles operativos quizás más equilibrados o con "problemas" más acotados. Vender la Tienda 1 es una decisión estratégica para capitalizar su posición actual antes de que sus debilidades operativas puedan erosionar su valor.
