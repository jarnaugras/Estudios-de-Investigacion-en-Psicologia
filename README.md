Diseños Experimentales en Psicología
Herramientas para el análisis y creación de datos en investigación experimental psicológica

Introducción
La página web que presentamos tiene por objetivo facilitar el análisis de datos para los diseños experimentales de uso común en las ciencias sociales y de la salud, especialmente en psicología y educación. De esta forma, pretendemos resolver, de manera rápida y sin dificultades, el problema de obtener resultados de los trabajos científicos dentro de este contexto.
Se evita el uso de programas complejos propios para estadísticos como son, por ejemplo, el SPSS, SAS, Minitab y R, entre otros. Este último, el programa R, requiere una mínima formación en programación. Todo ello añade una grave dificultad para quienes están centrados en investigar y obtener respuestas inmediatas a las hipótesis de trabajo.
Palabras clave: Diseño experimental, estadística, caso único, modelos de análisis, anova.
Páginas web de libre acceso
Presentamos, de mamera sucinta, cuatro páginas web orientadas a la resolucón de problemas de análisis en el ámbito psicologico. Las tres primeras son intrumentos útiles para la ejecución del análisis y la presentación gráfica relativas a diseños expeerimentales clásicos y diseños de caso único. La cuarta  página web permite generar datos, completamente ficticios, que pueden usarse a modo de ejemplo para la ejecución de los análisis.
1.	Diseños Experimentales Clásicos
  URL: "https://jarnau.shinyapps.io/disexpsy/"
  Contiene los diseños experimentales clásicos utilizados en psicología.
2.	Diseños de Medidas Repetidas
  URL: "https://jarnau.shinyapps.io/disexpsy-mr/"
   Se centra particularmente en los diseños de medidas repetidas.
3.	Diseños de Caso Único
  URL: "https://jarnau.shinyapps.io/discupsy/"
  Ofrece la posibilidad de analizar los diseños de caso o sujeto único propios del ámbito clínico y educativo.
4.	Generador de Datos
  URL: "https://jarnau.shinyapps.io/creardisexpsy/"
  Herramienta útil para quienes estén interesados en utilizar un sistema generador de datos para los diseños anteriormente descritos.
En este documento solo se describirán las condiciones de ejecución y características de la primera página web, en la que se recogen los principales modelos de diseños experimentales clásicos en Psicología.

Consideraciones Generales en Torno a los Diseños Experimentales en Psicología
Los diseños experimentales, utilizados en ciencias sociales y de la salud, son estrategias de investigación que se ajustan a un patrón determinado. Su estructura se articula en términos de variables:
  Variable dependiente o de respuesta: Valores de medida
  Variable/s independiente/s o tratamiento/s: Variables manipuladas por el investigador
   Variable de sujeto o id: Identificador de los participantes
   Covariables: De naturaleza biológica o social (edad, estatus socioeconómico, etc.)
La variación de los valores de la variable dependiente es resultado del manejo de las variables independientes y es función del impacto de la variable independiente. Por lo general, son medidas de la respuesta del sujeto a las condiciones de variación sistemática. La escala usada para su medición suele ser de intervalo.
Desde la perspectiva del diseño, la variable independiente es categórica y puede ser:
   Entre-sujetos: Toma valores distintos para distintos grupos de sujetos
   Intra-sujetos: Repite los valores para todos los sujetos de la muestra (variable de medidas repetidas)

Diseño de Caso Único
Una variedad de Diseño de investigación en la que se utiliza una unidad de observación (individuo o grupo) es el Diseño de Caso Único (Sujeto Único o N=1). Esta estructura sigue la lógica del diseño clásico en el sentido de estimar el posible efecto de la variable de tratamiento sobre las respuestas generadas, por lo general, por un sujeto.
Dentro del contexto del diseño de caso único:
   Las sesiones de observación configuran las fases
  Las fases representan distintos niveles de la variable de tratamiento o variable independiente   La unidad de observación puede ser un grupo de sujetos (ejemplo: el aula de una escuela)
   Se puede analizar el efecto de dos o más tratamientos así como sus posibles interacciones
Siempre deben adoptarse las debidas precauciones y controles para preservar la validez interna del diseño.
En Torno a los Datos: Creación de los Archivos de Datos en Formato CSV
El archivo o base de datos, en contextos de plataformas digitales o de Internet, suelen tener un formato 'csv' (columnas delimitadas por comas). El método más fácil para crear un fichero de datos es mediante el programa Excel:
1.	Crear tantas columnas como variables y etiquetarlas con el nombre de la respectiva variable
2.	Seleccionar de la barra de menús de Excel la pestaña Datos
3.	Clicar con el cursor la primera casilla de la primera columna
4.	Ir a Herramientas de los datos y ejecutar la secuencia:   Texto en columnas → siguiente
  Marcar la casilla de la 'coma' → siguiente   Marcar 'final'
5.	Guardar el fichero con un nombre
6.	En el desplegable inferior 'Tipo de fichero' marcar la opción 'CSV (delimitado por comas)'
Para verificar si se ha creado correctamente un fichero en formato csv, se puede abrir con el bloc de notas y comprobar si las columnas están separadas por comas.
El uso del formato csv (valores separados por comas) es soportado especialmente por programas y lenguajes de programación (Excel, R, Python, SPSS, MATLAB, etc.) y permite hacer transferencias sin necesidad de formatos propios. A su vez, pueden abrirse y editarse mediante un simple bloc de notas. Es un formato
estándar en el análisis estadístico, lo que facilita su manejo en R y permite el procesamiento de datos en aplicaciones como las desarrolladas por Shiny.
Modelos de Análisis de los Diseños Experimentales Clásicos
1.	Diseños de Grupos
Los diseños multigrupo o de grupos, de uso frecuente en ciencia psicológica y social, son estructuras de una sola variable independiente a tres o más valores o niveles. Se ajustan a un patrón de investigación en que los sujetos son totalmente asignados al azar a los diferentes grupos de tratamiento.
Al seleccionar más de dos valores de la variable independiente o de tratamiento, es posible extraer la relación funcional entre la variable independiente y dependiente del experimento. Por dicha razón, estas estructuras se conocen por experimentos funcionales. En suma, son estrategias de investigación conocidas también por diseños completamente al azar.

Diseño: A

Modelo One-Way ANOVA

Y = μ + Ai + ϵ Donde:
  Y es la variable dependiente
  Ai representa el efecto del grupo o factor (variable independiente categórica)   ϵ es el error aleatorio

Análisis

Se utiliza un ANOVA de un factor (one-way ANOVA o unifactorial) que permite comparar las medias de varios grupos y determinar si existen diferencias significativas entre ellos.

A Tener en Cuenta

Para aplicar un ANOVA de una vía (one-way ANOVA) en un diseño experimental multigrupo, se deben cumplir ciertos supuestos estadísticos clave:
1.	Independencia de las observaciones
   Las mediciones de cada grupo deben ser independientes entre sí
  Se debe asegurar que no haya dependencia entre las observaciones dentro de un mismo grupo ni entre grupos
2.	Normalidad de la variable dependiente
  La variable dependiente debe seguir una distribución normal en cada grupo de la variable independiente
  Se puede evaluar con pruebas como Shapiro-Wilk, Kolmogorov-Smirnov, o visualmente con histogramas o Q-Q plots
3.	Homogeneidad de varianzas (Homoscedasticidad)
  Las varianzas de los grupos deben ser aproximadamente iguales   Se puede verificar con pruebas como Levene o Bartlett
4.	Escala de medición adecuada
  La variable independiente debe ser categórica con dos o más niveles (grupos)   La variable dependiente debe ser continua (intervalo o razón)
2.	Diseño Factorial (Two-Way ANOVA)
Es un plan de trabajo que permite estudiar el efecto principal de dos factores o variables de tratamiento y al mismo tiempo el efecto cruzado entre ambos. Es decir, el grado en que la acción del primer factor depende del segundo. En la presente web se ha incorporado un modelo básico de diseño factorial de dos factores de uso frecuente en este contexto de investigación.
Diseño factorial: A x B Modelo:
Y = μ + Ai + Bj + (A×B)ij + ϵ Donde:
  Ai y Bj representan los efectos principales de dos factores independientes   (A×B)ij es el efecto de interacción entre ambos factores
  ϵ es el error aleatorio

Análisis

Se aplica un ANOVA factorial de dos factores (two-way ANOVA) que evalúa los efectos individuales de los factores y su interacción (efecto combinado).
A Tener en Cuenta

Para aplicar un ANOVA de dos vías (two-way ANOVA) en un diseño experimental factorial, se deben cumplir los siguientes supuestos estadísticos:
1.	Independencia de las observaciones
  Cada observación debe ser independiente de las demás
  Se debe garantizar que no haya relación entre las mediciones dentro de un mismo grupo ni entre grupos
2.	Normalidad de la variable dependiente
  La variable dependiente debe seguir una distribución normal en cada combinación de niveles de los factores
  Se puede evaluar con pruebas como Shapiro-Wilk, Kolmogorov-Smirnov, o mediante gráficos como histogramas o Q-Q plots
3.	Homogeneidad de varianzas (Homoscedasticidad)
  Las varianzas de la variable dependiente deben ser aproximadamente iguales en todos los grupos definidos por la combinación de los niveles de los factores
   Se puede verificar con la prueba de Levene o Bartlett
4.	Escala de medición adecuada
   Los factores deben ser variables categóricas con dos o más niveles
   La variable dependiente debe ser continua (escala de intervalo o razón)
5.	Aditividad y ausencia de interacción (para ciertos análisis)
  Si se desea interpretar los efectos principales sin interferencia de interacción, la interacción entre los factores debe ser mínima
  Sin embargo, el ANOVA de dos vías permite analizar interacciones entre factores, lo que debe verificarse mediante términos de interacción en el modelo
3.	Diseño de Medidas Repetidas (Repeated Measures ANOVA)
Con este formato, los sujetos de la muestra reciben todos los tratamientos y repiten medidas o registros de respuesta. La comparación de los tratamientos es intra-sujeto. El uso del procedimiento de medidas repetidas proporciona un control más efectivo de las fuentes de variación extrañas asociadas, por lo general, a las características individuales; es decir, se consigue una reducción de la variancia del error.
De este modo, la variabilidad debida a las diferencias individuales es eliminada del error y se convierte en un diseño más potente que el de los grupos completamente aleatorizados.
Diseño: S x A Modelo:
Y = μ + Ai + Sk + (A × S)ik + ϵ Donde:
   Ai es el efecto dentro de los sujetos (within-subjects factor)
  Sk representa la variabilidad individual entre los sujetos   (A×S)ik es el error dentro de los sujetos
  ϵ es el error residual

Análisis

Se usa un ANOVA de medidas repetidas incorporando la estructura de error adecuada con Error(sujeto/factor- intra). Se realiza además la prueba de esfericidad de Mauchly (mauchly.test) para verificar si se cumple la suposición de esfericidad.
Para ello se aconseja que:
   El factor repetido (la variable intra-sujetos) tenga al menos 3 condiciones (niveles)
  Se requiera una cantidad adecuada de sujetos, de 10 o más, para estimar correctamente la varianza y la covariancia entre las condiciones

A Tener en Cuenta

El diseño de medidas repetidas es uno de los formatos más comunes en Psicología, especialmente cuando se trata de estudiar el efecto del paso del tiempo o secuencias de carácter longitudinal.
1.	Independencia de las observaciones
  Cada sujeto debe ser independiente de los demás
  Sin embargo, dentro de cada sujeto, las mediciones pueden estar correlacionadas (por eso se usa este tipo de ANOVA)
2.	Normalidad de la variable dependiente
  La variable dependiente debe seguir una distribución normal en cada nivel del factor de medición repetida
  Se puede evaluar con pruebas como Shapiro-Wilk o Kolmogorov-Smirnov, así como con histogramas o Q-Q plots
3.	Esfericidad (Homogeneidad de varianzas y covarianzas)
  La varianza de las diferencias entre todas las combinaciones de pares de mediciones repetidas debe ser constante
  Se evalúa con la prueba de Mauchly
  Si este supuesto se viola, se pueden aplicar correcciones como Greenhouse-Geisser o Huynh- Feldt
4.	Escala de medición adecuada
  La variable independiente dentro de los sujetos (factor de medidas repetidas) debe ser categórica con dos o más niveles
   La variable dependiente debe ser continua (escala de intervalo o razón)

4.	Diseño Factorial de Medidas Repetidas (Factorial Repeated Measures ANOVA)
El diseño factorial de medida repetidas permite analizar de forma simultánea el efecto de varios factores cuyos valores se aplican, de forma cruzada, a cada uno de los sujetos de la muestra. Son factores de carácter intra-sujetos. Este tipo de diseño es común en psicología y otras ciencias del comportamiento, ya que permite evaluar cómo interactúan diferentes variables dentro de los mismos individuos a lo largo del tiempo o en diversas condiciones.
Al utilizar a los mismos sujetos en todas las condiciones, se reduce la variabilidad debida a diferencias individuales, lo que aumenta la sensibilidad estadística para detectar efectos de los factores y sus interacciones.

Diseño con dos factores intra-sujetos: S x A x B Modelo:
Y = μ + Ai + Bj + (A × B)ij + Sk + (A × S)ik + (B × S)jk + (A × B × S)ijk + ϵ
Donde:
  Ai y Bi son los factores intra-sujetos o efectos principales de la variables de medidas repetidas   (A × B)ij es la interacción entre factores intra-sujetos
   Sk es la variabilidad entre sujetos
  (A × S)ik es la interacción entre el factor A y S    (B × S)jk es la interacción entre el factor B y S
  (A × B × S)ijk es la interacción triple entre A, B y S   ϵ es el error residual

Análisis

Se usa un ANOVA factorial de medidas repetidas especificando la estructura de error adecuada. También se evalúa la prueba de esfericidad de Mauchly para verificar el supuesto de homogeneidad de las varianzas y covarianzas.

A Tener en Cuenta

1.	Independencia de las observaciones
  Cada sujeto debe ser independiente de los demás
   Sin embargo, dentro de cada sujeto, las mediciones repetidas pueden estar correlacionadas
2.	Normalidad de la variable dependiente
  La variable dependiente debe seguir una distribución normal en cada combinación de niveles de los factores repetidos
  Se evalúa con pruebas como Shapiro-Wilk o Kolmogorov-Smirnov, o con gráficos como histogramas y Q-Q plots
3.	Esfericidad (Homogeneidad de varianzas y covarianzas)
  La varianza de las diferencias entre todas las combinaciones de pares de mediciones repetidas debe ser constante
  Se evalúa con la prueba de Mauchly
  Si se viola este supuesto, se pueden aplicar correcciones como Greenhouse-Geisser o Huynh- Feldt
4.	Homogeneidad de las covarianzas
  Se asume que las correlaciones entre las mediciones repetidas son similares en todos los sujetos    Esto es una extensión del supuesto de esfericidad y puede evaluarse con matrices de covarianza
5.	Escala de medición adecuada
  Los factores dentro de sujetos (medidas repetidas) deben ser categóricos con al menos dos niveles
   La variable dependiente debe ser continua (escala de intervalo o razón)
5.	Diseño Factorial Mixto (Mixed ANOVA)
El diseño mixto integra, en un mismo estudio, dos enfoques de investigación lo cual requiere la presencia de al menos dos variables independientes. Así, los valores o niveles de la primera variable independiente generan grupos separados y su efecto se infiere por la comparación entre grupos o entre sujetos (estrategia entre- sujetos). Los valores de la segunda variable se administran a todos los sujetos, en cuyo caso los sujetos repiten medidas (estrategia intra-sujetos).
De esto se concluye que el diseño mixto requiere siempre una estructura factorial.

Diseño: S(A) x B Modelo:
Y = μ + Ai + Bj + (A × B)ij + Sk + (B × S)jk + ϵ
Donde:
   Ai es un factor entre sujetos (between-subjects)
  Bj es un factor dentro de sujetos (within-subjects)   (A × B)ij representa la interacción
   Sk es la variabilidad entre sujetos
  (B × S)jk es la variabilidad entre sujetos en el factor intra   ϵ es el error residual

Análisis

Se usa un modelo lineal mixto (Linear Mixed Model, LMM), considerando un factor aleatorio para los sujetos.

A Tener en Cuenta

1.	Independencia de las observaciones
  Las observaciones entre sujetos deben ser independientes
  Dentro de los sujetos, las mediciones repetidas pueden estar correlacionadas, pero deben seguir un patrón estructurado
2.	Normalidad de la variable dependiente
  La variable dependiente debe seguir una distribución normal en cada combinación de los niveles de los factores (dentro y entre sujetos)
  Se evalúa con pruebas como Shapiro-Wilk o Kolmogorov-Smirnov, o mediante gráficos como histogramas y Q-Q plots
3.	Homogeneidad de varianzas (para el factor entre sujetos)
  Las varianzas de los grupos definidos por el factor entre sujetos deben ser aproximadamente iguales
  Se evalúa con la prueba de Levene
4.	Esfericidad (para el factor dentro de sujetos)
  La varianza de las diferencias entre todas las combinaciones de mediciones repetidas debe ser constante
  Se evalúa con la prueba de Mauchly
   Si se viola, se aplican correcciones como Greenhouse-Geisser o Huynh-Feldt
5.	Escala de medición adecuada
   La variable independiente entre sujetos debe ser categórica con dos o más niveles
  La variable independiente dentro de sujetos (medidas repetidas) también debe ser categórica con al menos dos niveles
   La variable dependiente debe ser continua (escala de intervalo o razón)

6.	Diseño Split-Plot (ANOVA de Parcelas Divididas)
Tiene su origen en la investigación agrícola. La técnica split-plot consiste en dividir una zona amplia de terreno en una serie de parcelas o plots (variable de plots-completos) y, a su vez, subdividir cada uno de los plots completos en sub-plots (variable de sub-plots).
Su aplicación al campo psicosocial consiste en:
   Sustituir los plots-completos por grupos de sujetos
  Los sub-plots por repetir medidas de los sujetos (niveles de la variable de tratamiento) Desde la perspectiva longitudinal:
  Los sujetos son agrupados según los valores de una variable de clasificación o variable pronóstica   Son observados, mediante registro, a lo largo de una serie de puntos del tiempo (ocasiones de
observación)
  Tiene un carácter longitudinal

Diseño: S(A) x B Modelo:
Y = μ + Ai + Bj + (A × B)ij + Sk + (A × S)ik + ϵ Donde:
   Ai es el factor entre sujetos o tratamiento aplicado a la parcela grande (whole-plot factor)
  Bj es el factor intra-sujetos o tratamiento aplicado dentro de cada parcela (subparcelas o subplot factor)
  (A × B)ij es la variación de A dependiendo del nivel de B   Sk es la variabilidad entre sujetos
   (A × S)ik es el error de la parcela principal
   ϵ es el error residual (variabilidad no explicada por los efectos anteriores)

Análisis

Se usa un ANOVA de parcelas divididas (split-plot ANOVA), definiendo la estructura de error Error(sujeto/parcela).
 
Consideraciones Generales sobre el Diseño Split-Plot

En este diseño:
  La unidad experimental en la parcela completa es el grupo de sujetos que comparten el mismo nivel del factor entre sujetos
  Las parcelas subdivididas representan las condiciones o mediciones repetidas aplicadas dentro de esos grupos
  Esta estructura permite analizar tanto los efectos de los factores entre sujetos como los de los factores dentro de sujetos, así como sus posibles interacciones
Es importante destacar que, aunque los diseños split-plot se originaron en la agricultura, su aplicación en psicología y otras ciencias ha permitido manejar situaciones donde ciertos factores son más difíciles de manipular o aleatorizar completamente. Esto facilita la investigación de efectos complejos en contextos donde la aleatorización completa no es práctica o posible.
A Tener en Cuenta

1.	Independencia de las observaciones
  Las unidades experimentales principales (parcelas grandes) deben ser independientes entre sí   Las subunidades dentro de cada parcela pueden estar correlacionadas, lo cual se maneja
mediante el diseño
2.	Normalidad de la variable dependiente
  La variable dependiente debe seguir una distribución normal en cada combinación de niveles de los factores
  Se evalúa con pruebas como Shapiro-Wilk o Kolmogorov-Smirnov, o mediante gráficos como histogramas y Q-Q plots
3.	Homogeneidad de varianzas (Homoscedasticidad)
  Se debe cumplir para el factor de parcelas grandes (factor entre sujetos)   Se evalúa con la prueba de Levene
4.	Esfericidad para el factor de medidas repetidas
  Se aplica al factor de parcelas divididas (factor dentro de sujetos)   Se evalúa con la prueba de Mauchly
   Si se viola, se aplican correcciones como Greenhouse-Geisser o Huynh-Feldt
5.	Homogeneidad de las covarianzas
   Se asume que la relación entre mediciones repetidas dentro de cada parcela es constante
6.	Escala de medición adecuada
   Factor de parcelas grandes (entre sujetos): categórico con al menos dos niveles
  Factor de parcelas divididas (dentro de sujetos): categórico con al menos dos niveles   Variable dependiente: continua (escala de intervalo o razón)
 
Todos estos modelos permiten analizar diferentes tipos de diseños experimentales con estructura de datos específica, considerando tanto efectos fijos como aleatorios.
Cómo Entrar las Variables en los Campos de la App por Diseño
El procedimiento para el ingreso de las variables en las respectivas ventanas o campos de la web sigue la siguiente pauta, según el diseño de que se trate:
1.	Diseño de Grupos
Objetivo: Comparar la variable dependiente entre diferentes grupos definidos por un único factor.
   Variable Dependiente (Y): La medida de respuesta (por ejemplo, valor)
  Variables Independientes (X): El factor o tratamiento que define los grupos (por ejemplo, grupo o tratamiento)
  Variable Aleatoria: No se requiere
  Variables Entre/Intra: No se utilizan en este diseño

2.	Diseño Factorial (Two-Way ANOVA)
Objetivo: Evaluar el efecto de dos factores (por ejemplo, tratamientos) que se aplican entre sujetos, analizando efectos principales e interacción.
   Variable Dependiente (Y): La medida de respuesta (por ejemplo, valor)
   Variables Independientes (X): Los dos factores, separados por coma (por ejemplo, factor1, factor2)
  Variable Aleatoria: No se requiere, ya que cada combinación de factores corresponde a grupos distintos
  Variables Entre/Intra: No se utilizan en este diseño

3.	Diseño de Medidas Repetidas
Objetivo: Evaluar la variable dependiente en un mismo sujeto bajo diferentes condiciones u ocasiones de observación.
   Variable Dependiente (Y): La medida de respuesta (por ejemplo, valor)
  Variables Independientes (X): Un factor que representa las condiciones o momentos (por ejemplo, tiempo o condición)
  Variable Aleatoria: El identificador del sujeto (por ejemplo, sujeto), ya que cada sujeto es medido en todas las condiciones
  Variables Entre/Intra: No se utilizan en este diseño

4.	Diseño Factorial de Medidas Repetidas
Objetivo: Cada sujeto se evalúa en todas las combinaciones de dos factores; se analiza la variación intra- sujeto en ambos factores y su interacción.
   Variable Dependiente (Y): La medida de respuesta (por ejemplo, valor)
  Variables Independientes (X): Los dos factores, separados por coma (por ejemplo, factor1, factor2)   Ambos factores se consideran repetidos en cada sujeto
   Variable Aleatoria: El identificador del sujeto (por ejemplo, sujeto)
 
  Variables Entre/Intra: Generalmente no se utilizan campos adicionales para este diseño, ya que el modelo se construye a partir de los dos factores y el sujeto. Dejar en blanco "Entre" e "Intra" (a menos que la app requiera llenarlos, en cuyo caso podrías repetir los nombres de los factores, pero no es lo ideal)
5.	Diseño Factorial Mixto
Objetivo: Combina factores entre sujetos y dentro de los mismos sujetos, analizando efectos principales e interacciones considerando la estructura de datos anidada.
   Variable Dependiente (Y): La medida de respuesta (por ejemplo, valor)
   Variables Independientes (X): Los dos factores (por ejemplo, factor1, factor2)
   Variable Aleatoria: El identificador del sujeto (por ejemplo, sujeto)
  Variable Entre Sujetos: El factor que varía entre sujetos (por ejemplo, si factor1 es el que asigna a cada grupo, ingresa factor1)
   Variable Intra Sujetos: El factor que varía dentro de cada sujeto (por ejemplo, factor2)

6.	Diseño Split-Plot
Objetivo: Se utiliza cuando se aplican tratamientos a dos niveles: un factor (entre sujetos) a unidades mayores (por ejemplo, parcelas completas) y un segundo factor (intra sujetos) a subunidades.
   Variable Dependiente (Y): La medida de respuesta (por ejemplo, valor)
  Variables Independientes (X): Los dos factores, separados por coma (por ejemplo, factor1, factor2)   El primer factor se considera el factor entre sujetos (aplicado a las unidades grandes)
   El segundo factor es el factor dentro de sujetos (aplicado a las subunidades)
   Variable Aleatoria: El identificador del sujeto o bloque (por ejemplo, sujeto)
  Variables Entre/Intra: No se usan campos adicionales en la app para este diseño; la estructura se define mediante el orden de los factores en el campo de variables independientes
Resumen General
  Para diseños simples (Grupos, Medidas Repetidas, Factorial): Solo necesitas llenar Y y X (y Random en el caso de medidas repetidas)
  Para diseños mixtos y de medidas repetidas factoriales: Además, es obligatorio ingresar la Variable Aleatoria para identificar a cada sujeto
  Para el diseño mixto: Es importante especificar qué factor es entre sujetos y cuál es intra sujetos mediante los campos "Entre" e "Intra"
  Para el diseño split-plot: El primer factor en el campo X se asume como entre sujetos y el segundo como intra-sujetos, junto con la variable aleatoria
Con esta guía se podrán introducir correctamente las variables en la app según el diseño experimental que se esté utilizando.
Bibliografía en castellano
Arnau, J. (1975). Diseños experimentales en esquemas. Edicions de la Universitat de Barcelona, Barcelona.
Arnau, J. (1975). Los diseños experimentales en psicología. Anuario de Psicología, 12: 3-52.
Arnau, J. y Bono, R. (1997). Diseños experimentales: prácticas. Edicions de la Universitat de Barcelona, Barcelona.
Arnau, J. (1990). Diseños experimentales en psicología y educación (2da. Ed.). Vol. I. Trillas, México.
Arnau, J. (1990). Diseños experimentales en psicología y educación (2da. Ed.). Vol. II. Trillas, México.
Ato, M. y Vallejo, G. (2007). Diseños experimentales en psicología. Editorial Pirámide, Madrid.
Barlow, D.H. y Hersen, M. (1988). Diseños experimentales de caso único. Estrategias para el estudio del cambio conductual. Martínez Roca, Barcelona.
Balluerka, N. y Vergara, A.I. (2002). Diseños de investigación experimental en psicología. Pearson Educación, España.
Bono, R. y Arnau, J. (2014). Diseños de caso único en ciencias sociales y de la salud.  Síntesis, Madrid.

