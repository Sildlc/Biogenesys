# Biogenesys

La empresa farmacéutica BIOGENESYS se encuentra en la evaluación de distintas locaciones para la expansión de sus instalaciones. 

Por el nivel de inversiones a realizar  y los objetivos que se han fijado, han decidido que se deben considerar los datos de incidencia de COVID-19, tasas de vacunación y disponibilidad de infraestructuras sanitarias, para optimizar la respuesta a los efectos de la pandemia y postpandemia.

Los objetivos de la empresa son:
- Facilitar la toma de decisiones futuras basando dicho proceso en datos que poseen
- Identificar ubicaciones estratégicas para la apertura de nuevos laboratorios y centros de vacunación
- Mejorar el acceso a las vacunas


### Introducción

Con el presente proyecto solicitan realizar un estudio y análisis de los datos proporcionados, que ayude a la toma de decisiones futuras que requiere su estrategia de expansión en Latinoamérica, específicamente en los países de Argentina, Brasil, Chile, Colombia, México y Perú. 

Los objetivos del proyecto son concretos y medibles:
- Realizar un análisis exploratorio de datos sobre la incidencia de COVID-19 y otros factores relevantes, identificando tendencias y patrones mediante estadísticas, mediciones y visualizaciones.
- Aplicar técnicas de limpieza de datos para asegurar la calidad de los datos.
- Mejorar el acceso a los datos mediante operaciones eficientes de extracción, transformación y carga (ETL), aumentando la eficacia del análisis y la toma de decisiones.
- Desarrollar dashboards interactivos con visualizaciones eficientes, permitiendo explorar datos desde múltiples perspectivas para una toma de decisiones informada y poder obtener oportunidades que faciliten una expansión eficiente
- Se utilizarán los datos proporcionados por la empresa para ofrecer insights valiosos sobre posibles ubicaciones estratégicas para futuros laboratorios y centros de vacunación. 


### Desarrollo del proyecto

Con los datos suministrados en un primer avances se han realizado limpiezas de datos faltantes y nulos que eviten distorsiones en los análisis y mediciones posteriores. 

Para asegurar la disponibilidad de los datos con los cuales se trabaja en todo el proceso se guarda y pone a disponibilidad un nuevo dataset que con los cambios realizados será la base para los siguientes avances. (“DatosFinalesFiltrado.csv”) El archivo posee 3744 registros y 50 columnas (originalmente el archivo proporcionado para el proyecto era de 22 millones de registros y 707 columnas)

Durante el primer avance se trabaja con las librerías de NUMPY y PANDAS registrando todas la modificadiones en un archivo de extensión .ipynb con comentarios que clarifican o dan cuenta de los criterios utilizados en cada operación. 
Se obtienen los datos estadísticos descriptivos (mediana, promedios, percentiles) de las columnas que han sido filtradas y forman parte del archivo final.

Durante el segundo avances se hace un anáisis exploratorio de los datos para realizar con ellos visualizaciones que den cuenta de información valiosa para obtener patrones, tendencias, relaciones o inconsistencias que afecten la evaluación.
Se utilizan las librerias de MATPLOTLIB Y SEABORN que permiten realizar histograma, gráficos de barras, gráficos de líneas, gráficos de densidad poblacional, gráficos de dispersión de variables y de mapas que muestren correlaciones entre ellas.

En esta etapa también se realizaron analisis temporales, ubicando el periodo de análisis central desde el inicio del año 2021 en adelante ya que fue el solicitado por ser el año de desarrollo de la pandemia en conjunto con la vacunación.


### EDA e Insights

Durante un tercer avance con los datos se procede a relizar cálculos y visualizaciones que permitan brindar información valiosa, patrones o tendencias a tener en cuenta.
Se analizan datos con los distintos criterios o segmentaciones:
- por pais y comparación entre ellos
- edades (se establecen grupos etáreos para analizar su evolución con la pandemia, porcentajes de mortalidad y vacunacion recibida
- distribución geográfica (nivel de urbanización y su correspondiente relación con las vacunas recibidas y su respuesta a la pandemia
- cantidad de casos que presentaron evoluciones positivas o que se han recuperado e indices de mortalidad,incidencia de la vacunación,
- crecimiento de los casos o contagios y de decesos, en lapsos temporales de meses
- temperaturas promedio en los distintos paises y su incidencia en los resultados obtenidos o evolución de la pandemia
- nivel de urbanización y su relación con estrategia de vacunación realizada
- prevalencia de enfermedades prexistentes (como diabetes o fumadores) para la respuesta a la pandemia y a su evolución posterior

 
Al analizar los datos y las visualizaciones mencionadas se podrian mencionar los siguientes hallazgos:

- Las estrategias de vacunación realizadas por los 6 paises analizados son muy distintas entre si, teniendo en cuenta que sus dimensiones geograficas, distribución poblacional urbana y por rango etáreo también presentan diferencias y que a nivel nacional los distintos gobiernos establecieron momentos, población afectadas y estrategias de vacunación distintas
- Las temperaturas pueden tener una correlación con la cantidad de casos aunque no necesariamente a mayor temperatura la incidencia es menor ya se pueden ver momentos de altas temperatura y aumento de casos
- Para el caso de factores que inciden en la evolución de los casos si brinda una tendencia el analisis de las poblaciones con enfermedades prexistentes como diabetes, ya que los paises se componen de manera muy distinta y eso conlleva una necesidad de atención sanitaria y estrategias de vacunación diferentes con éste tipo de poblaciones
- También se ha identificado la falta de valores por país en cuanto a la mortalidad, o registro temporal correspondiente que afecta el análisis que se pretendió realizar ya que al reemplazar valores con promedios o máximos puede ser una estimación teorica que lleva a no percibir diferencias entre los paises analizados

### Análisis del dashboard
Se realiza un Dashboard para que se puedan observar de manera intearactiva datos agrupados de la siguiente forma:
- Datos de la Pandemia ( visualizaciones por pais de casos de enfermos, mortalidad y casos recuperados)
- Estrategia de vacunación (cómo se realizó la vacunacion en tiempo, grupos afectados, y distribución)
- Análisis demograficos (densidad poblacional, acceso a la vacunación, grupos etáreos, enfermedes prexistentes)
- Conclusiones y recomendaciones sugeridas por el analista

