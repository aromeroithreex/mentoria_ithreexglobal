# Potencia las Ventas con IA: Aprende a Usar Clustering, Predicción, sistemas de recomendaciones y AI generativa para construir un asistente de venta de consumo mayorista.

## 🧠  Descripción y Objetivo del Proyecto

Este proyecto parte de una base de datos transaccional que registra ventas realizadas a distintos puntos de venta (PDV), los cuales funcionan como clientes en el sistema.
El objetivo es aplicar técnicas de ciencia de datos para extraer valor estratégico y mejorar la toma de decisiones comerciales.

Se trabajará sobre tres ejes principales:

🔹 Clusterización de Puntos de Venta
Se buscará segmentar los PDV en grupos con comportamientos de compra similares. Esto permitirá:

Identificar patrones en las dinámicas comerciales

Optimizar campañas de marketing

Asignar recursos de manera más eficiente

🔹 Sistema de Recomendación
Se desarrollará un modelo de recomendación basado en el historial de ventas, con el fin de:

Sugerir productos relevantes para cada cliente

Aumentar la efectividad comercial y fidelización

🔹 Predicción de Demanda
Se entrenarán modelos supervisados para estimar la demanda futura por PDV y producto. Esto permitirá:

Mejorar la planificación logística

Reducir pérdidas por exceso o falta de inventario

Optimizar el manejo de stock

La mentoría busca que los participantes apliquen metodologías reales de ciencia de datos sobre un caso concreto, combinando exploración, modelado y comunicación de resultados.

## ❓ Preguntas que Guiarán el Proyecto
¿Qué patrones de comportamiento de compra se pueden identificar entre los puntos de venta?

¿Cómo segmentar a los PDV para reflejar diferencias significativas en sus hábitos de consumo?

¿Qué productos conviene recomendar a cada PDV para maximizar las ventas?

¿Es posible anticipar la demanda futura de productos para mejorar la logística?

¿Qué variables influyen más en el volumen de ventas y cómo varían según el cliente?

## 🧪 Estructura de los Prácticos (a definir)

✅ Práctico 1 – Análisis y Visualización

Consistira en la exploración inicial del dataset para comprender la estructura de los datos y sus principales características. Se realizará un análisis descriptivo de las variables más relevantes (volumen de ventas, frecuencia de compra, productos, puntos de venta, fechas, entre otros), y se generarán visualizaciones que permitan detectar tendencias, estacionalidades, patrones de comportamiento y posibles anomalías.

El objetivo de este práctico es familiarizarse con la base de datos, identificar relaciones significativas entre variables y establecer hipótesis iniciales que guíen los siguientes pasos del proyecto. Se utilizarán herramientas como Pandas, Matplotlib, Seaborn y Plotly para la manipulación y visualización interactiva de los datos.

✅ Práctico 2 – Análisis Exploratorio y Curación de Datos

Se trabajara la depuración, transformación y validación del dataset para asegurar su calidad antes del modelado. Se identificarán y tratarán valores faltantes, inconsistencias, duplicados y outliers. También se realizarán transformaciones necesarias y ajuste de formatos de fechas.

Adicionalmente, se ajustarán los valores monetarios por inflación utilizando índices de precios oficiales para homogeneizar los montos a moneda constante. Luego, se aplicará una estandarización de los montos con el fin de facilitar la comparación entre puntos de venta y mejorar la performance de los modelos de machine learning.

Todas las decisiones tomadas durante esta etapa serán documentadas, y se evaluará su impacto sobre la integridad del conjunto de datos.

✅ Práctico 3 – Modelado con Machine Learning

Se trabajara la implementación de modelos de machine learning tanto supervisados como no supervisados para abordar los distintos objetivos del proyecto.
En la fase de aprendizaje no supervisado, se aplicarán algoritmos de clusterización como K-Means, DBSCAN o Gaussian Mixture Models para segmentar los puntos de venta en función de su comportamiento de compra. Esta segmentación permitirá identificar grupos con características similares, facilitando estrategias comerciales diferenciadas por perfil de cliente.
En paralelo, se desarrollará un sistema de recomendación de productos para cada punto de venta. Se explorarán tanto enfoques colaborativos (basados en similitud entre puntos de venta) como basados en contenido (características de los productos o historial de compra). El objetivo será sugerir productos relevantes para cada cliente, optimizando la oferta comercial y aumentando la probabilidad de compra.
Por último, en la fase de aprendizaje supervisado, se construirán modelos de predicción de demanda por punto de venta y producto, utilizando algoritmos como XGBoost, Random Forest, regresión lineal, redes neuronales u otros. Estos modelos permitirán anticipar el volumen de ventas, mejorando la planificación logística, el abastecimiento y la gestión de inventario. Como bonus, integraremos toda la informacion de salida de cada practico a un repositorio de datos para que un modelo de AI Generativa genere las recomendaciones mediante un asistente teniendo en cuenta dichos datos.



