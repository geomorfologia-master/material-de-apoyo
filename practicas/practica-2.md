Práctica 2. Uso básico de software SIG de código abierto (QGIS + GRASS
GIS + R + Python): derivar productos, estadística zonal.
================
José Ramón Martínez Batlle
29-08-2022

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
    bajo el nombre “OLAYA-Sistemas-de-Informacion-Geografica.pdf.”

-   QGIS Development Team (2022). En el [Drive de la
    asignatura](https://drive.google.com/drive/folders/1orlvmg86kad08FznStkmYaesxaTbzAQD?usp=sharing),
    bajo el nombre
    “QGIS-Guia-de-usuario-version-escritorio-de-QGIS-3.22.pdf.”

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

## Ejercicio 1. Genera información morfométrica a partir de un DEM y simboliza adecuadamente

1.  Obtén

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
