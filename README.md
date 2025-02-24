# 📊🧮Pruebas-A-B-para-Estrategias-de-Marketing 📈
## Descripción del proyecto
Como analista en una gran tienda online, colaboré estrechamente con el departamento de marketing para identificar y explorar estrategias que pudieran aumentar nuestros ingresos. Se recopilo una lista de hipótesis que, según, podrían tener un impacto significativo en las ventas.
Mi tarea consistió en priorizar estas hipótesis, diseñar y ejecutar un test A/B para evaluar su efectividad. Después de implementar los tests, analicé los resultados para determinar qué enfoques fueron más exitosos. Este proceso permitió identificar las estrategias más efectivas y proporcionar recomendaciones basadas en datos para mejorar las futuras campañas de marketing, optimizando así el rendimiento general de la tienda online.

## Motivación
El proceso de priorizar hipótesis y realizar tests A/B es clave para entender qué tácticas realmente funcionan y cómo afectan las ventas. Analizar los resultados y hacer recomendaciones basadas en datos es fundamental para ajustar y mejorar continuamente las campañas de marketing, maximizando el retorno de inversión. Este tipo de proyectos es motivador porque no solo ofrece la posibilidad de influir en el éxito de la tienda, sino también de contribuir a una toma de decisiones más efectiva y eficiente, ayudando a la empresa a crecer y mejorar en un entorno altamente competitivo. Además, este enfoque de trabajo permite adquirir habilidades clave en análisis de datos, pruebas y optimización de estrategias, lo que es esencial en el mundo del marketing digital.

## Características del Dataset

### /datasets/orders_us.csv

-transactionId: identificador de pedido.

-visitorId: identificador del usuario que realizó el pedido.

-date: fecha del pedido.

-revenue: ingresos del pedido.

-group: el grupo del test A/B al que pertenece el usuario.

### /datasets/visits_us.csv

-date: la fecha.

-group: grupo de la prueba A/B.

-visits: el número de visitas en la fecha especificada en el grupo de pruebas A/B especificado.

## Herramientas Utilizadas
### Lenguaje: 
Python 
### Librerías:
-pandas para la manipulación de datos.
-numpy para cálculos numéricos.
-matplotlib y seaborn para visualizaciones.
-scikit-learn para la creación y evaluación de modelos de Machine Learning.
-scipy.stats para calculos estadísticos 
Jupyter Notebook para la documentación del análisis.

## Proceso del Proyecto
### Carga y Exploración de Datos
Análisis inicial del dataset: revisión de los valores faltantes, tipos de datos y distribuciones.
Exploratory Data Analysis (EDA) para entender las relaciones entre las variables 

### Limpieza y Preprocesamiento
Imputación de valores faltantes en variables.
Conversión de variables categóricas en variables numéricas, date.
Normalización de variables continuas

### Priorizar hipotesis 

1.Aplicar el framework ICE para priorizar hipótesis. Ordenarlas en orden descendente de prioridad.

2.Aplicar el framework RICE para priorizar hipótesis. Ordenarlas en orden descendente de prioridad.

3.Mostrar cómo cambia la priorización de hipótesis cuando utilizas RICE en lugar de ICE.

Proporcionar una explicación de los cambios.

### Análisis del test A/B

#### Ingreso acumulado por grupo
Se representó gráficamente el ingreso acumulado por cada grupo. Los resultados mostraron que el grupo A obtuvo un ingreso más estable, mientras que el grupo B experimentó un aumento significativo en el ingreso a partir del segundo día. Esto sugiere que el grupo B pudo haber respondido positivamente a un cambio implementado, como una oferta especial o modificación en el diseño.

#### Tamaño de pedido promedio acumulado por grupo
El gráfico del tamaño de pedido promedio acumulado mostró que el grupo B superó al grupo A en términos de monto promedio de pedido después de unos días. Esto podría indicar que las estrategias implementadas en el grupo B impulsaron a los usuarios a gastar más.

#### Diferencia relativa en el tamaño de pedido promedio acumulado
La diferencia relativa en el tamaño de pedido promedio entre los grupos mostró un crecimiento progresivo a favor del grupo B. Esto sugiere que la intervención tuvo un impacto positivo en el comportamiento de compra en el grupo B.

#### Tasa de conversión diaria de cada grupo
Al graficar las tasas de conversión diarias, se observó que el grupo B mostró una tasa de conversión más alta en comparación con el grupo A, especialmente durante los primeros días. Esto indicó que las tácticas en el grupo B atrajeron más conversiones por visita.

#### Gráfico de dispersión del número de pedidos por usuario
Se trazó un gráfico de dispersión para observar la distribución del número de pedidos por usuario. El gráfico mostró que el grupo B tenía una mayor concentración de usuarios que realizaron múltiples pedidos en comparación con el grupo A.

#### Cálculo de percentiles 95 y 99 del número de pedidos por usuario
Se calcularon los percentiles 95 y 99, y los puntos de datos por encima de estos percentiles fueron considerados anomalías. Se encontraron algunos puntos extremos en el grupo A, lo que podría sugerir comportamientos inusuales o usuarios con pedidos extraordinarios.

#### Gráfico de dispersión de precios de pedidos
El gráfico de dispersión de precios de pedidos mostró que los precios se distribuyeron de manera más homogénea en el grupo B, mientras que el grupo A tenía más pedidos de bajo precio.

#### Cálculo de percentiles 95 y 99 de precios de pedidos
Se calcularon los percentiles 95 y 99 de los precios, y los valores por encima de estos percentiles fueron considerados anomalías. Los datos sugirieron que los precios más altos en el grupo A podrían estar asociados con usuarios que hicieron compras excepcionales.

#### Significancia estadística de la diferencia en conversión entre grupos
Al analizar la significancia estadística, se encontró que la diferencia en la tasa de conversión entre los grupos era estadísticamente significativa. Esto sugiere que la intervención aplicada en el grupo B realmente tuvo un impacto positivo.


#### Significancia estadística de la diferencia en el tamaño promedio de pedido
El análisis estadístico también reveló una diferencia significativa en el tamaño promedio de pedido entre los grupos. Esto respalda la hipótesis de que las estrategias en el grupo B tuvieron un impacto directo en el valor de los pedidos.


#### Significancia estadística de la diferencia en conversión entre los grupos (datos filtrados)
Al realizar un análisis con los datos filtrados, la diferencia en las tasas de conversión se mantuvo estadísticamente significativa, lo que refuerza los resultados anteriores.


#### Significancia estadística de la diferencia en el tamaño promedio de pedido entre los grupos (datos filtrados)
Se observó que la diferencia en el tamaño promedio de pedido entre los grupos se mantenía significativa, incluso después de filtrar los datos.


#### Decisión basada en los resultados de la prueba
Basándonos en los resultados de la prueba, donde el grupo B mostró mejoras claras en ingresos, tamaño de pedido y tasa de conversión, la recomendación fue parar la prueba y considerar al grupo B como líder.







