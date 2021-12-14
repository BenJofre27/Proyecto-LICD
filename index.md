# <img style="float: left; padding-right: 0.2cm; width: 9.0cm" src="https://th.bing.com/th/id/R.69cb7735a422db336e0d49d0dc89c21c?rik=YmUVpMyvcM4B%2bw&pid=ImgRaw&r=0">

## Análisis de rendimiento del Campeonato Nacional de Futbol Chileno Profesional entre los años 2010 a 2020

#### Este proyecto surgió por el fanatismo que tenemos hacia el futbol, los torneos nacionales y cada amistoso que se ha desarrollado que hemos puesto nuestra atencion, desarrollando un gran sentimiento de amor y aprecio por el deporte, generando lazos con equipos determinados por su juego, cordinacion y determinacion por ganar.

#### Dando un paso mas alla, nos intrigo el funcionamiento de cada equipo para que nos den el espectaculo que tanto nos gusta ver en vivo, y nos concentramos en analizar estadisticas de los campeonatos nacionales de fútbol profesional chileno de primera división.

#### Utilizamos como fuentes de información las paginas siguientes:

- #### Wkipedia, que nos facilitaba la obtención de resultados positivos, ya que poseia varias tablas con información útil respecto al año de torneo que se requería, y era mas sencillo aplicar web scraping.

- #### Tansfermarkt, el cual provee información sobre valores de mercados de los equipos, vlores de mercado de los jugadores, ingresos obtenidos por venta de jugadores de los equipos por año, costos obtenidos por la compra de jugadores de los equipos por año, etc.

#### Nuestra propuesta fue analizar las estadisticas de torneos y mundiales futbolisticos de la ultima decada; donde tocamos temas como:

- #### Estadisticas descriptivas de desempeño por equipo en cada año que participaron del torneo

- #### Comprender la distribucion por region de los equipos en permanencia en primera division

- #### Relacion entre popularidad (en base a hinchada) y rendimiento de un equipo por torneo 

- #### Relacion del balance total por equipo en concepto de venta y compra de jugadores y su rendimiento

#### 1-¿Existe correlación entre la popularidad de un equipo y su rendimiento en los torneos?

#### 2-¿Cómo es la distribución de los equipos por región participantes de los torneos por año?

#### 3-¿Existe correlación entre ser un equipo de región y el rendimiento de dicho equipo?

#### 4-¿De qué regiones son los equipos con mejor rendimiento?

#### 5-¿Existe correlación entre el balance total en concepto de compra y venta de jugadores de los 3 mejores equipos y los 3 peores equipos de los torneos por años y su rendimiento en los torneos?

#### 6-¿Serán los equipos que más invierten los con mejor rendimiento?

# Observaciones y hallazgos

### Veamos un gráfico que presente los puntos obtenidos por todos los equipos en nuestro Data Frame final.

{% include graphg.html %}

### Veamos un **mapa** con el cual podremos visualizar la distribución de los equipos y su estadio a lo largo de Chile.

{% include figure.html %}


### Los resultados hallados durante el estudio de lo planteado los responderemos en base a la relacion que tienen con respecto a las preguntas de investigación planteadas:


<img style="float: left; padding-right: 0.4cm; width: 8.5cm" src="https://raw.githubusercontent.com/fmeza7/Proyecto_Cs_Datos_Grupo_1/main/graficos%20finales/regresion_2/regresion_2.png">

#### 1) Respondiendo a la pregunta 1, utilizamos el dataset de los equipos que permanecieron en primera división durante todo el intervalo de tiempo medido para el proyecto. Es importante resaltar que el numero de datos ingresados son bajos ya que el Nº de equipos que se mantuvo en primera división durante los 10 años en que se midio el proyecto fueron 9. De esta manera las metricas utilizadas como el MSE y R2, dificilmente son posibles de analizar correctamente debido a la baja cantidad de datos. Por lo tanto el análisis para este apartado estaría sesgado debido a la baja cantidad de datos.

<img style="float: left; padding-right: 0.8cm; width: 8.0cm" src="https://raw.githubusercontent.com/fmeza7/Proyecto_Cs_Datos_Grupo_1/main/graficos%20finales/GDF_ESPECIFICO.PNG" width="600" height="315">

#### 2) Para la pregunta dos apreciamos que gran parte de los equipos que han estado en primera división estos 10 útlimos años pertenecen a la región metropolitana. Se puede apreciar que en general estos equipos son los que presentan un mayor gasto en compra y venta de jugadores, lo que habla del poder adquisitivo de estos equipos en comparación con los equipos de regiones. También es notoria la diferencia en la capacidad de los estadios, superando hasta en casi 4 veces el tamaño de los estadios de los equipos de regiones pequeños.

##### Distribución de equipos que permanericeron en primera división.

{% include huasos.html %}


#### 3) Para las preguntas 3 y 4, al analizar el dataframe de rendimiento acumulado, vemos que 6 de los 7 equipos de la región metropolitana se han mantenido sin descender a lo largo del intervalo de tiempo estudiado. Esto puede ser indicativo de que al ser un equipo de región se tiene mayores probabilidades de descender a la segunda división del fútbol chileno. No consideramos el ser de región como variable categórica en el análisis ya que pudimos llegar a esta conclusión mediante el dataframe de rendimiento acumulado.

<img style="float: left; padding-right: 0.4cm; width: 8.0cm" src="https://raw.githubusercontent.com/fmeza7/Proyecto_Cs_Datos_Grupo_1/main/graficos%20finales/regresion_1/lasso_esp.png">

#### 4) Y con respecto a las ultimas dos preguntas, en base al modelo multilineal con regularización seleccionado(regresión Lasso con alfa igual a 1), notamos que las variables ingresos y costos no tienen un peso significativo en la predicción de cantidad de puntos obtenidos por equipo, por lo tanto estas variables no estan influyendo en los rendimientos de los equipos.

---

### Video de la presentación

<p align="center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/t5098uwdkMo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

---
#### Referencias:
* ##### Tablas de campeonatos :
    * ##### [2020](https://es.wikipedia.org/wiki/Primera_Divisi%C3%B3n_de_Chile_2020)
    * ##### [2019](https://es.wikipedia.org/wiki/Primera_Divisi%C3%B3n_de_Chile_2019)
    * ##### [2018] : https://es.wikipedia.org/wiki/Primera_Divisi%C3%B3n_de_Chile_2018
    * ##### 2017 : https://es.wikipedia.org/wiki/Torneo_de_Transici%C3%B3n_2017_(Chile)
    * ##### 2016 : https://es.wikipedia.org/wiki/Torneo_Clausura_2017_(Chile)
    * ##### 2015 : https://es.wikipedia.org/wiki/Torneo_Clausura_2016_(Chile)
    * ##### 2014 : https://es.wikipedia.org/wiki/Torneo_Clausura_2015_(Chile)
    * ##### 2013 : https://es.wikipedia.org/wiki/Temporada_2013-2014_del_f%C3%BAtbol_chileno
    * ##### 2012 : https://es.wikipedia.org/wiki/Torneo_Clausura_2012_(Chile)
    * ##### 2011 : https://es.wikipedia.org/wiki/Torneo_Clausura_2011_(Chile)
    * ##### 2010 : https://es.wikipedia.org/wiki/Primera_Divisi%C3%B3n_de_Chile_2010
    
* ##### Datos de Estadio y Asistencia:
    * ##### Asistencia de público: http://www.estadioseguro.gob.cl/2019/01/04/asistencia-de-publico-a-los-estadios-marca-cifra-record-en-2018/
    * ##### Estadios: https://es.wikipedia.org/wiki/Anexo:Estadios_de_f%C3%BAtbol_de_Chile
    
* ##### Datos de transferencias 2010-2021:
    * ##### Transferencias : https://www.transfermarkt.es/primera-division-de-chile/einnahmenausgaben/wettbewerb/CLPD/plus/0?ids=a&sa=&saison_id=2009&saison_id_bis=2009&nat=&pos=&altersklasse=&w_s=&leihe=&intern=0