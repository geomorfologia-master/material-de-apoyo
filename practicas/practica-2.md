Práctica 2. Uso básico de software SIG de código abierto (QGIS + GRASS
GIS + R + Python): derivar productos, estadística zonal, simbología.
================
José Ramón Martínez Batlle
03-\|0-2022

# Fecha de entrega

-   14 de octubre de 2022

# Introducción

Desde su origen en el siglo pasado (sin considerar momentáneamente los
orígenes de la cartografía), los sistemas de información geográfica
(SIG) han experimentado una densa evolución. Diría que la confusión más
común entre usuarios ha sido el asociar SIG con el software que nos dan
acceso a ellos propiamente. Aunque el software es una pieza (importante)
de los SIG, no es lo único ni lo que los define, puesto que también se
incluyen los usuarios, los datos y modelos, el hardware, las fuentes,
entre otros elementos (Olaya, 2020).

# Objetivos de aprendizaje

Al terminar esta práctica deberías ser capaz de:

-   Cargar distintas fuentes (rásters, vectoriales y delimitados).

-   Aplicar simbología.

-   Derivar productos a partir de un modelo digital de elevaciones
    (DEM).

-   Extraer información geomorfológica a partir de un DEM y conservarla
    en un archivo vectorial.

-   Generar e interpretar un mapa de geomórfonos.

# Lecturas previas recomendadas, preparación, recursos disponibles

-   Olaya (2020), páginas 1-28 de la versión PDF. En el [Drive de la
    asignatura](https://drive.google.com/drive/folders/1orlvmg86kad08FznStkmYaesxaTbzAQD?usp=sharing),
    bajo el nombre “OLAYA-Sistemas-de-Informacion-Geografica.pdf”.

-   QGIS Development Team (2022). En el [Drive de la
    asignatura](https://drive.google.com/drive/folders/1orlvmg86kad08FznStkmYaesxaTbzAQD?usp=sharing),
    bajo el nombre
    “QGIS-Guia-de-usuario-version-escritorio-de-QGIS-3.22.pdf”.

-   GRASS Development Team (2022). Disponible sólo en línea. Ver vínculo
    en [Referencias](#referencias)

-   Wickham & Grolemund (2019). Capítulos 1 a 7. Ver vínculo en
    [Referencias](#referencias)

-   Martínez-Batlle (2022). Específicamente, leer el tutorial
    “Introducción a R, simple features y análisis exploratorio de datos
    espaciales (ESDA)” (vínculo en [Referencias](#referencias)).

-   Demostraciones en aula.

# Informe

Entregarás tu informe en formato PDF, el cual podrás elaborar con tu
procesador de texto favorito (por ejemplo, LibreOffice Writer, LaTeX,
Word) o mediante entornos de desarrollo integrado (e.g. Atom, Visual
Studio Code, Jupyter Notebooks, RMarkdown-RStudio). Características del
documento:

-   Número máximo de páginas: 10.

-   En la primera página, deberás incluir nombre, matrícula, asignatura,
    nombre de la práctica, fecha.

-   Para evitar la proliferación de tipografías y formatos, debes usar
    estilos. Lo más fácil es basarse en plantillas. Hay muchos recursos
    en la web sobre cómo usar estilos (término de búsqueda recomendado:
    estilos en procesadores de texto).

-   Debes incluir tu código informático en las respuestas de los
    ejercicios donde uses lenguajes de programación (e.g. R, Python). El
    código debe ser incluido como texto, no como imagen (e.g. captura de
    pantalla).

-   Realiza doble revisión de ortografía y gramática.

-   Las páginas deben estar numeradas.

-   Si aplica, incluir ilustraciones y tablas de apoyo (a ambas debes
    incluirles título, “*caption*”), así como lista de referencias
    bibliográficas.

-   Puedes usar un apéndice para incluir información complementaria que
    no te quepa en las 10 páginas centrales.

-   Podré solicitar los archivos fuente empleados para elaborar el PDF y
    los resultados intermedios generados en cada ejercicio.

# Criterios de evaluación

| Concepto                                                                                                                    | Porcentaje |
|:----------------------------------------------------------------------------------------------------------------------------|:-----------|
| Redacción, que incluye organización de las ideas, gramática, ortografía                                                     | 60%        |
| Presentación, que incluye uso apropiado de estilos, tablas y figuras (legibilidad, uso de *caption*), numeración de páginas | 40%        |

# Ejercicios

## Ejercicio 1. Extrae estadísticos descriptivos

1.  Localiza la capa ráster `gtopo_30_arcsec.tif`, que es el DEM GTOPO30
    (“30” se refiere al “espaciado”, de 30 arco-segundos), el cual
    descargué para ti por medio del
    [EarthExplorer](https://earthexplorer.usgs.gov/)). Localiza tu capa
    vectorial en la lista de capas asignadas de la práctica 1,
    [aquí](practica-1.md#1a-instala-y-prueba-qgis); recuerda que las
    capas vectoriales se encuentran en el subdirectorio `d001` del
    directorio `data` del repo de [material de
    apoyo](https://github.com/geomorfologia-202202/material-de-apoyo),
    que es el repo desde donde, de hecho, estás leyendo este texto.
    Descarga dichos archivos a tu PC y, mediante dos
    software<sup>(1)</sup> de los instalados en la práctica 1, extrae
    los siguientes estadísticos descriptivos de la elevación:

-   Media
-   Mediana
-   Desviación estándar
-   Varianza
-   Valor mínimo
-   Valor máximo

<sup>(1)</sup>Sólo puedes combinar los dos software la siguiente
manera: - QGIS con Python. - GRASS GIS con R

2.  Describe el procedimiento mediante un párrafo y auxiliándote de,
    máximo, dos capturas de pantalla.

3.  En un párrafo, compara el resultado obtenido a partir de cada uno de
    los dos software usados. Reflexiona al respecto sobre las
    diferencias o similitudes encontradas.

Te regalo 10 puntos adicionales si respondes esta pregunta: ¿Es
significativamente diferente el promedio de elevación de tu provincia
respecto del de la provincia contenida en la capa `HE0jF91U.gpkg`.

## Ejercicio 2. Genera información morfométrica a partir de un DEM y simboliza adecuadamente

1.  Obtén, mediante R o Python, el promedio de la pendiente, orientación
    (*aspect*), TPI y TRI de tu provincia. Para ello, necesitarás usar
    funciones que crean estos derivados a partir del DEM.

2.  Describe el procedimiento mediante un párrafo y auxiliándote de,
    máximo, dos capturas de pantalla.

Te regalo 10 puntos adicionales si generas estos mismos derivados desde
QGIS o GRASS GIS (aparte de en R o en Python).

## Ejercicio 3. Aplica simbología apropiadamente al ráster y al vectorial

1.  En GRASS GIS o en QGIS, aplica una simbología apropiada para lograr
    que, de manera conjunta, el lienzo de mapa muestre el DEM dentro de
    la provincia coloreado de acuerdo a la elevación sobre el mapa de
    sombras y la provincia; fuera de la provincia debes hacer visible el
    mismo DEM (duplicándolo) pero sólo en modo sombras. Adicionalmente,
    añade alguna capa web de referencia territorial, por ejemplo,
    OpenStreetMap. Toma en cuenta que …

    -   Las elevaciones deben colorearse de acuerdo al rango valores de
        tu provincia. Tendrás que recortar el DEM al ámbito de tu
        provincia (puedes hacerlo cortándolo efectivamente o usando un
        ráster virtual).

    -   Las capas superiores no pueden ocultar a las inferiores. Deberás
        usar modos de mezcla apropiados (algunas personas prefieren usar
        la transparencia, pero no se basa en el mismo principio).

    -   EL límite de la provincia debe estar visible, pero también el
        interior de misma (relleno) debe destacarse con alguna
        coloración, por lo que también deberás usar un modo de mezcla
        apropiado. También sería apropiado destacar las elevaciones y
        las sombras sólo en el interior de la provincia usando “Polígono
        invertido”.

2.  Describe, en un párrafo, la topografía de tu provincia. Usa tus
    habilidades de descripción geográfica, por ejemplo, rangos de
    elevación, sectores con mayores o menores elevaciones o donde se
    concentran los áreas altas y bajas, si las hubiere.

## Ejercicio 4. Genera una capa de geomórfonos y extrae las proporciones de cada geomórfono dentro de la provincia

1.  Usando GRASS GIS o QGIS, podrás generar los geomórfonos sólo de tu
    provincia.

2.  Extrae, con GRASS GIS o QGIS, las proporciones de cada geomórfono.

3.  Describe, en un párrafo, la distribución de los geomórfonos.

# Referencias

<div id="refs" class="references csl-bib-body hanging-indent"
line-spacing="2">

<div id="ref-grass2022grass" class="csl-entry">

GRASS Development Team. (2022). *GRASS GIS 8.0.3dev Reference Manual*.
<https://grass.osgeo.org/grass80/manuals/index.html>.

</div>

<div id="ref-jose_ramon_martinez_batlle_2022_7028143" class="csl-entry">

Martínez-Batlle, J. R. (2022). <span
class="nocase">maestria-geotel-master/material-de-apoyo: First
release</span> (Version v0.0.0.9000).
<https://doi.org/10.5281/zenodo.7028143>

</div>

<div id="ref-olaya2020sistemas" class="csl-entry">

Olaya, V. (2020). *<span class="nocase">Sistemas de Informaci<span
class="nocase">ó</span>n Geogr<span class="nocase">á</span>fica. Un
libro libre de V<span class="nocase">í</span>ctor Olaya</span>*. Versión
en línea: <https://volaya.github.io/libro-sig/>. Versión PDF:
<https://github.com/volaya/libro-sig/releases/download/v3.0/Sistemas.de.Informacion.Geografica.pdf>.

</div>

<div id="ref-qgis2022qgis" class="csl-entry">

QGIS Development Team. (2022). *QGIS Desktop 3.22 User Guide*. Versión
en línea: <https://docs.qgis.org/3.22/es/docs/user_manual/>. Versón PDF:
<https://docs.qgis.org/3.22/pdf/es/QGIS-3.22-DesktopUserGuide-es.pdf>.

</div>

<div id="ref-Wickham2019Res" class="csl-entry">

Wickham, H., & Grolemund, G. (2019). *R para ciencia de datos*.
Retrieved from <https://es.r4ds.hadley.nz/>

</div>

</div>
