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

<script type="application/json" data-for="htmlwidget-34790fa5d5cfaf44a456">{"x":{"filter":"none","data":[["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","31","32","33","34","35","36","37","38","39","40","41","42","43","44","45","46","47","48","49","50","51","52","53","54","55","56","57","58","59","60","61","62","63","64","65","66","67","68","69","70","71","72","73","74","75","76","77","78","79","80","81","82","83","84","85","86","87","88","89","90","91","92","93","94","95","96","97","98","99","100","101","102","103","104","105","106","107","108","109","110","111","112","113","114","115","116","117","118","119","120","121","122","123","124","125","126","127"],["1983","1983","1984","1984","1985","1985","1986","1987","1987","1988","1988","1989","1989","1990","1991","1992","1992","1993","1994","1994","1994","1994","1995","1995","1995","1995","1995","1996","1996","1996","1996","1996","1997","1997","1997","1997","1997","1998","1998","1998","1998","1998","1999","1999","1999","1999","1999","2000","2000","2000","2000","2000","2001","2001","2001","2001","2001","2002","2002","2002","2002","2002","2003","2003","2003","2003","2003","2004","2004","2004","2004","2004","2005","2005","2005","2005","2005","2006","2006","2006","2006","2006","2007","2007","2007","2007","2007","2008","2008","2008","2008","2008","2009","2009","2009","2009","2009","2010","2010","2010","2010","2010","2011","2011","2011","2011","2011","2012","2012","2012","2012","2012","2013","2013","2013","2013","2013","2014","2014","2014","2014","2014","2015","2015","2015","2015","2015"],["Activision","Nintendo","Activision","Nintendo","Activision","Nintendo","Nintendo","Activision","Nintendo","Activision","Nintendo","Activision","Nintendo","Nintendo","Nintendo","Electronic Arts","Nintendo","Nintendo","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft","Activision","Electronic Arts","Nintendo","Sony Computer Entertainment","Ubisoft"],[1.94,10.96,0.27,45.56,0.48,49.95,16.18,1.12,11.95,0.75,36.44,0.47,63.88,35.49,15.97,0.06,38.11,20.04,2.08,0.65,24.99,3.43,4.21,3.33,16.72,18.45,3.03,1.95,7.9,73.7,35.07,0.16,2.55,22.94,25.8,43.9,0.25,7.54,29.95,48.41,34.64,0.3,7.57,20.15,65.33,36.24,4.61,14.48,25.13,34.05,21.69,4.75,18.59,45.12,45.37,43.29,4.99,25.94,73.01,48.31,25.85,16.21,21.38,69.83,38.14,24.32,16.89,39.23,67.33,60.65,35.16,15.4,35.39,67.01,127.47,26.38,16.49,17.4,58.41,205.61,33.81,17.27,63.57,71.33,104.18,37.54,48.6,67.41,84.12,91.22,26.64,57.44,78.06,86.2,128.89,36.53,47.01,63.39,81.38,61.07,34.89,42.62,51.74,72.25,51.53,27.4,48.03,53.25,49.9,56.47,12.85,37.31,43.49,52.92,52.79,12.61,27.39,44.48,46.8,48.65,19.02,41.95,35.63,45.42,27.08,11.01,12.79],[2,0,0,1,0,1,3,2,0,1,0,1,0,0,1,0,1,0,0,0,1,0,0,0,0,2,0,1,3,1,0,0,1,1,1,3,0,2,1,1,4,1,0,2,2,3,0,4,2,2,3,3,6,4,2,4,1,13,13,6,4,7,5,13,0,3,17,12,10,5,2,10,22,13,2,7,18,8,12,3,2,10,22,18,3,5,13,32,5,1,2,13,44,25,3,5,16,19,16,3,5,16,24,22,6,8,13,29,16,7,11,10,8,2,4,3,10,22,0,4,6,11,17,4,7,5,14],[1,4,0,0,0,4,2,0,0,0,3,0,1,1,2,0,1,2,0,0,4,0,0,0,3,2,1,0,0,4,2,0,0,0,4,3,0,3,1,3,4,0,1,0,2,3,3,2,0,5,2,8,0,0,3,4,5,1,4,4,5,8,5,1,4,3,5,10,4,14,4,0,6,0,6,4,6,8,0,4,2,6,7,0,4,3,0,0,2,5,7,1,0,1,1,5,7,4,0,4,3,0,1,0,3,4,6,0,0,2,2,3,7,0,5,0,8,0,0,3,2,3,3,0,4,1,0],[0,0,0,0,0,0,0,0,1,0,0,0,0,0,1,0,1,0,0,0,0,0,0,1,0,1,0,0,1,0,0,0,0,0,0,2,0,0,1,1,3,0,1,0,0,1,0,0,0,0,3,1,0,0,1,0,4,0,2,4,4,3,0,0,1,3,4,1,1,7,0,4,5,1,3,3,2,0,0,0,7,2,5,1,3,1,8,2,0,2,1,7,4,2,5,2,12,2,0,2,4,6,2,3,1,1,6,0,0,1,2,0,0,0,1,3,0,3,0,0,0,0,0,0,0,0,0],[0,0,0,1,1,1,0,0,0,0,1,0,3,2,2,0,4,2,0,0,0,0,0,0,4,0,0,0,0,2,0,0,1,0,2,1,0,1,0,1,3,0,0,0,1,0,0,0,0,2,2,0,1,0,2,0,2,0,0,0,0,1,1,0,2,0,1,0,0,8,0,1,0,1,4,3,3,0,0,9,2,1,1,0,6,0,3,0,3,1,1,4,0,3,3,0,4,0,0,3,0,2,0,0,1,0,1,0,0,1,0,0,0,0,1,0,0,1,0,1,0,1,0,0,4,0,0],[0,0,0,2,0,0,0,0,0,1,0,0,1,0,2,0,0,1,0,0,0,1,0,3,0,5,0,1,0,0,0,0,0,0,2,4,0,1,1,0,0,0,2,1,1,2,0,0,1,1,1,0,1,2,0,3,1,5,14,1,1,4,5,11,0,2,7,6,8,3,2,8,14,16,1,3,15,8,5,2,5,12,10,11,2,3,8,12,11,0,2,8,18,4,2,2,3,13,10,0,4,3,8,9,1,5,5,7,1,0,2,7,12,12,0,2,0,12,8,0,0,5,9,8,1,1,3],[0,1,0,1,0,0,0,0,0,0,0,0,1,0,0,0,2,0,0,0,0,0,0,1,1,2,0,0,0,0,7,0,0,0,2,1,0,1,1,1,4,0,1,0,3,4,1,0,1,1,4,0,1,0,0,6,0,1,1,2,3,1,1,0,4,11,2,0,0,7,8,1,4,0,9,9,2,5,1,15,10,3,12,5,9,13,18,18,11,7,13,24,29,7,5,14,17,8,8,5,9,15,13,7,6,9,29,2,0,6,0,10,0,0,4,0,10,0,0,2,1,11,5,0,6,0,7],[0,1,0,2,0,1,0,0,1,0,1,0,3,1,2,0,0,1,0,0,1,2,0,2,0,4,0,0,6,1,6,0,0,12,1,5,0,0,14,3,4,0,1,7,2,2,3,3,14,3,11,1,9,20,0,11,3,18,37,1,6,5,10,34,1,6,0,10,36,3,9,0,12,51,4,10,0,11,52,4,8,0,6,45,3,9,11,14,50,2,6,16,9,34,4,5,5,24,32,2,6,12,9,20,0,5,8,0,17,2,3,1,0,21,2,2,0,0,22,2,0,0,4,15,1,3,6],[0,0,1,2,0,0,1,0,0,0,1,0,0,2,1,0,1,1,0,0,0,2,0,3,0,1,0,0,2,3,4,1,0,3,1,7,1,2,5,2,1,2,1,11,2,4,3,2,8,3,3,0,3,11,3,7,2,5,13,0,2,6,1,9,4,1,2,2,10,2,3,3,1,16,1,5,3,4,13,1,7,4,9,10,2,2,2,9,13,1,1,2,8,12,1,6,3,10,4,0,3,2,12,3,1,1,9,2,4,0,3,0,0,6,0,1,0,0,0,1,1,7,0,2,0,0,0],[0,0,0,0,1,0,0,0,0,0,0,0,0,1,1,0,0,0,0,2,0,0,0,1,0,3,0,0,1,1,1,0,1,3,0,3,0,0,0,2,1,0,0,0,1,1,2,1,1,0,1,1,1,2,2,0,0,2,4,1,1,0,0,11,0,0,4,0,7,0,0,1,1,9,4,0,5,0,9,1,0,13,2,13,1,1,19,0,15,3,0,29,3,16,1,1,29,6,9,1,1,8,5,7,2,1,5,0,1,2,0,1,0,1,1,0,0,0,1,1,0,0,0,3,1,0,0],[0,0,0,0,0,0,0,0,2,0,0,0,0,0,0,0,0,1,0,0,0,1,0,0,1,4,0,0,0,2,5,0,0,1,0,1,0,1,2,0,4,0,0,3,1,0,0,0,1,1,0,3,1,2,1,0,2,4,0,0,0,3,0,2,1,1,1,0,5,0,0,0,0,8,1,2,0,0,5,2,3,1,0,0,0,2,1,0,3,1,2,2,0,2,1,2,2,0,2,0,2,1,0,2,0,0,1,0,0,1,1,0,0,0,0,0,1,0,0,2,0,0,0,0,0,0,0],[0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,1,0,0,2,1,0,0,1,4,0,1,0,2,3,0,0,1,0,2,0,1,0,1,2,0,1,0,2,5,1,1,0,2,2,3,0,1,4,3,5,1,0,3,4,4,2,1,8,2,4,5,4,5,2,4,5,0,8,2,2,6,1,12,5,6,1,2,5,2,3,1,1,8,2,1,6,3,5,1,1,2,6,7,1,0,0,3,5,2,1,2,7,9,0,0,2,0,4,1,0,3,5,4,3,6,0,0,7,0,0],[0,0,0,0,0,0,0,0,0,0,0,0,0,0,1,1,0,0,1,0,0,0,1,0,0,3,0,0,0,1,0,0,0,4,0,2,0,2,4,2,0,0,0,2,3,0,0,0,3,3,0,1,0,1,4,0,0,0,0,0,0,2,4,3,2,0,0,1,1,3,0,0,0,2,2,0,1,0,4,0,0,3,0,2,4,0,2,0,6,1,0,5,0,3,1,2,3,1,1,1,5,7,1,0,0,0,3,0,0,0,0,0,9,0,1,0,0,1,0,0,0,0,1,0,1,0,2]],"container":"<table class=\"display\">\n  <thead>\n    <tr>\n      <th> <\/th>\n      <th>Year<\/th>\n      <th>Publisher<\/th>\n      <th>Global_Sales<\/th>\n      <th>Action<\/th>\n      <th>Platform<\/th>\n      <th>Adventure<\/th>\n      <th>Puzzle<\/th>\n      <th>Shooter<\/th>\n      <th>Misc<\/th>\n      <th>Sports<\/th>\n      <th>Racing<\/th>\n      <th>Simulation<\/th>\n      <th>Fighting<\/th>\n      <th>Role-Playing<\/th>\n      <th>Strategy<\/th>\n    <\/tr>\n  <\/thead>\n<\/table>","options":{"pageLength":5,"scrollX":true,"columnDefs":[{"className":"dt-right","targets":[3,4,5,6,7,8,9,10,11,12,13,14,15]},{"orderable":false,"targets":0}],"order":[],"autoWidth":false,"orderClasses":false,"lengthMenu":[5,10,25,50,100]}},"evals":[],"jsHooks":[]}</script>

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
