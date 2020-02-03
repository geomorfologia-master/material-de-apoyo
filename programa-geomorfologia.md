
<!-- Este .md fue generado a partir del .Rmd homónimo. Edítese el .Rmd -->

# Programa de “Geomorfología” <br/> Licenciatura en Geografía <br/> Universidad Autónoma de Santo Domingo (UASD)

Enero 2020 <br/> *José Ramón Martínez Batlle*

## Básicos:

  - Correo: <jmartinez19@uasd.edu.do>
  - Lugar y horario: FC-203, Martes de 2 a 6 pm

## URLs del contenido del curso:

  - [Programa (hipervínculo recursivo)](programa-geomorfologia.md)
  - [¿Cómo realizar una asignación?](ref/como-hacer-una-asignacion.md)
  - [Guía mínima de RMarkdown](ref/guia-minima-de-rmarkdown.md)
  - [Introducción a R](ref/introduccion-a-r.md)

## Descripción

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

Guarda ésto: “…el principal proceso activo…”, y quédate también con esta
otra cita:

> La Geomorfología, como otras ramas de la ciencia, necesita pasar de la
> simple descripción a la cuantificación y para ello tiene que utilizar
> métodos de otras áreas científicas, fundamentalmente la Física
> (Gutiérrez Elorza, 2008)

Tricart (1956) aseguraba que la Geomorfología debía apoyarse en el
estudio de los procesos y también en la morfogénesis antrópica. No
porque lo haya dicho él, sino porque la historia reciente le ha dado la
razón: la geomorfología de procesos se ha convertido en la rama
dominante desde mediados del siglo XX hasta la actualidad. Como su
nombre indica, esta rama se preocupa más por el proceso que por la
forma, lo cual deja de lado la evolución de los grandes conjuntos de
relieve (Gutiérrez Elorza, 2008).

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
(to’eta plepla no e’de’barde) en la parte teórica, pero en esta edición
además introduciré geomorfometría, soporte matemático y aplicaciones
tecnológicas usando software de código abierto, centrando el aprendizaje
en asignaciones sobre geomorfometría y en un manuscrito que escribirás
tú.

**Me apoyaré en [R](https://www.r-project.org/) y en [GRASS
GIS](https://grass.osgeo.org/)** (las vainas del tali), y tienes la
opción de usar Python. Para visualizar salidas, opcionalmente podrás
usar [**QGIS**](https://qgis.org/es/site/) (por ejemplo, localmente en
una PC tuya o en las del SIGCART). Con suerte, y si alcanza el tiempo,
verás posibles usos de [**OpenDroneMap**](https://www.opendronemap.org/)
en geomorfología, así como de herramientas fotogramétricas, de
navegación por satélite para mediciones precisas y de teledetección.

En cuanto a escribir código, te adelanto que para superar las
dificultades y los desafíos inherentes de las asignaciones y el
manuscrito, tendrás que:

1.  Sufrir. Nadie dijo que fajarse con geomorfometría con R, GRASS GIS o
    Python fuese placentero. A diferencia de los software de pago, aquí
    no hay un botoncito que lo resuelva todo. Cuesta esfuerzo, mucho;
    eso sí, es gratis, como todas las cosas buenas. Adelanto también que
    este mismo principio aplica a la redacción; escribir con concisión
    apoyándote en tus resultados es tarea complicada. Por lo tanto,
    sufre, pero con un motivo.

2.  Recibir tutorías. Estoy de lunes a jueves, de 8 am a 1 pm en la
    pecera del piso 7 (Facultad de Ciencias) del “Edificio
    Administrativo”. No necesitas cita previa, pero recomiendo que me
    escribas (jmartinez19@uasd.edu.do) por si tuviese compromisos fuera
    el día que elijas visitarme.

3.  Aprender a pedir ayuda. Elimina esta expresión de tu vocabulario:
    “da error”. Con eso nadie podrá ayudarte. Lo importante es qué
    error obtienes al ejecutar qué cosa. Por ello, cuando pidas ayuda,
    por ejemplo, mediante *issues* de GitHub, deberás ofrecer un ejemplo
    reproducible. En la medida de lo posible, evita las capturas de
    pantalla y prefiere código reproducible + error. El *ecrinchó ’ta
    bien pa’guasá* y otras vainas, pero no para pedir ayuda con código
    informático.

No tendrás que preocuparte por el hardware (ya me ensucio yo las manos
con esa cosa tan mundana llamada computadora), pero ocúpate por escribir
código con sentido, por razonar bien tus asignaciones y, especialmente,
por escribir bien tu manuscrito; escribe que se te entienda, yo pediré a
monesvol para que te ilumine. Dispondrás de un servidor de RStudio de
modestas prestaciones habilitado por mí, con los paquetes requeridos en
el curso ya pre-instalados. Así podrás realizar tus asignaciones sobre
geomorfometría y tu manuscrito sin preocuparte de instalaciones de
paquetes.

Parecería “natural” utilizar interfaz gráfico de usuario para analizar
datos geomorfológicos y hacer análisis geomorfométrico, pero a lo largo
de esta asignatura verás que lo razonable es utilizar código. Realizar
análisis reproducibles de manera eficiente sólo se logra escribiendo y
ejecutando código. Igualmente, para visualizar patrones espaciales se
requiere de herramientas versátiles, que tanto R como otros lenguajes
proveen normalmente a través de
paquetes.

## Evaluación

| Ítem                                                   | % de la  nota final |
| ------------------------------------------------------ | ------------------: |
| [Manuscrito (basado en trabajo de campo)](#manuscrito) |                 40% |
| [Presentación oral](#presentación-oral)                |                 10% |
| [Trabajo de campo](#trabajo-de-campo)                  |                 20% |
| [Asignaciones](#asignaciones)                          |                 30% |

Sí sí, lo que viste, no hay examen.

Brevemente, cada ítem a evaluar consistirá en lo siguiente (más detalles
por medio de asignaciones a lo largo del curso):

### Manuscrito

Tratará sobre procesos geomorfológicos en morfosistemas o elementos
morfológicos puntuales, prefiriendo una localidad cercana a Santo
Domingo, de manera que puedas combinar técnicas de geocomputación,
geomorfometría y trabajo de campo. Lo elaborarás siguiendo las
siguientes fases:

1.  Selección del tema. Hay muchas opciones, pero elige una (consulta al
    profesor, libros y artículos de geomorfología):
    1.  Geomorfología tectónica. Algunos ejemplos: deformación,
        ¿depósitos? (difíciles de conseguir), perfiles de ríos
        afectados.
    2.  Ríos. Evolución de canales, distribución de depósitos,
        inundaciones, abanicos aluviales, cuencas.
    3.  Vertientes. Debris flows, deslizamientos, geometría de
        vertientes.
    4.  Litorales. Costas rocosas, costas no rocosas, evolución,
        depósitos.
    5.  Formas eólicas. Depósitos, dunas, evolución.
2.  Formulación del problema/pregunta(s) de investigación, siendo
    preceptiva la sencillez de diseño. Las preguntas de investigación a
    responder las diseñarás tú. Consulta al profesor para construir tus
    preguntas en una sesión de clase, para que las preguntas formuladas
    sean “respondibles” sin caer en simplismos.
3.  Revisión bibliográfica. Busca fuentes en línea, pero evita abrumarte
    con la enorme disponibilidad de publicaciones científicas sobre
    geomorfología. Prefiere las publicaciones disponibles en acceso
    libre.
4.  Selección de metodología, incluyendo técnicas cuantitativas de forma
    preceptiva.
5.  Recogida de datos de campo.
6.  Análisis de datos.
7.  Redacción.

Los criterios de evaluación que usaré para el manuscrito son:

1.  Cumplimiento de los requisitos exigidos por el Anuario, tanto los de
    forma (estilos de documento) como los de fondo.
2.  Redacción coherente y concisa.
3.  Resultados, con el debido apoyo estadístico y gráfico, que respondan
    a las preguntas formuladas.
4.  Concisa extracción de conclusiones. Los resultados negativos son
    igualmente válidos.

Para preparar tu manuscrito, sigue las normas para autores/as del
[Anuario de Investigaciones Científicas de la
UASD](docs/instrucciones-para-autores-anuario-investigaciones-cientificas-UASD.pdf).
Fungiré como editor ficticio de la revista, e incluso como revisor.

  - Como verás, el manuscrito requiere los siguientes ítems:
      - Título.
      - Nombre de autor/a.
      - Resumen y palabras clave.
      - *Abstract* y *keywords* (optativo).
      - Metodología.
      - Resultados.
      - Discusión.
      - Agradecimientos (optativo).
      - Referencias citadas.
      - Declaración de cumplimientos legales y de no conflictos de
        intereses (optativo).
      - Otros requerimientos (ponle atención también a esta parte en las
        [normas](docs/instrucciones-para-autores-anuario-investigaciones-cientificas-UASD.pdf)).

Toma en consideración lo siguiente: \* No impartiré lecciones sobre
redacción ni sobre procesadores de texto, por lo que se recomienda
consultar material tanto vía web como en el economato, como forma de
mejorar dichas capacidades. \* El plagio y la falsificación de datos
supondrán la reprobación inmediata de la asignatura. \* Te recomiendo
consultar [uno o varios artículos de cualquier número del
Anuario](https://www.uasd.edu.do/index.php/publicaciones-cientificas),
para que te familiarices con el estilo de redacción.

### Presentación oral

Dispondrás de 15 minutos para presentar oralmente tu trabajo al final
del semestre. Valoraré el dominio que muestres del tema y de tus
resultados.

### Trabajo de campo

Dependerá mucho del tema que elijas. En todo caso, incluirá recogida de
datos que posteriormente puedan procesarse informáticamente.

### Asignaciones

Te enviaré asignaciones sobre geomorfometría por correo electrónico, que
te ayudarán a manejar herramientas reproducibles en geomorfología.
Podrás realizar tus asignaciones utilizando el servidor RStudio
habilitado por mí (sólo necesitarás una PC con conexión a Internet y un
navegador), o utilizando tu propia PC, pero en este último caso tendrás
que instalar R, RStudio y los paquetes requeridos.

Orientaré con ejemplos y soluciones de forma pública a través de
*issues* que abrirás en el GitHub. De esta forma las discusiones quedan
disponibles para otras personas. Al abrir un *issue* de GitHub debes
plantear el problema al que te enfrentas, cómo has intentado resolverlo
o qué soluciones has probado. Si se trata de cuestión relacionada con
programación o análisis de datos, deberás facilitar **código
reproducible y mensaje de error (si lo hubiere)**. Cuando escribas tus
dudas, no recurras al típico “da error”, puesto que no conduce a nada.

Evita preguntar por correo electrónico, porque cualquier consulta que
realices, así como las posibles soluciones que surjan, quedarán en
privado y sólo serán aprovechables por ti.

## Contenido teórico

  - Tema 1. Epistemología, conceptos, bases geológicas. Geomorfología
    estructural Definición de geomorfología, disciplinas auxiliares,
    epistemología, métodos Estructura y composición del interior de la
    Tierra, rocas (rocas comunes en RD), placas y límites de placa
    (reflejo de la tectónica de placas en el Caribe, deformaciones),
    fallas, pliegues, diaclasas. Páginas en Gutiérrez Elorza (2008): 1 a
    45, ambas inclusive.

  - Tema 2. Meteorización y tiempo en geomorfología. Técnicas de
    datación relativas, técnicas de datación absoluta. En Gutiérrez
    Elorza (2008): capítulo 5 y páginas 52 a 54, ambas inclusive.

  - Tema 3. Procesos fluviales. Conceptos básicos de hidrología e
    hidráulica fluvial, procesos fluviales. Formas y depósitos
    fluviales (aluvionamientos, terrazas, diques, barras, etc.),
    abanicos. En Gutiérrez Elorza (2008): capítulos 8 y 9.

  - Tema 4. Procesos de laderas y movimientos en masa. Laderas, balance
    de masa, y otros. Procesos elementales: rainsplash, solifluxión,
    procesos biogeomorfológicos, y otros. Movimientos de masa (procesos
    gravitacionales/de laderas): principios físicos, tipologías (caída,
    deslizamiento, flujo, reptación), debris flow, modelos de
    laderas/morfometría. En Gutiérrez Elorza (2008): capítulo 7.

  - Tema 5. Procesos litorales. Aguas marinas litorales, productos
    característicos de la dinámica litoral. Básicos: conceptos, dinámica
    de las aguas litorales (oleajes, mareas, corrientes). Zonas,
    subzonas, elementos del litoral, productos morfológicos (costas
    arenosas, costas rocosas). En Gutiérrez Elorza (2008): capítulo 11.

  - Tema 6. Geomorfología kárstica. En Gutiérrez Elorza (2008): capítulo
    6.

  - Tema 7. Geomorfología climática: medios áridos y semi-áridos,
    dominio tropical. En Gutiérrez Elorza (2008): capítulos 12, 16, 17 y
    18.

## Referencias

<div id="refs" class="references">

<div id="ref-anderson2010geomorphology">

Anderson, R. S., & Anderson, S. P. (2010). *Geomorphology: The mechanics
and chemistry of landscapes*. Cambridge University Press.

</div>

<div id="ref-gutierrez2008geomorfologia">

Gutiérrez Elorza, M. (2008). *Geomorfologı'a*.

</div>

<div id="ref-tricart1956geomorphologie">

Tricart, J. (1956). *La géomorphologie et la pensée marxiste*. La
Pensée.

</div>

</div>
