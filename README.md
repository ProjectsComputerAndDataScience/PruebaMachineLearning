Ejercicio
================

Por favor contesta las siguientes 5 preguntas sobre implementaciones
algoritmicas de ciencia de datos.

Si tienes alguna duda o crees que se necesita hacer algun supuesto para
resolver la pregunta por favor hazlo. (y decláralo)

La base de datos que se presenta a continuación pertenece al repositorio
**open-source de KAGGLE**
<https://www.kaggle.com/gregorut/videogamesales>.

La base contiene la información de ventas por año y desarrollador (top
10 en ventas) a nivel global desde 1983 hasta 2015 con el número de
juegos publicados por genero en el año.

<!--html_preserve-->

<div id="htmlwidget-34790fa5d5cfaf44a456" class="datatables html-widget" style="width:100%;height:auto;">

</div>


<!--/html_preserve-->

## Pregunta 1: Regresión lineal

1.  Utiliza la base de datos Pregunta1.csv para construir un código
    **reutilizable** que; primero filtre las filas cuya columna
    **Publisher sea igual a “Nintendo”**. Con esta sub-base calcule la
    regresion de la columna Global\_Sales como variable objetivo a
    predecir ‘Y’ contra las demas columnas numéricas (es decir de Action
    a Strategy). Después se deberá obtener la serie de predicciónes de
    “Global\_Sales” \(\hat{Y}\) y con esta calucular el **error medio
    absoluto** = \[\frac{\sum_{t=1..T}{|y_t-\hat{y}_t}|}{T}\]

Por favor muestra el valor del Error medio absoluto aqui:

2.  Utiliza el codigo anterior ( o modifícalo si asi lo consideras) para
    correr ese mismo ejercicio **para cada uno de los niveles de la
    variable “Publisher”**. En este ejercicio lo que buscamos es una
    lista de 5 elementos numericos donde cada uno contenga el valor del
    error medio absoluto del la venta del Publisher “i” vs la prediccion
    de esa venta por elmodelo “i”.

Por favor muestra la lista (nombrada) o diccionario aqui:

*Las llaves o nombres deben corresponder al nivel de la variable
Publisher para el cual se ajusto el modelo*

# Pregunta 2 : Red Neuronal

**Por favor para esta pregunta considera unicamente las filas de la
tabla cuyo Publisher sea Nintendo.**

Utiliza esta base y tensorflow / pythorch (puedes tambien usar API’s
como keras para interactuar con ellos) para construir una red neuronal
con una única capa oculta totalmente conexa (de 10 neuronas) . La red
neuronal tendra que predecir el valor de la variable Global\_Sales para
cada año dados las columnas: (Action Platform Adsventure Puzzle Shooter
Misc Sports Racing Simulation Fighting Role-Playing Strategy)

Ajusta el modelo y obten \(\hat{Y}\) ; Despues **calcula el error
absoluto promedio** de este modelo

Por favor escribe el error absoluto promedio del modelo aqui:

# Pregunta 3 : Random Forest with extreme boosting

**Por favor para esta pregunta considera unicamente las filas de la
tabla cuyo Publisher sea Nintendo.**

Por favor, construye un modelo de bosque aleatorio a partir de muestras
bootstrap de la tabla. Si gustas usa los siguientes hiperparametros -o
propon los propios-:

1.  profundidad maxima de cada arbol 7 niveles  
2.  numero de arboles 1000
3.  sub\_muestra (para bootstrap) .9
4.  numero de caracteristicas por arbol 7

El bosque aleatorio tendrá que predecir el valor de la variable
**Global\_Sales** ‘\(Y\)’ para cada año dados las columnas: **(Action
Platform Adventure Puzzle Shooter Misc Sports Racing Simulation Fighting
Role-Playing Strategy)**

Ajusta el modelo y obten \(\hat{Y}\) ; Despues **calcula el error
absoluto promedio** de este modelo

Por favor escribe el error absoluto promedio del modelo aqui:

**Sugerencia**

Para este ejercicio puedes usar las libreria xgboost o scikit learn

# Pregunta 4 : ARIMA’s / Prophet

**Por favor para esta pregunta considera unicamente las filas de la
tabla cuyo Publisher sea Nintendo.**

Ajusta un modelo de serie de tiempo clasico (ARIMA) para la variable
Global\_Sales o implementa el algoritmo de la libreria prophet.

El modelo propuesto tendrá que predecir el valor de la serie de tiempo
**Global\_Sales** ‘\(Y\)’ para cada año

Ajusta el modelo y obten \(\hat{Y}\) ; Despues **calcula el error
absoluto promedio** de este modelo

Por favor escribe el error absoluto promedio del modelo aqui:

# Pregunta 5 : Resultados

Presenta una tabla con el resultado del error absoluto promedio para
cada uno de los modelos implementados en la parte 1 a 4,

1.  Si solo un modelo se pudiera implementar en produccion , ¿Cuál
    recomendarias? ¿Porqué?

2.  ¿Qué mejorarías en los modelos para que se ajusten mejor al data set
    utlizado? (por ejemplo para tomar en cuenta la correlación entre
    observaciones)

**Por favor envia tus resultados en una carpeta comprimida “.zip” con el
siguiente nombre : nombre\_candidato\_consultora.zip la carpeta debera
contener tanto las respuestas a las preguntas aquí expuestas como el
CODIGO que se ejecutó para la obtención de las mismas.(por ejemplo un
archivo con el codigo .py y un archivo con las repuestas .txt o word )**
