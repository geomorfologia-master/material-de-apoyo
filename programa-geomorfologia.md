
<!-- Este .md fue generado a partir del .Rmd homónimo. Edítese el .Rmd -->

# Programa de “Geomorfología” <br/> Licenciatura en Geografía <br/> Universidad Autónoma de Santo Domingo (UASD)

Febrero 2022 <br/> *José Ramón Martínez Batlle, el tali*

## Básicos:

-   Correo: <jmartinez19@uasd.edu.do>

-   Lugar y horario: Zoom, Lunes de 4 a 8 pm

-   [Programa (vínculo recursivo)](programa-geomorfologia.md)

## Recursos informático de la asignatura

Sitúa apropiadamente los recursos de los que dispondrás en esta
asignatura, los cuales describo
[aquí](guia-redaccion-manuscrito.md#ecosistema).

## Descripción

Comienzo con una cita, primero en su idioma original, luego traducida:

> Earth’s landscapes are sculpted by a suite of geomorphic processes
> that vary with position on the Earth and with time due to changes in
> the climate. Landscapes contain signatures of the principal active
> processes that we would like to learn to read (Anderson & Anderson,
> 2010).

> Los paisajes de la Tierra son esculpidos \[modelados\] por un conjunto
> de procesos geomorfológicos que cambian según la posición en el
> planeta y en el tiempo debido a cambios en el clima. Los paisajes
> contienen “firmas” \[registros\] del **principal proceso activo**, el
> cual “nos \[te\] interesa \[para aprobar o para lo que veas\]”
> aprender a leer (Anderson & Anderson, 2010).

Guarda ésto: “…el principal proceso activo…,” y quédate también con esta
otra cita:

> La Geomorfología, como otras ramas de la ciencia, necesita pasar de la
> simple descripción a la cuantificación y para ello tiene que utilizar
> métodos de otras áreas científicas, fundamentalmente de la Física
> (Gutiérrez Elorza, 2008)

Tricart (1956) aseguraba que la Geomorfología debía apoyarse en el
estudio de los procesos y también en la morfogénesis antrópica. No
porque lo haya dicho él, sino porque la historia reciente le ha dado la
razón: la geomorfología de procesos se ha convertido en la rama
dominante desde mediados del siglo XX hasta la actualidad. Esta rama se
preocupa más por el proceso que por la forma, lo cual la separa de la
evolución de los grandes conjuntos de relieve (Gutiérrez Elorza, 2008).

Dos grupos de procesos geomorfológicos convergen en la superficie del
planeta (Anderson & Anderson, 2010):

1.  Las rocas de la superficie son movidas por procesos geofísicos
    profundos.

2.  La atmósfera es movida por una distribución desigual de la radiación
    solar.

Aunque seguiré un guión de geomorfología de procesos, no olvidaré
aproximaciones geomorfológicas tradicionales que, de otra manera,
quedarían excluidas del programa (e.g. geomorfología litológica y
evolutiva).

La geomorfología de procesos no sería posible sin el avance de los
últimos siglos en matemáticas. Igualmente, sin la irrupción de la
tecnología y el desarrollo de la programación en la segunda mitad del
siglo XX, tampoco sería posible estudiar procesos a escalas grandes.
Estas herramientas han permitido que la geomorfología dé respuestas cada
vez más precisas a problemas de ciencias de la Tierra, como los riesgos
de desastres.

Puedes presuponer que seguiré un esquema de geomorfología de procesos
(to’eta plepla no e’de’barde) en la parte teórica, pero además
introduciré geomorfometría, soporte matemático y aplicaciones
tecnológicas usando software de código abierto, centrando el aprendizaje
en asignaciones sobre geomorfometría y en un manuscrito que escribirás
tú.

**Me apoyaré en [R](https://www.r-project.org/) y en [GRASS
GIS](https://grass.osgeo.org/)** (las vainas del tali), y tienes la
opción de usar Python, o quizá Julia, Javascript o cualquier otro
lenguaje que sepas. Para visualizar salidas, opcionalmente podrás usar
[**QGIS**](https://qgis.org/es/site/) (por ejemplo, en tu propia PC).
Con suerte, y si alcanza el tiempo, verás posibles aplicaciones en
geomorfología de la fotogrametría digital
(e.g. [**OpenDroneMap**](https://www.opendronemap.org/)), de las
técnicas de navegación por satélite para mediciones precisas, y de la
teledetección, especialmente radar.

En cuanto a escribir código, te adelanto que, para superar las
dificultades y los desafíos inherentes de las asignaciones y el
manuscrito, tendrás que:

1.  Contar con el profesor. No te abandonaré a tu suerte al analizar
    datos. No hay horario para pedirme ayuda, y pregunta lo que quieras
    preguntar, yo responderé cuando pueda. Intentaré darte soluciones
    cuando te tranques, pero con la condición de que, antes de
    preguntarme, intentes avanzar soluciones del problema. Lee los
    puntos 3 y 4 más abajo.

2.  Sufrir. Nadie dijo que fajarse con geomorfometría mediante R, GRASS
    GIS o Python fuese placentero. A diferencia de los software de pago,
    aquí no hay un botoncito mágico que lo resuelve todo. Cuesta
    esfuerzo, mucho; eso sí, es gratis, como todas las cosas buenas.
    Además, te obliga a la abstracción y a la resolución de problemas,
    algo que siempre viene bien en términos profesionales y académicos.
    Adelanto también que este mismo principio aplica a la redacción;
    escribir concisamente apoyándote en tus resultados es tarea
    complicada. Por lo tanto, sufre, pero con motivo.

3.  Pedir ayuda. Escríbeme o pide ayuda a tus compañeros y compañeras
    cuando te surjan dudas. Tienes varias alternativas:

    1.  Vía el foro de la asignatura (vía más eficiente y preferida).
    2.  A mi correo: jmartinez19@uasd.edu.do
    3.  Creando *issues* en GitHub.

4.  Al hilo del punto anterior, utilizar estrategias proactivas para
    pedir ayuda. Elimina esta expresión de tu vocabulario: “da error.”
    Con eso nadie podrá ayudarte. Lo importante es informar qué
    intentaste hacer y qué error o problema te surgió. Por ello, cuando
    pidas ayuda, deberás ofrecer un ejemplo reproducible. En la medida
    de lo posible, evita las capturas de pantalla y prefiere código
    reproducible + error. Si la captura de pantalla es el único camino
    que tienes para mostrar tu problema, entonces úsala, pero no olvides
    incluir los dos elementos primordiales: 1) qué intentaste hacer y 2)
    qué error/problema se te presentó. Otras estrategias son: consultar
    posibles soluciones a tu problema en foros ya existentes (como
    stackoverflow), probar alternativas, documentar lo que hiciste,
    explicar qué entiendes que pudo provocar el error. En definitiva,
    sólo pide ayuda cuando realmente te hayas “trancado.”

No tendrás que preocuparte por el hardware (ya me ensucio yo las manos
con esa cosa tan mundana llamada computadora), pero sí ocúpate por
escribir código con sentido, por razonar bien tus asignaciones y,
especialmente, por escribir bien tu manuscrito; escribe que se te
entienda, yo pediré a monesvol para que te ilumine. Dispondrás de un
servidor de RStudio de modestas prestaciones administrado por “yo
mesmamente,” con los paquetes requeridos en el curso ya pre-instalados.
Así podrás realizar tus asignaciones sobre geomorfometría y tu
manuscrito sin preocuparte de instalaciones de software/paquetes. Queda
a opción tuya hacer visualizaciones de datos y mapas usando software de
interfaz gráfica (e.g. QGIS), pero necesitarás instalarlo en tu propia
PC.

Parecería “natural” utilizar interfaz gráfica de usuario para analizar
datos geomorfológicos y hacer análisis geomorfométrico, pero a lo largo
de esta asignatura verás que lo razonable es utilizar código. Realizar
análisis reproducibles de manera eficiente sólo se logra escribiendo y
ejecutando código. Igualmente, para visualizar patrones espaciales se
requiere de herramientas versátiles, que tanto R como otros lenguajes
proveen normalmente a través de paquetes.

## Evaluación

| Ítem                                                       | % de la  nota final |
|------------------------------------------------------------|--------------------:|
| [Manuscrito (basado en datos pre-existentes)](#manuscrito) |                 50% |
| [Presentación oral](#presentación-oral)                    |                 20% |
| [Asignaciones](#asignaciones)                              |                 30% |

Sí sí, lo que viste, no hay examen.

Brevemente, cada ítem a evaluar consistirá en lo siguiente (más detalles
por medio de asignaciones a lo largo del curso):

### Manuscrito

Tratará sobre una cuenca hidrográfica que te asignaré, con especial
énfasis en morfometría, de manera que puedas combinar técnicas de
geocomputación y geomorfometría digital.

Alternativamente, tu manuscrito puede tratar sobre procesos
geomorfológicos en morfosistemas o elementos morfológicos específicos
elegidos por ti. Si eliges este camino, para la selección de tema, debe
existir un interés puntual de tu parte. Hay muchas opciones, elige una
(consulta al profesor, mira en libros y artículos de geomorfología):

1.  Geomorfología tectónica. Algunos ejemplos: deformación, ¿depósitos?
    (difíciles de conseguir), perfiles de ríos afectados.

2.  Ríos. Evolución de canales, distribución de depósitos, inundaciones,
    abanicos aluviales, cuencas.

3.  Vertientes. Debris flows, deslizamientos, geometría de vertientes.

4.  Litorales. Costas rocosas, costas no rocosas, evolución, depósitos.

5.  Formas eólicas. Depósitos, dunas, evolución.

6.  Karst. Morfometría kárstica, procesos, depósitos, evolución.

Con independencia de si tu tema es cuencas hidrográficas, o uno elegido
por ti libremente, elaborarás tu manuscrito siguiendo estas fases:

1.  Formulación del problema/pregunta(s) de investigación, siendo
    preceptiva la sencillez de diseño. Las preguntas de investigación a
    responder las diseñarás tú. Consulta al profesor para construir tus
    preguntas en una sesión de clase, para que las preguntas formuladas
    sean “respondibles” sin caer en simplismos.

2.  Revisión bibliográfica. Busca fuentes en línea, pero evita abrumarte
    con la enorme disponibilidad de publicaciones científicas sobre
    geomorfología. Prefiere las publicaciones disponibles en acceso
    libre, y no olvides el [Sci-Hub](https://sci-hub.se).

3.  Selección de metodología, incluyendo técnicas cuantitativas de forma
    preceptiva.

4.  Recogida de datos, ya fuese un modelo digital de elevaciones (DEM) o
    por levantamientos en campo.

5.  Análisis de datos.

6.  Redacción. Volver eterna y recursivamente a 5 hasta que la redacción
    quede “nítida.”

Los criterios de evaluación que usaré para el manuscrito son:

1.  Cumplimiento de los requisitos exigidos por el [Anuario de
    Investigaciones
    Científicas](https://www.uasd.edu.do/index.php/publicaciones-cientificas)
    de la UASD.

2.  Redacción coherente y concisa.

3.  Resultados, con el debido apoyo estadístico y gráfico, que respondan
    a las preguntas formuladas.

4.  Concisa extracción de conclusiones.

Para preparar tu manuscrito, sigue las normas para autores/as del
[Anuario de Investigaciones Científicas de la
UASD](docs/instrucciones-para-autores-anuario-investigaciones-cientificas-UASD.pdf).
Fungiré como editor ficticio de la revista, e incluso como revisor
(*reviewer \#2*).

-   Como verás, el manuscrito requiere los siguientes ítems:

    -   Título.
    -   Nombre de autor/a.
    -   Resumen y palabras clave.
    -   *Abstract* y *keywords* (optativo).
    -   Introducción
    -   Metodología.
    -   Resultados.
    -   Discusión.
    -   Agradecimientos (optativo).
    -   Referencias citadas.
    -   *Script* reproducible
    -   Declaración de cumplimientos legales y de no conflictos de
        intereses (optativo).
    -   Otros requerimientos (ponle atención también a esta parte en las
        [normas](docs/instrucciones-para-autores-anuario-investigaciones-cientificas-UASD.pdf)).

-   Toma en consideración lo siguiente:

    -   No impartiré lecciones sobre redacción ni sobre procesadores de
        texto, por lo que te recomiendo consultar material tanto vía web
        como en el economato para mejorar dichas capacidades.

    -   El plagio y la falsificación de datos supondrán la reprobación
        inmediata de la asignatura.

    -   Te recomiendo consultar [uno o varios artículos de cualquier
        número del
        Anuario](https://www.uasd.edu.do/index.php/publicaciones-cientificas),
        para que te familiarices con el estilo de redacción.

### Presentación oral

Dispondrás de 15 minutos para presentar oralmente tu trabajo al final
del semestre. Valoraré el dominio que muestres del tema y de tus
resultados.

### Asignaciones

Ocasionalmente, te enviaré asignaciones sobre geomorfometría, que te
ayudarán a manejar herramientas reproducibles en geomorfología. Podrás
realizar tus asignaciones utilizando el servidor RStudio habilitado por
mí (sólo necesitarás una PC con conexión a Internet y un navegador), o
utilizando tu propia PC, pero en este último caso tendrás que instalar
R, RStudio y los paquetes requeridos.

Orientaré con ejemplos y soluciones de forma pública en las sesiones de
clases y en el foro. De esta forma, las discusiones quedan disponibles
para otras personas. Al hacer una consulta, debes plantear el problema
al que te enfrentas, cómo has intentado resolverlo o qué soluciones has
probado. Si se trata de alguna cuestión relacionada con programación o
análisis de datos, deberás facilitar **código reproducible y mensaje de
error (si lo hubiere)**. Cuando escribas tus dudas, no recurras al
típico “da error,” puesto que no conduce a nada. En su lugar prefiere
estas expresiones *“intente este procedimiento … , dio este error, luego
intenté esta solución … pero no consigo dar con el fallo”*.

Prefiere el foro como medio de consulta, porque la discusión que se
genere quedará accesible a las demás personas. Además, el foro te ofrece
múltiples herramientas para formatear tu código, y ¡puedes subir
capturas de pantalla con facilidad!

## Contenido teórico

-   Tema 1. Epistemología, conceptos, bases geológicas e introducción a
    los procesos de la superficie terrestre. Páginas en Gutiérrez
    Elorza (2008): 1 a 45, ambas inclusive. Páginas Anderson &
    Anderson (2010): 1 a 15, ambas inclusive.

-   Tema 2. Tiempo en geomorfología. Técnicas de datación relativas,
    técnicas de datación absoluta. En Gutiérrez Elorza (2008): páginas
    52 a 54, ambas inclusive. En Anderson & Anderson (2010): capítulo 6.

-   Tema 3. Meteorización y formas resultantes. En Gutiérrez
    Elorza (2008): capítulo 5. En Anderson & Anderson (2010):
    capítulo 7.

-   Tema 4. Procesos fluviales. Conceptos básicos de hidrología e
    hidráulica fluvial, procesos fluviales. Formas y depósitos fluviales
    (aluvionamientos, terrazas, diques, barras, etc.), abanicos. En
    Gutiérrez Elorza (2008): capítulos 8 y 9.

-   Tema 5. Procesos de laderas y movimientos en masa. Laderas, balance
    de masa, y otros. Procesos elementales: rainsplash, solifluxión,
    procesos biogeomorfológicos, y otros. Movimientos de masa (procesos
    gravitacionales/de laderas): principios físicos, tipologías (caída,
    deslizamiento, flujo, reptación), debris flow, modelos de
    laderas/morfometría. En Gutiérrez Elorza (2008): capítulo 7.

-   Tema 6. Procesos litorales. Aguas marinas litorales, productos
    característicos de la dinámica litoral. Básicos: conceptos, dinámica
    de las aguas litorales (oleajes, mareas, corrientes). Zonas,
    subzonas, elementos del litoral, productos morfológicos (costas
    arenosas, costas rocosas). En Gutiérrez Elorza (2008): capítulo 11.

-   Tema 7. Geomorfología kárstica. En Gutiérrez Elorza (2008):
    capítulo 6.

-   Tema 8. Geomorfología climática: medios áridos y semi-áridos,
    dominio tropical. En Gutiérrez Elorza (2008): capítulos 12, 16, 17
    y 18.

## Referencias

<div id="refs" class="references csl-bib-body hanging-indent"
line-spacing="2">

<div id="ref-anderson2010geomorphology" class="csl-entry">

Anderson, R. S., & Anderson, S. P. (2010). *Geomorphology: The mechanics
and chemistry of landscapes*. Cambridge University Press.

</div>

<div id="ref-gutierrez2008geomorfologia" class="csl-entry">

Gutiérrez Elorza, M. (2008). *Geomorfologı́a*.

</div>

<div id="ref-tricart1956geomorphologie" class="csl-entry">

Tricart, J. (1956). *La géomorphologie et la pensée marxiste*. La
Pensée.

</div>

</div>
