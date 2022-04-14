# Detección de anomalías en despachos de combustible
<small>Guía de trabajo como parte de la mentoría en Diplomatura en Ciencia de Datos FaMAF-UNC 2022.</small>

## Descripción
La identificación de anomalías en el consumo de combustible es un aspecto crucial para optimizar consumos, reducir costos e identificar posibles fallas en los dispositivos. 

El objetivo de este trabajo es identificar transacciones anómalas registradas por nodos IoT en los surtidores para su posterior análisis. 

Algunos resultados que se esperan obtener a partir de este proyecto son:
- Detectar posibles fallas en los surtidores para realizar un mantenimiento proactivo.
- Identificar posibles fugas o descargas inusuales en una estación.

Los prácticos contarán con ejercicios de base y algunos ejercicios opcionales para quienes quieran profundizar en el área.

### Este tema es interesante porque…
El desarrollo en la industria de sistemas basados en el Internet de las Cosas (IoT) surge ante la necesidad de poder contar con datos en tiempo real sobre distintos dispositivos con el objetivo de monitorear, aumentar la productividad o controlar los inventarios. Estos datos de por sí no aportan demasiada información a los usuarios si no se analizan o procesan. De allí, nace el uso de la inteligencia artificial en este rubro en auge para poder brindar información relevante a partir de los datos. El mundo IoT y Ciencia de Datos es un área en constante crecimiento.

Además, este trabajo es interesante ya que aplicando técnicas de análisis y machine learning simples se pueden obtener buenos resultados. 

### Trataremos de responder algunas de las siguientes preguntas:
¿Existen características comunes que se pueden observar en las transacciones detectadas como anómalas?
¿Es importante la temporalidad de los datos?
¿Se observan comportamientos similares entre las distintas estaciones? ¿Y entre sectores?
¿Ciertas transacciones podrían considerarse anómalas en una estación mientras que en otra no?
¿Se pueden ver secuencias de transacciones anómalas? ¿O siempre se encuentran esporádicamente en el tiempo?
¿Podría la anomalía tratarse de una falla en el surtidor?
Datos
Las transacciones de despacho registradas en este dataset son realizadas por varios sectores de la industria, tales como empresas de transporte, estaciones de servicios, telecomunicaciones, minería, petroleras, etc.

El conjunto pertenece a datos reportados por nodos IoT durante los meses de enero a marzo de 2022. 

Se trata de un conjunto de series temporales y contiene en general la siguiente información:
- Nro de la transacción.
- Fecha y hora de inicio y de fin de la transacción.
- Cantidad de litros de combustible despachado.
- Volumen real registrado por otros nodos IoT en los tanques durante el inicio y fin de la descarga.
- Estación, surtidor, empresa de origen.
- Tipo de combustible transaccionado.
- Geolocalización (si es soportada).
- Unidad de consumo de destino.
- Sector de la industria a la que pertenece la estación.

Si querés inspeccionar el conjunto de datos, lo encontrarás en
https://www.kaggle.com/datasets/danielabosch/fuel-transactions-from-gas-pump o bien https://drive.google.com/file/d/1xTyVgattNoHQMSJnqUyg8P4W-_d-UMWI/view?usp=sharing 

## Hitos de la Mentoría
**Entrega 20/05 - Práctico de análisis y visualización.**
En este trabajo conocemos los datos, observamos sus distintas variables y nos familiarizamos con las series temporales. Podremos obtener una primera aproximación a los resultados observando la distribución de las variables de las series. Algunos temas a tratar:
- Visualización de series temporales, uso de pivotes, groupby.
- Estadística descriptiva sobre variables de interés.
- Correlación entre variables.
- Visualización de outliers sobre distintas variables.
- (Opcional) Descomposición de series temporales. Visualización de la estacionalidad, la tendencia y el residuo de una serie temporal.

**Entrega 17/06 - Práctico de análisis exploratorio y curación de datos.**
Realizamos agregaciones sobre las series para observar otros comportamientos. Aplicamos otros estadísticos de interés, como las medias móviles para acercarnos una segunda aproximación a los resultados. Además, dejamos listo nuestro dataset para los siguientes trabajos. Algunos temas a tratar:
- Análisis sobre agregaciones sobre la cantidad despachada.
- Medias móviles, medianas móviles para observar anomalías.
- Imputación de datos faltantes para el correcto funcionamiento de los modelos a utilizar en los trabajos posteriores.
- Guardado del dataset con los tipos de datos adecuados.
- (Opcional) Media móvil sobre el residuo de una serie descompuesta.
 
**Entrega 24/06 - Video de presentación intermedia del proyecto y dataset**
 
**Entrega 29/07 - Práctico aprendizaje supervisado.**
Utilizamos técnicas supervisadas para la detección de anomalías. Predecimos a partir de errores conocidos como el código de error, la cantidad cero, etc. Identificamos los falsos positivos. Algunos temas a tratar:
- Resultados con distintos modelos.
- (Opcional) Uso de técnicas semi supervisadas.
 
**Entrega 26/08  - Práctico aprendizaje no supervisado, que consistirá en:**
Detectamos anomalías con técnicas no supervisadas. Realizamos una comparación sobre las distintas estrategias usadas. Algunos temas a tratar:
- Clustering en series temporales.
- Outliers globales, contextuales, colectivos.
- (Opcional) Detección basada en forecasting y otras técnicas.
 
**Entrega 23/09 - Video de presentación final de mentoría**
 
**Jornadas 11/11 y 12/11 - Presentación de mentorías**
