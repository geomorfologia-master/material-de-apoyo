Práctica 3. Colecta y procesamiento de datos GNSS <br> Asignatura
Geomorfología, UASD
================
José Ramón Martínez Batlle
14-11-2022

# Fecha de entrega

- 21 de noviembre de 2022

# Introducción

Desde la navegación a estima (dead reckoning), basada en una posición
previa conocida, la humanidad ha avanzado enormemente en las técnicas de
navegación y posicionamiento. El recurso más eficiente disponible en la
actualidad para el posicionamiento global preciso, son los sistemas de
navegación por satélite. Las versiones con cobertura global de estos
sistemas, se denominan sistemas de navegación global por satélite o
“GNSS” (siglas de **Global Navigation Satellite Systems**), y la
modalidad que provee coordenadas precisas al instante se denomina
“navegación cinética satelital en tiempo real” o “GNSS-RTK” o,
simplemente, “RTK”. Tanto la tecnología GNSS en general, como su
modalidad RTK, son muy útiles en aplicaciones de geografía física
(especialmente en geomorfología), agrimensura, topografía, agricultura
de precisión, entre otras disciplinas.

En esta práctica instalarás y utilizarás recursos de software y hardware
para iniciarte en la tecnología GNSS desde cero. Específicamente, verás
software de código abierto para procesamiento de datos GNSS y
representación de soluciones (RTKLIB, QGIS, GoogleEarth),

# Objetivos de aprendizaje

Al terminar esta práctica deberías ser capaz de:

- Colectar datos en terreno con un receptor GNSS DIY de bajo costo.

- Reconocer algunos formatos de datos GNSS.

- Aplicar herramientas de código abierto para procesamiento de datos
  GNSS.

- Generar soluciones fijas por posproceso.

# Lecturas previas recomendadas, preparación, recursos disponibles

- (Jeffrey, 2010)

- Demostraciones en aula.

# Informe

Entregarás tu informe en formato PDF, el cual podrás elaborar con tu
procesador de texto favorito (por ejemplo, LibreOffice Writer, LaTeX,
Word) o mediante entornos de desarrollo integrado (e.g. Atom, Visual
Studio Code, Jupyter Notebooks, RMarkdown-RStudio). Características del
documento:

- Número máximo de páginas: 10.

- En la primera página, deberás incluir nombre, matrícula, asignatura,
  nombre de la práctica, fecha.

- Para evitar la proliferación de tipografías y formatos, debes usar
  estilos. Lo más fácil es basarse en plantillas. Hay muchos recursos en
  la web sobre cómo usar estilos (término de búsqueda recomendado:
  estilos en procesadores de texto).

- En los casos que aplique, debes incluir tu código informático en las
  respuestas de los ejercicios donde uses lenguajes de programación
  (e.g. R, Python). El código debe ser incluido como texto, no como
  imagen (e.g. captura de pantalla).

- Realiza doble revisión de ortografía y gramática.

- Las páginas deben estar numeradas.

- Si aplica, incluir ilustraciones y tablas de apoyo (a ambas debes
  incluirles título, “*caption*”), así como lista de referencias
  bibliográficas. Sólo incluye figuras que refieras en el texto.

- Puedes usar un apéndice para incluir información complementaria que no
  te quepa en las 10 páginas centrales.

- Podré solicitar los archivos fuente empleados para elaborar el PDF y
  los resultados intermedios generados en cada ejercicio.

# Criterios de evaluación

| Concepto                                                                                                                    | Porcentaje |
|:----------------------------------------------------------------------------------------------------------------------------|:-----------|
| Redacción, que incluye organización de las ideas, gramática, ortografía                                                     | 60%        |
| Presentación, que incluye uso apropiado de estilos, tablas y figuras (legibilidad, uso de *caption*), numeración de páginas | 40%        |

# Ejercicios

## Ejercicio 1. Colecta tus datos en terreno

¡Hecho! Si quieres, puedes incluir tu foto de campo en esta sección.
Verás la que te tomé (guardada con tu nombre) en esta ruta del repo:
`data/d003/fotos/`

## Ejercicio 2. Instala software

Instala los siguientes programas:

1.  Instala u-center2 y u-center v22.07 (de u-blox) desde
    <https://www.u-blox.com/en/product/u-center>. Abre ambos programas.

2.  Descarga los ejecutables del fork demo5 de RTKBLIB desde
    <https://github.com/rtklibexplorer/RTKLIB/releases/download/b34g/demo5_b34g.zip>

3.  QGIS y Google Earth Pro si aún no los tienes. ¿Aún no los tienes?
    Mejor no me respondas, no quiero saber. Abre ambos programas.

4.  Redimensiona las ventanas para que quepan todas en la pantalla.
    Captura la pantalla con todos los programas abierto y pégala en tu
    informe.

5.  Describe el proceso de instalación en cada caso.

## Ejercicio 3. Explora tu archivo con software propietario

1.  Descarga el contenido de la carpeta `data/d003/` de este repo. La
    mejor forma de hacerlo es descargando el repo, mediante el botón
    verde `Code` que se encuentra en la
    [raíz](https://github.com/geomorfologia-202202/material-de-apoyo).
    La misma estructura que veas en GitHub, la tendrás replicada en el
    comprimido que descargues.

2.  Los datos que colectaste en campo se denominan “observaciones del
    rover”. Cada estudiante tiene sus propias observaciones, y se
    encuentran en un archivo de extensión `.ubx`, con el nombre de cada
    quien, dentro del comprimido `rover.zip`, que se encuentra en
    `data/d003/` (importante: Windows normalmente oculta las extensiones
    de los archivos). Extrae tu archivo fuera del comprimido.

3.  Abre y explora tus datos con los dos programas u-center.

4.  Abre y explora tus observaciones del rover con RTKPLOT de RTKLIB.
    Puedes abrir esta herramienta mediante el lanzador de aplicaciones
    de RTKLIB, el cual puedes arrancar haciendo doble-clic en
    `rtklaunch.exe`.

5.  Describe el proceso de exploración, y destaca alguna observación
    particular que demuestre que abriste y exploraste tu archivo
    asignado. Coloca alguna captura de pantalla.

## Ejercicio 4. Genera una solución fija por posproceso

1.  En el ejercicio anterior, exploraste tus observaciones del rover.
    Ahora localiza el archivo de observaciones brutas de la base
    (`.obs`) y el archivo de mensajes de navegación (`.nav`),
    localizados dentro del comprimido `base.zip`, que se encuentra en
    `data/d003/`. Extrae ambos archivos fuera del comprimido.

2.  Extrae y abre los PDF que se encuentran en el comprimido
    `coordenadas-base-conf.zip` de la carpeta \`data/d003/. Estos
    contienen las coordenadas de la base en formato ITRF2014 y WGS84.
    Explorálos.

3.  Extrae y abre el archivo de configuración `.conf` que se encuentra
    en el comprimido `coordenadas-base-conf.zip` de la carpeta
    `data/d003/`. Lo necesitarás más adelante.

4.  Mediante la lanzador de programas de RTKLIB (`rtklaunch.exe`), abre
    el programa RTKPOST.

5.  Realiza el posproceso tal como muestro en el vídeo, obteniendo un
    archivo `.pos`. Aquí verás las coordenadas, así como estadísticos
    básicos de las mismas.

6.  BONUS: calcula, por tu cuenta, la desviación estándar y el error
    estándar de las componentes latitud, longitud y altura.

7.  Describe el proceso realizado en un párrafo.

# Referencias

<div id="refs" class="references csl-bib-body hanging-indent"
line-spacing="2">

<div id="ref-jeffrey2010" class="csl-entry">

Jeffrey, C. (2010). *An introduction to GNSS: GPS, GLONASS, galileo and
other global navigation satellite systems*. Retrieved from
<https://novatel.com/an-introduction-to-gnss>

</div>

</div>
