Introducción a software SIG de código abierto (QGIS + GRASS GIS + R +
Python) aplicados a la cartografía geomorfológica.
================
José Ramón Martínez Batlle

# Introducción

Desde su origen en el siglo pasado, los sistemas de información
geográfica (SIG) han experimentado una larga evolución. Diría que la
confusión más común entre usuarios ha sido el confundir los SIG con los
software; este último es una pieza (importante) del primero, pero no lo
único, porque también se incluyen los usuarios, los datos y modelos, el
hardware, las fuentes, entre otros elementos (Olaya, 2020).

Lo que hoy conocemos como software SIG está en crisis. La irrupción del
software como servicio en el mercado, ha provocado muchas aplicaciones
se ofrezcan en la nube, relegando así la tradicional aplicación de
escritorio. Trabajar en la nube tiene muchas ventajas, una de las más
importantes es que se reduce el riesgo de fallos en la aplicación (o al
menos se pueden corregir con mayor facilidad), se elimina la necesidad
de una instalación previa (el “infierno de dependencias” desaparece), y
ofrecen la posibilidad de conectar con bases de datos grandes y
diversas. Entre las desventajas, las más importante es que, como
usuarios, perdemos libertad, puesto que cada vez estamos más atados a la
nube para hacer nuestro trabajo. Asimismo, aunque se trate de software
de código abierto, mucho software ofrecido como servicio en la nube
termina convirtiéndose en una cuota mensual más a nuestra factura.

Mientras nos preparamos para ese “promisorio futuro”, todavía tenemos la
posibilidad de hacer análisis en la PC propia. Tratándose de
geomorfología, los software SIG son fundamentales para nuestros
análisis, sobre todo para realizar cartografía del relieve de forma
masiva.

En esta práctica examinarás cuatro herramientas fundamentales, algunas
de las cuales quizá ya las conoces. Comenzarás desde lo básico, la
instalación, posteriormente deberás conocer la interfaz gráfica de QGIS
y de GRASS GIS, y te introducirás en los lenguajes de programación R y
Python. En todos los casos aplicarás estas herramientas a ejemplos muy
básicos sobre cartografía geomorfológica.

# Objetivos de aprendizaje

Al terminar esta práctica deberías ser capaz de:

-   Instalar y poner en marcha software de SIG en una PC.

-   Cargar distintas fuentes, tanto rásters como vectoriales.

-   Aplicar simbología.

-   Derivar productos a partir de un modelo digital de elevaciones
    (DEM).

-   Extraer información geomorfológica a partir de un DEM y conservarla
    en un archivo vectorial.

-   Generar e interpretar un mapa de geomórfonos.

# Lecturas previas recomendadas

-   Olaya (2020), páginas 1- de la versión PDF

# 

# Referencias

<div id="refs" class="references csl-bib-body hanging-indent"
line-spacing="2">

<div id="ref-olaya2014sistemas" class="csl-entry">

Olaya, V. (2020). *<span class="nocase">Sistemas de Informaci<span
class="nocase">ó</span>n Geogr<span class="nocase">á</span>fica. Un
libro libre de V<span class="nocase">í</span>ctor Olaya</span>*.
Retrieved from <https://volaya.github.io/libro-sig/>

</div>

</div>
