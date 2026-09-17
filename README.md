PA02 · Geomorfometría<small><br>Geomorfología (GEO-114)<br>Universidad
Autónoma de Santo Domingo (UASD)</small>
================
El Tali
2026-09-01

<!-- README.md se genera a partir de README.Rmd. Por favor, edita este archivo. -->

Versión HTML (quizá más legible),
[aquí](https://geomorfologia-master.github.io/geomorfometria/README.html)

# Fecha/hora de entrega

**VER PORTAL DE LA ASIGNATURA**

# Propósito de la práctica

La geomorfometría no consiste simplemente en producir mapas de
pendiente, curvatura o acumulación de flujo. Consiste en **medir y
analizar cuantitativamente la superficie terrestre**, reconocer patrones
del relieve, evaluar cómo dependen de la escala y de los datos
empleados, y utilizar esas mediciones para responder preguntas
geomorfológicas (Florinsky, 2016; Hengl y Reuter, 2009; Wilson, 2018).

En esta práctica desarrollarás una **pequeña investigación
geomorfométrica**. Elegirás una pregunta entre las sugeridas más abajo
—o propondrás otra equivalente—, obtendrás datos públicos, ejecutarás un
flujo de análisis con software adecuado, producirás evidencia
cuantitativa y redactarás un **minimanuscrito científico**.

El producto principal **no es el mapa ni el código por separado: es el
manuscrito**, respaldado por un análisis que otra persona pueda
comprender, ejecutar y auditar. Las competencias de reproducibilidad,
redacción científica, estilos de formato, elaboración de figuras y
tablas, y gestión de citas y referencias, trabajadas previamente, se
consideran en esta práctica **competencias acumulativas ya adquiridas**:
deberás aplicarlas de manera autónoma, pero no constituyen el tema de la
PA02.

> **IMPORTANTE · IA bajo auditoría.** Puedes usar herramientas de
> inteligencia artificial como apoyo, tutor, depurador o interlocutor.
> Sin embargo, deberás identificar y demostrar durante la defensa **al
> menos un error, limitación, simplificación indebida o afirmación no
> verificada producida por una IA durante tu trabajo**, ya sea de
> carácter técnico, conceptual, bibliográfico o epistemológico. No se
> acepta como demostración una afirmación genérica como “la IA puede
> equivocarse”: debes conservar evidencia concreta y explicar cómo
> verificaste o corregiste el problema.

# Objetivos

Al finalizar la práctica deberás demostrar o mejorar tus capacidades
para:

- formular una **pregunta geomorfométrica concreta y realizable**;
- obtener, documentar y preparar un DEM u otras fuentes topográficas
  públicas;
- calcular e interpretar parámetros, objetos o clases del relieve;
- analizar cuantitativamente patrones y relaciones del relieve para
  responder una pregunta geomorfológica;
- reconocer que los resultados pueden depender del **DEM, resolución
  espacial, escala de análisis, algoritmo, parámetros y
  preprocesamiento**;
- comparar críticamente resultados obtenidos bajo distintas escalas,
  fuentes de datos, algoritmos o parámetros, cuando la pregunta lo
  requiera;
- trabajar con herramientas reales de geomorfometría y SIG,
  seleccionando las más adecuadas para el problema;
- interpretar los resultados en términos geomorfológicos y reconocer sus
  limitaciones;
- identificar las limitaciones del trabajo de escritorio, indicando qué
  aspectos mejoraría si se incluyese colecta de datos en terreno y
  verificación de campo;
- aplicar de manera autónoma, en el minimanuscrito y su defensa, las
  competencias previamente adquiridas de reproducibilidad, redacción
  científica, elaboración de figuras y tablas, y gestión de citas y
  referencias;
- auditar críticamente el uso de inteligencia artificial.

# Entregables

> **Competencias acumulativas.** A partir de esta práctica se da por
> supuesto el dominio básico de RMarkdown, estructura de manuscrito,
> estilos de formato, figuras, tablas, citas y referencias trabajado
> previamente. Estos elementos siguen siendo requisitos de calidad de la
> entrega, pero la **materia nueva y el foco temático de la PA02 es la
> geomorfometría**. En esta práctica, usarás el estilo APA como estilo
> de documento y sistema de citación.

> **Nota sobre el estilo APA.** El estilo APA no se limita a un sistema
> de citación bibliográfica, sino que constituye un **estilo editorial
> para la preparación y presentación de documentos académicos**. Sus
> normas abarcan, entre otros aspectos, la estructura del manuscrito,
> los niveles de encabezados, la presentación de tablas y figuras y
> determinadas convenciones tipográficas y de formato. **Dentro de este
> estilo general se encuentra el estilo APA de citas y referencias**,
> que establece específicamente cómo se reconocen las fuentes en el
> texto y cómo se construye la lista de referencias. Por tanto, en esta
> práctica, cuando se solicite un *manuscrito en estilo APA*, se
> entenderá que deben seguirse tanto las normas generales de
> presentación del documento como, de manera particular, las
> correspondientes a citas y referencias. Pero no te estreses por este
> aspecto, porque el archivo plantilla.Rmd ya contiene la estructura y
> formato correctos, y solo deberás adaptarlo a tu investigación.

Debes generar **tres productos obligatorios**.

## 1. Manuscrito reproducible

Entrega un manuscrito breve generado desde **RMarkdown**. El archivo
fuente `.Rmd`, el PDF final, la bibliografía y el código necesario deben
encontrarse en tu repositorio.

Para elaborar el manuscrito, utiliza como punto de partida el archivo
**`plantilla.Rmd` incluido en este repositorio**, preparado para generar
un manuscrito en formato APA 7. La plantilla contiene ejemplos de
estructura, citas y referencias, tablas, figuras y referencias cruzadas.
**Debes modificarla y adaptarla a tu investigación**, eliminando los
textos, datos, figuras y ejemplos demostrativos que no formen parte de
tu trabajo. El manuscrito final deberá compilarse a PDF desde dicho
archivo y poder regenerarse a partir del contenido del repositorio.

> **Importante:** `plantilla.Rmd` es una plantilla didáctica, no un
> manuscrito parcialmente resuelto. Los ejemplos incluidos —entre ellos
> tablas, figuras, datos de demostración y texto orientativo— sirven
> únicamente para mostrar cómo construir el documento. **Ningún ejemplo
> que no corresponda a tu investigación debe permanecer en el manuscrito
> entregado.**

**Extensión sugerida:** 5–9 páginas, sin contar referencias ni material
suplementario.

El manuscrito debe contener, como mínimo:

- título;
- título corto (se coloca en la cabecera de cada página; en
  `plantilla.Rmd` se coloca dentro de la macro `\shorttitle`)
- autor/a;
- resumen y palabras clave;
- introducción;
- materiales y métodos;
- resultados;
- discusión;
- conclusiones;
- referencias;
- declaración breve de reproducibilidad;
- nota breve de auditoría de IA;
- opcionalmente, información suplementaria.

## 2. Diapositivas

Prepara una presentación breve, preferentemente de **8–10
diapositivas**, centrada en la pregunta, el método, la evidencia
principal, la interpretación y las limitaciones.

## 3. Defensa oral

Realizarás una defensa oral de **7 minutos**. Debes poder explicar:

- qué pregunta intentaste responder;
- por qué tu procedimiento geomorfométrico era adecuado;
- qué datos utilizaste y qué representan realmente;
- cuáles fueron las decisiones de escala, algoritmo y parámetros;
- qué muestran tus resultados;
- cuáles son las principales limitaciones;
- qué error o limitación concreta detectaste en el uso de IA.

# Mandato

## 1. Elige una pregunta, no sólo una herramienta

Selecciona **uno** de los temas sugeridos en la tabla de esta práctica o
propón otro de dificultad equivalente (consulta con el profesor si
tienes dudas).

Tu trabajo debe formular una pregunta que pueda responderse con
evidencia. Por ejemplo, **“¿cómo cambia la clasificación de formas del
terreno al variar la escala de búsqueda?”** es una pregunta adecuada;
**“hacer un mapa de geomórfonos”** es sólo una tarea.

Cada tema será realizado por una sola persona.

## 2. Elige un área de estudio manejable

Puedes trabajar en cualquier lugar de la **República Dominicana** y, si
la pregunta lo justifica, en La Española o en otra área comparable.
Claro, para trabajar a escala de país o de isla, necesitarás reducir la
resolución de los datos (e.g. DEM con celda de 1 km lado) para poder
analizarlos computacionalmente. Por ello, **prioriza áreas de estudio
más pequeñas**, que permitan un análisis más detallado y una
interpretación más confiable. Prioriza unidades con sentido
geomorfológico, como éstas:

- cuencas o subcuencas;
- tramo de valle;
- abanicos aluviales;
- macizo o sierra;
- llanura;
- zona kárstica;
- municipio cuando tenga sentido como ventana espacial;
- área protegida u otra unidad territorial si la pregunta relaciona
  relieve y ambiente.

No elijas un área tan grande que convierta la práctica en un problema de
cómputo. Como regla general, para DEM de 30 m una ventana de algunos
cientos a pocos miles de km² suele ser suficiente.

## 3. Usa datos públicos y documentados

Puedes usar uno o más de los siguientes modelos y servicios:

- **Copernicus DEM GLO-30**, DSM global de ~30 m;
- **NASADEM**, DEM global de 1 segundo de arco basado en SRTM;
- **SRTM 1 arc-second**, cuando sea apropiado;
- **ALOS World 3D AW3D30**, DSM global de ~30 m;
- **MERIT DEM / MERIT Hydro**, particularmente para análisis
  hidrogeomorfológicos;
- **DTM/MDT del IGN de República Dominicana**, cuando esté disponible
  para el área;
- otros DEM públicos, si documentas procedencia, resolución, datum
  vertical y limitaciones.

También puedes obtener DEM globales mediante **OpenTopography** o
trabajar con colecciones disponibles en **Google Earth Engine**.

> **DEM no significa siempre terreno desnudo.** Copernicus DEM y AW3D30
> son modelos de superficie (DSM): pueden incluir el efecto de
> vegetación, edificaciones e infraestructura. Debes saber qué
> representa la fuente elegida y discutir las consecuencias para tu
> análisis.

## 4. Usa software apropiado

No existe obligación de repetir el análisis en dos programas. Escoge el
entorno que permita responder mejor tu pregunta y documenta las
versiones utilizadas. El servidor dispone de los ejecutabes de **GRASS
GIS 7.8.7** y **WhiteboxTools**, y adicionalmente cuentas con los
intérpretes de **R** y **Python** con librerías geoespaciales. Si lo
necesitases, podría instalar **SAGA GIS** (solicítamelo) para usarlo por
medio de la consola de comandos. En tu PC, instala **QGIS** y **Google
Earth Pro**; si puedes, instala en QGIS las extensiones de **SAGA GIS**
y **WhiteboxTools** (GRASS GIS normalmente viene de serie), para no
tener que usar la consola de comandos. Créate una cuenta en **Google
Earth Engine**, porque muchos análisis los correrás más fácilmente y
algunas fuentes las conseguirás en menos pasos. Puedes usar otros
programas, pero debes documentar su instalación y funcionamiento, y el
procedimiento debe ser reproducible. En QGIS podrías ejecutar tuberías
de procesamiento usando Python.

Son especialmente apropiados:

- **GRASS GIS 7.8.7**: `r.slope.aspect`, `r.param.scale`, `r.watershed`,
  `r.stream.*`, `r.geomorphon`, `r.viewshed`, `r.relief`, entre otros;
- **WhiteboxTools** y su interfaz desde R/Python;
- **SAGA GIS**;
- **R**: `terra`, `sf`, `stars`, entre otros;
- **Python**: `rasterio`, `xarray`, `geopandas`, etc.;
- **QGIS**, particularmente como interfaz para GDAL, GRASS, SAGA y
  Whitebox;
- **Google Earth Engine (GEE)** para acceso a datos, procesamiento a
  gran escala y ciertos derivados topográficos.

GEE calcula directamente pendiente, orientación y sombreado mediante
`ee.Terrain`, pero no sustituye a un paquete geomorfométrico completo.
Si tu pregunta requiere geomórfonos, HAND, métricas multiescala,
acondicionamiento hidrológico u otros métodos especializados, utiliza
una herramienta que realmente los implemente.

Este ejemplo de código R usando WhiteboxTools funciona en el servidor de
RStudio. De la misma forma, tu caso particular también podría aprovechar
WhiteboxTools.

``` r
library(terra)
library(whitebox)

# Directorio de trabajo de WhiteboxTools:
# usamos el directorio actual del proyecto RStudio
wbt_wd(getwd())

# Comprobar que WhiteboxTools responde
wbt_version()

# Crear un DEM artificial
dem <- rast(
  nrows = 100,
  ncols = 100,
  xmin = 0,
  xmax = 1000,
  ymin = 0,
  ymax = 1000,
  crs = "EPSG:32619"
)

# Coordenadas de los centros de las celdas
xy <- crds(dem)

# Crear una superficie inclinada con relieve ondulado
values(dem) <-
  100 +
  0.05 * xy[, 1] +
  10 * sin(xy[, 1] / 100) *
  cos(xy[, 2] / 100)

# Guardar el DEM
writeRaster(
  dem,
  "dem_prueba_wbt.tif",
  overwrite = TRUE
)

# Visualizar el DEM
plot(dem, main = "DEM artificial con Whitebox Tools")
```

<img src="README_files/figure-gfm/unnamed-chunk-4-1.png" width="100%" />

``` r
# Calcular pendiente con WhiteboxTools
wbt_slope(
  dem = "dem_prueba_wbt.tif",
  output = "pendiente_prueba_wbt.tif",
  units = "degrees"
)

# Leer el resultado generado por WhiteboxTools
pendiente <- rast("pendiente_prueba_wbt.tif")

# Resumen
pendiente
```

    ## class       : SpatRaster 
    ## size        : 100, 100, 1  (nrow, ncol, nlyr)
    ## resolution  : 10, 10  (x, y)
    ## extent      : 0, 1000, 0, 1000  (xmin, xmax, ymin, ymax)
    ## coord. ref. : WGS 84 / UTM zone 19N (EPSG:32619) 
    ## source      : pendiente_prueba_wbt.tif 
    ## name        : pendiente_prueba_wbt

``` r
global(
  pendiente,
  c("min", "mean", "max"),
  na.rm = TRUE
)
```

    ##                             min     mean      max
    ## pendiente_prueba_wbt 0.04412854 4.453254 9.849384

``` r
# Visualizar
plot(
  pendiente,
  main = "Pendiente calculada con WhiteboxTools"
)
```

<img src="README_files/figure-gfm/unnamed-chunk-4-2.png" width="100%" />

Con GRASS GIS funcionaría algo parecido.

``` r
library(terra)
library(rgrass)

# ------------------------------------------------------------
# Prueba mínima de GRASS GIS desde R
# ------------------------------------------------------------

# 1. Crear un DEM artificial
dem <- rast(
  nrows = 100,
  ncols = 100,
  xmin = 0,
  xmax = 1000,
  ymin = 0,
  ymax = 1000,
  crs = "EPSG:32619"
)

xy <- crds(dem)

values(dem) <-
  100 +
  0.05 * xy[, 1] +
  10 * sin(xy[, 1] / 100) *
  cos(xy[, 2] / 100)

writeRaster(
  dem,
  "dem_prueba_grass.tif",
  overwrite = TRUE
)

# 2. Crear una base de datos GRASS temporal
grassdb <- tempfile("grassdb_")
dir.create(grassdb)

# 3. Crear una location GRASS usando el CRS del propio GeoTIFF
system2(
  "grass",
  args = c(
    "-c",
    normalizePath("dem_prueba_grass.tif"),
    "-e",
    file.path(grassdb, "prueba")
  )
)

# 4. Inicializar GRASS sobre esa location
initGRASS(
  gisBase = system("grass --config path", intern = TRUE),
  home = tempdir(),
  gisDbase = grassdb,
  location = "prueba",
  mapset = "PERMANENT",
  override = TRUE
)
```

    ## gisdbase    /tmp/RtmpdX6ayS/grassdb_6e78a1c1e118a 
    ## location    prueba 
    ## mapset      PERMANENT 
    ## rows        100 
    ## columns     100 
    ## north       1000 
    ## south       0 
    ## west        0 
    ## east        1000 
    ## nsres       10 
    ## ewres       10 
    ## projection:
    ##  PROJCRS["WGS 84 / UTM zone 19N",
    ##     BASEGEOGCRS["WGS 84",
    ##         ENSEMBLE["World Geodetic System 1984 ensemble",
    ##             MEMBER["World Geodetic System 1984 (Transit)"],
    ##             MEMBER["World Geodetic System 1984 (G730)"],
    ##             MEMBER["World Geodetic System 1984 (G873)"],
    ##             MEMBER["World Geodetic System 1984 (G1150)"],
    ##             MEMBER["World Geodetic System 1984 (G1674)"],
    ##             MEMBER["World Geodetic System 1984 (G1762)"],
    ##             MEMBER["World Geodetic System 1984 (G2139)"],
    ##             ELLIPSOID["WGS 84",6378137,298.257223563,
    ##                 LENGTHUNIT["metre",1]],
    ##             ENSEMBLEACCURACY[2.0]],
    ##         PRIMEM["Greenwich",0,
    ##             ANGLEUNIT["degree",0.0174532925199433]],
    ##         ID["EPSG",4326]],
    ##     CONVERSION["UTM zone 19N",
    ##         METHOD["Transverse Mercator",
    ##             ID["EPSG",9807]],
    ##         PARAMETER["Latitude of natural origin",0,
    ##             ANGLEUNIT["degree",0.0174532925199433],
    ##             ID["EPSG",8801]],
    ##         PARAMETER["Longitude of natural origin",-69,
    ##             ANGLEUNIT["degree",0.0174532925199433],
    ##             ID["EPSG",8802]],
    ##         PARAMETER["Scale factor at natural origin",0.9996,
    ##             SCALEUNIT["unity",1],
    ##             ID["EPSG",8805]],
    ##         PARAMETER["False easting",500000,
    ##             LENGTHUNIT["metre",1],
    ##             ID["EPSG",8806]],
    ##         PARAMETER["False northing",0,
    ##             LENGTHUNIT["metre",1],
    ##             ID["EPSG",8807]]],
    ##     CS[Cartesian,2],
    ##         AXIS["(E)",east,
    ##             ORDER[1],
    ##             LENGTHUNIT["metre",1]],
    ##         AXIS["(N)",north,
    ##             ORDER[2],
    ##             LENGTHUNIT["metre",1]],
    ##     USAGE[
    ##         SCOPE["Engineering survey, topographic mapping."],
    ##         AREA["Between 72°W and 66°W, northern hemisphere between equator and 84°N, onshore and offshore. Aruba. Bahamas. Brazil. Canada - New Brunswick (NB); Labrador; Nunavut; Nova Scotia (NS); Quebec. Colombia. Dominican Republic. Greenland. Netherlands Antilles. Puerto Rico. Turks and Caicos Islands. United States. Venezuela."],
    ##         BBOX[0,-72,84,-66]],
    ##     ID["EPSG",32619]]

``` r
# 5. Importar el DEM
execGRASS(
  "r.in.gdal",
  input = normalizePath("dem_prueba_grass.tif"),
  output = "dem",
  flags = c("overwrite", "quiet")
)

# 6. Ajustar la región computacional al DEM
execGRASS(
  "g.region",
  raster = "dem"
)

# 7. Calcular pendiente
execGRASS(
  "r.slope.aspect",
  elevation = "dem",
  slope = "pendiente",
  format = "degrees",
  flags = c("overwrite", "quiet")
)

# 8. Exportar el resultado a GeoTIFF
execGRASS(
  "r.out.gdal",
  input = "pendiente",
  output = normalizePath(
    "pendiente_prueba_grass.tif",
    mustWork = FALSE
  ),
  format = "GTiff",
  flags = c("overwrite", "quiet")
)
```

    ## ERROR 6: /home/jose/202602/repos-gh/geo114/geomorfometria/pendiente_prueba_grass.tif, band 1: SetColorTable() only supported for Byte or UInt16 bands in TIFF format.

``` r
# 9. Leer y comprobar el resultado en R
pendiente <- rast("pendiente_prueba_grass.tif")

pendiente
```

    ## class       : SpatRaster 
    ## size        : 100, 100, 1  (nrow, ncol, nlyr)
    ## resolution  : 10, 10  (x, y)
    ## extent      : 0, 1000, 0, 1000  (xmin, xmax, ymin, ymax)
    ## coord. ref. : WGS 84 / UTM zone 19N (EPSG:32619) 
    ## source      : pendiente_prueba_grass.tif 
    ## name        : pendiente

``` r
global(
  pendiente,
  c("min", "mean", "max"),
  na.rm = TRUE
)
```

    ##                  min     mean      max
    ## pendiente 0.04898992 4.491461 8.507064

``` r
plot(dem, main = "DEM artificial con GRASS GIS")
```

<img src="README_files/figure-gfm/unnamed-chunk-5-1.png" width="100%" />

``` r
plot(
  pendiente,
  main = "Pendiente calculada con GRASS GIS"
)
```

<img src="README_files/figure-gfm/unnamed-chunk-5-2.png" width="100%" />

En ambos ejemplos, WhiteboxTools y GRASS GIS, usé un DEM artificial para
ilustrar el flujo de trabajo. En tu caso, reemplaza la creación del DEM
con la lectura de un DEM real, y ajusta los parámetros según tu pregunta
de investigación. Pídele ayuda a IA.

# Reglas mínimas del análisis

Independientemente del tema elegido, tu trabajo debe cumplir lo
siguiente:

1.  **Pregunta explícita.** Debe aparecer al final de la introducción.
2.  **Al menos una hipótesis o expectativa razonada**, cuando la
    naturaleza del tema lo permita.
3.  **Más de un producto descriptivo.** Un único mapa de pendiente no
    constituye una investigación.
4.  **Al menos una comparación, gradiente, clasificación, estadístico o
    prueba cuantitativa.**
5.  **Escala documentada.** Debes declarar tamaño de píxel y, cuando
    aplique, tamaño de ventana/radio/umbral.
6.  **CRS y unidades documentados.** Para operaciones basadas en
    distancia/área, trabaja en un CRS proyectado adecuado o justifica
    otro procedimiento.
7.  **Preprocesamiento documentado.** Explica recorte, reproyección,
    relleno de depresiones, suavizado, resampleo o acondicionamiento
    hidrológico si los utilizaste.
8.  **Dos figuras científicas como mínimo**, al menos una de ellas un
    mapa.
9.  **Una tabla como mínimo**, generada reproduciblemente desde los
    datos.
10. **Código ejecutable y organizado.** No se acepta una cadena de clics
    no documentada como único registro metodológico; por esta razón,
    prefiere cuadernos RMarkdown o Jupyter.

# 30 temas realizables para elegir

La columna “producto mínimo” indica una forma razonable de mantener el
tema acotado. Puedes mejorarla, pero no convertir la práctica en un
proyecto semestral. Elige un tema y comunícalo en el hilo
correspondiente en el foro.

|  \# | Tema/pregunta posible                                                                                                                 | Datos sugeridos                    | Herramientas apropiadas      | Producto mínimo verificable              |
|----:|---------------------------------------------------------------------------------------------------------------------------------------|------------------------------------|------------------------------|------------------------------------------|
|   1 | ¿Cómo cambia la **pendiente** estimada entre dos DEM globales de resolución semejante?                                                | Copernicus GLO-30 + NASADEM/AW3D30 | R, GRASS, Whitebox           | mapa de diferencias + distribución/MAE   |
|   2 | ¿Cuánto cambia la pendiente al **degradar la resolución** del DEM?                                                                    | Copernicus GLO-30                  | R/GRASS                      | 30, 60 y 90 m + comparación              |
|   3 | ¿Cómo varía la **curvatura** con el tamaño de ventana?                                                                                | DEM 30 m                           | GRASS `r.param.scale`, SAGA  | perfiles/planform curvature multiescala  |
|   4 | ¿Qué sectores presentan mayor **rugosidad del terreno** y cómo se relaciona con elevación?                                            | DEM 30 m                           | R/Whitebox                   | TRI/roughness + relación con elevación   |
|   5 | ¿La **posición topográfica (TPI)** cambia al usar escala local y de paisaje?                                                          | DEM 30 m                           | Whitebox/R                   | TPI en dos escalas + clases              |
|   6 | ¿Qué clasificación de **formas del terreno** producen los geomórfonos a dos radios de búsqueda?                                       | DEM 30 m                           | GRASS `r.geomorphon`         | dos mapas + matriz de transición         |
|   7 | ¿Dónde coinciden y dónde discrepan una clasificación por **TPI** y una por **geomórfonos**?                                           | DEM 30 m                           | Whitebox + GRASS             | mapa de acuerdo + tabla cruzada          |
|   8 | ¿Qué proporción del área corresponde a crestas, laderas, valles y superficies planas?                                                 | DEM 30 m                           | GRASS/Whitebox               | clasificación + porcentajes              |
|   9 | ¿Cómo cambia el **relieve relativo/local relief** con radios de 0.5, 1 y 2 km?                                                        | DEM 30 m                           | Whitebox/R focal             | superficies multiescala + perfiles       |
|  10 | ¿Dónde se concentran las mayores tasas de **disección topográfica**?                                                                  | DEM + drenaje derivado             | GRASS/R                      | densidad/relieve + zonificación          |
|  11 | ¿Qué diferencias produce el **relleno de depresiones** sobre la red de drenaje?                                                       | DEM 30 m                           | GRASS/Whitebox               | red antes/después + métricas             |
|  12 | ¿Cómo cambia la red extraída al variar el **umbral de acumulación de flujo**?                                                         | DEM 30 m                           | GRASS `r.watershed`/Whitebox | 3 umbrales + longitud/densidad           |
|  13 | ¿Qué algoritmo de flujo genera diferencias apreciables: **D8 frente a MFD/D∞**?                                                       | DEM 30 m                           | GRASS/Whitebox               | acumulación comparada + diferencias      |
|  14 | ¿Qué tan bien coincide una **red derivada del DEM** con una red hidrográfica de referencia?                                           | DEM + OSM/MERIT Hydro              | GRASS/R                      | distancia/acuerdo espacial               |
|  15 | ¿Cómo varían **orden de corriente y razón de bifurcación** dentro de una cuenca?                                                      | DEM                                | GRASS `r.stream.*`           | red ordenada + tabla Horton-Strahler     |
|  16 | ¿Cómo difieren dos subcuencas en **densidad de drenaje, relieve y pendiente**?                                                        | DEM                                | GRASS/R                      | tabla morfométrica comparativa           |
|  17 | ¿Cómo cambia la **curva hipsométrica** entre dos o más subcuencas?                                                                    | DEM + cuencas                      | R/GRASS                      | curvas + integral hipsométrica           |
|  18 | ¿Existe relación entre **integral hipsométrica y relieve local** entre subcuencas?                                                    | DEM                                | R/GRASS                      | métricas por subcuenca + gráfico         |
|  19 | ¿Cómo varía el **Topographic Wetness Index (TWI)** según el algoritmo de acumulación?                                                 | DEM                                | GRASS/SAGA/Whitebox          | dos TWI + comparación                    |
|  20 | ¿Qué zonas bajas próximas al drenaje identifica **HAND** y cómo cambian con un umbral distinto de red?                                | DEM                                | Whitebox/GEE/GRASS + scripts | HAND + áreas bajo 5/10 m                 |
|  21 | ¿Qué diferencia existe entre **HAND y elevación absoluta** para identificar fondos de valle?                                          | DEM                                | Whitebox/R                   | mapas + perfiles transversales           |
|  22 | ¿Dónde se concentran superficies potencialmente más expuestas a radiación según **aspect/northness/eastness**?                        | DEM                                | R/GEE/GRASS                  | componentes de aspecto + estadísticos    |
|  23 | ¿Cómo cambia la **insolación potencial** entre vertientes de diferente orientación?                                                   | DEM                                | GRASS `r.sun`                | radiación + comparación por orientación  |
|  24 | ¿Qué sectores combinan **alta pendiente y alta convergencia** como aproximación morfométrica a zonas de concentración de escorrentía? | DEM                                | SAGA/GRASS/R                 | índice compuesto + cuantiles             |
|  25 | ¿Puede una combinación de pendiente, curvatura y TPI separar **fondos de valle y divisorias**?                                        | DEM                                | R/Whitebox                   | clasificación simple + validación visual |
|  26 | ¿Cómo cambia la delimitación de una **divisoria** entre dos DEM distintos?                                                            | 2 DEM                              | GRASS/Whitebox               | polígonos + diferencia de área           |
|  27 | ¿Qué diferencias de elevación sistemáticas existen entre **Copernicus, NASADEM y AW3D30** en bosque frente a áreas abiertas?          | 3 DEM + cobertura                  | GEE/R                        | diferencias por cobertura                |
|  28 | ¿Cuánto afecta un **DSM frente a un DTM** a pendiente/rugosidad donde exista MDT público?                                             | Copernicus/AW3D30 + IGN MDT        | R/GRASS                      | diferencias y estadísticos               |
|  29 | ¿Qué porción de un área es visible desde uno o varios puntos mediante **viewshed** y cómo cambia con la altura del observador?        | DEM                                | GRASS `r.viewshed`           | 2 alturas + superficie visible           |
|  30 | ¿Qué combinación de variables geomorfométricas permite construir una **regionalización fisiográfica reproducible** sencilla?          | DEM                                | R/GRASS/Whitebox             | 3–5 variables + clustering/clases        |

# Orientaciones específicas para algunos temas

## Comparaciones entre DEM

Antes de restar DEM debes armonizar:

- extensión;
- tamaño y alineación de píxel;
- CRS horizontal;
- unidades;
- referencia vertical en la medida de lo posible.

No interpretes automáticamente toda diferencia como “error”. Los
productos pueden representar superficies distintas, proceder de sensores
distintos, tener fechas distintas y utilizar procedimientos de edición
diferentes.

## Análisis hidrológico

Una red derivada de un DEM depende del acondicionamiento de la
superficie y del algoritmo de flujo. Explica si:

- rellenaste o rompiste depresiones;
- excavaste/breached obstáculos;
- impusiste una red;
- utilizaste D8, MFD, D∞ u otro método;
- definiste la red mediante un umbral de número de celdas o área
  contribuyente.

Para comparaciones hidrográficas puedes utilizar MERIT Hydro, que
proporciona una hidrografía global basada en MERIT DEM y otras capas
hidrográficas (Yamazaki et al., 2019).

## Geomórfonos

Los geomórfonos clasifican formas elementales a partir de patrones de
visibilidad del entorno y no simplemente mediante una derivada local del
DEM (Jasiewicz y Stepinski, 2013). Por ello, el radio de búsqueda y el
umbral de planitud son decisiones metodológicas que debes declarar y,
preferiblemente, explorar.

## Escala

En geomorfometría, “escala” no es un detalle menor. El tamaño de píxel y
el vecindario utilizado determinan qué componentes del relieve pueden
aparecer o desaparecer. Un resultado multiescala suele ser más
informativo que una única elección arbitraria (Florinsky, 2016; Hengl y
Reuter, 2009).

# Datos: opciones recomendadas

## Copernicus DEM GLO-30

Es un **DSM global** a aproximadamente 30 m, basado principalmente en
TanDEM-X y distribuido públicamente. Puede obtenerse mediante Copernicus
Data Space, servicios públicos y plataformas como GEE/OpenTopography. No
debes describirlo como terreno desnudo sin matices.

## NASADEM / SRTM

NASADEM reprocesó la información SRTM y ofrece elevación global a un
segundo de arco para las latitudes cubiertas por la misión. SRTM sigue
siendo una referencia histórica esencial de la topografía global (Farr
et al., 2007).

## ALOS AW3D30

AW3D30 es un DSM global de aproximadamente un segundo de arco derivado
de datos PRISM de ALOS. Es útil como DEM alternativo para ejercicios de
comparación.

## MERIT Hydro

MERIT Hydro proporciona dirección de flujo, área de acumulación y otras
capas hidrográficas a aproximadamente 3 segundos de arco, con especial
utilidad como referencia en análisis de redes y cuencas (Yamazaki
et al., 2019).

# Flujo de trabajo recomendado

## Etapa 1 — Formular

Antes de procesar datos, escribe:

- pregunta;
- hipótesis o expectativa;
- área de estudio;
- variable de respuesta o criterio de comparación;
- DEM;
- algoritmo;
- escala(s);
- producto cuantitativo que permitirá responder la pregunta.

Si no puedes escribir esas siete cosas en unas pocas líneas,
probablemente el tema todavía está demasiado abierto.

## Etapa 2 — Adquirir y preparar

Guarda en `data_raw/` sólo archivos pequeños que puedan versionarse. Los
DEM grandes **no deben subirse al repositorio de GitHub, porque hay un
límite establecido de 50 MB por archivos individuales, pero sí pueden
subirse al servidor RStudio**. En su lugar, documenta la fuente y crea
un script de descarga o instrucciones reproducibles, o úsalo sólo en el
servidor y evita subirlo a GitHub por medio del archivo .gitignore.

Organización recomendada:

``` text
.
├── README.Rmd
├── bibliografia.bib
├── plantilla.Rmd
├── data_raw/
├── data/
├── R/
├── scripts/
├── outputs/
│   ├── figures/
│   ├── tables/
│   └── rasters/
├── docs/
└── ... otros archivos del repo ...
```

El repositorio incluye un archivo `.gitignore` con exclusiones básicas.
**Revísalo y amplíalo si tu flujo de trabajo genera otros archivos
grandes, temporales o regenerables.** Los patrones incluidos son
orientativos: no debes ignorar indiscriminadamente una carpeta completa
si contiene archivos pequeños necesarios para reproducir tu análisis.

## Etapa 3 — Analizar

Tu script debe:

1.  cargar o localizar los datos;
2.  verificar CRS, resolución, extensión y valores NoData;
3.  efectuar el preprocesamiento;
4.  calcular los derivados geomorfométricos;
5.  resumir cuantitativamente el resultado;
6.  producir tablas;
7.  producir figuras;
8.  guardar sólo las salidas necesarias.

Evita operaciones manuales irrepetibles. Si una operación se hace en
QGIS, conserva un modelo, comando, historial o descripción
suficientemente precisa.

## Etapa 4 — Verificar

No des por bueno el resultado porque “se ve razonable”. Realiza
controles mínimos:

- revisa mínimo, máximo, media/mediana y cuantiles;
- comprueba unidades;
- inspecciona visualmente zonas planas y abruptas;
- busca artefactos de borde;
- comprueba alineación espacial;
- verifica que los umbrales utilizados tengan significado físico;
- repite una parte del análisis con otro parámetro cuando la pregunta lo
  requiera.

## Etapa 5 — Redactar

El manuscrito debe construirse **a partir del análisis**, no como texto
independiente pegado encima del código.

# Estructura del manuscrito

## Título

Debe expresar la pregunta o el hallazgo principal y mencionar el área de
estudio. Evita títulos como “Práctica de geomorfometría”.

## Resumen

Entre **150 y 250 palabras**. Incluye brevemente:

- problema;
- datos;
- método;
- resultado principal cuantitativo;
- conclusión.

Añade entre **3 y 5 palabras clave** que no repitan innecesariamente el
título.

## Introducción

Extensión orientativa: **3–5 párrafos**.

Debes:

1.  situar el problema geomorfológico;
2.  explicar los conceptos geomorfométricos necesarios;
3.  mostrar qué problema, contraste o incertidumbre analizarás;
4.  terminar con pregunta, hipótesis/expectativa y objetivo(s).

Incluye **al menos cinco fuentes bibliográficas**, combinando
fundamentos y literatura reciente/relevante. Hengl & Reuter (Hengl y
Reuter, 2009) es una referencia básica, no la única.

No uses citas literales salvo necesidad excepcional. Cita ideas,
métodos, algoritmos y conjuntos de datos.

## Materiales y métodos

Extensión orientativa: **3–5 párrafos**, más una tabla o esquema si
resulta útil.

Documenta:

- área de estudio;
- DEM y datos auxiliares;
- resolución espacial;
- CRS horizontal y referencia vertical conocida;
- software y versiones;
- preprocesamiento;
- algoritmo(s);
- parámetros;
- análisis estadístico;
- procedimiento de elaboración de figuras/tablas.

Incluye una **tabla de reproducibilidad** como ésta, generada o
completada desde el propio RMarkdown:

| Elemento   | Información mínima                 |
|------------|------------------------------------|
| DEM        | nombre, versión/fuente             |
| Resolución | tamaño nominal y tamaño de trabajo |
| CRS        | EPSG o WKT                         |
| Software   | nombre y versión                   |
| Algoritmo  | método/módulo/función              |
| Parámetros | radios, umbrales, ventanas, etc.   |
| AOI        | criterio de delimitación           |
| Código     | archivo(s) del repositorio         |

## Resultados

Presenta primero la evidencia y después el texto que la describe.

Debes incluir como mínimo:

- **2 figuras**, al menos una cartográfica;
- **1 tabla**;
- **3 resultados cuantitativos** expresados en el texto.

No repitas en prosa todos los números de una tabla. Señala patrones y
valores necesarios para responder la pregunta.

Todas las figuras y tablas deben tener:

- número;
- título/caption informativo;
- referencia cruzada en el texto;
- unidades;
- leyenda adecuada;
- fuente cuando corresponda.

## Discusión

Extensión orientativa: **3–5 párrafos**.

Debes:

- responder explícitamente la pregunta;
- indicar si los resultados apoyan o no la expectativa/hipótesis;
- explicar geomorfológicamente el patrón;
- compararlo con literatura o conocimiento previo;
- discutir sensibilidad a DEM, escala, algoritmo y parámetros;
- identificar limitaciones;
- señalar qué análisis adicional tendría mayor valor.

No conviertas la discusión en una segunda sección de resultados.

## Conclusiones

Entre **1 y 3 párrafos breves**. Responde al objetivo con afirmaciones
respaldadas por los resultados. No introduzcas datos, métodos o citas
nuevas salvo necesidad justificada.

## Declaración de reproducibilidad

Incluye al final un párrafo breve indicando:

- dónde está el código;
- qué datos son públicos;
- qué archivos no se incluyen y cómo obtenerlos;
- qué versiones de software son relevantes;
- si existen pasos manuales no automatizados.

## Auditoría de IA

Incluye un recuadro o párrafo de **100–200 palabras** con:

- herramienta de IA utilizada, si la utilizaste;
- tarea para la que se usó;
- una respuesta problemática concreta;
- cómo detectaste el problema;
- fuente, prueba o ejecución con que lo verificaste;
- corrección final.

Si no utilizaste IA durante la práctica, declara explícitamente que no
la utilizaste; no tienes que inventar un error.

## Referencias

El manuscrito se elaborará siguiendo el **formato APA 7 implementado en
`plantilla.Rmd`**. Gestiona las citas y referencias mediante el archivo
BibTeX `bibliografia.bib` y comprueba manualmente que:

- todas las citas aparecen en referencias;
- no hay referencias no citadas;
- DOI y autores son correctos;
- las referencias sugeridas por IA existen realmente;
- citas de software y datos están documentadas cuando corresponde.

# Figuras: requisitos

Al menos una figura debe ser un **mapa analítico**, no una captura de
pantalla de QGIS o GEE.

El mapa debe contener, cuando sean pertinentes:

- leyenda;
- escala o información equivalente;
- sistema de coordenadas adecuado;
- unidades;
- referencia espacial suficiente para interpretar el área;
- paleta coherente con la variable;
- caption que explique qué se representa.

La segunda figura puede ser, por ejemplo:

- histograma/densidad;
- boxplot;
- perfil topográfico;
- curva hipsométrica;
- diagrama de dispersión;
- matriz de confusión/acuerdo;
- gráfico por clases;
- comparación multiescala.

# Tablas: requisitos

Las tablas deben generarse desde objetos de datos siempre que sea
posible. No insertes una captura de Excel.

Una tabla apropiada puede resumir:

- estadísticas de derivados;
- porcentajes por clase;
- métricas por subcuenca;
- diferencias entre DEM;
- longitud de red por orden;
- sensibilidad a parámetros;
- resultados de concordancia.

# Reproducibilidad técnica

El repositorio debe poder entenderse sin una explicación oral adicional.

Como mínimo:

- usa rutas relativas;
- evita rutas como `C:/Users/tu_nombre/...`;
- incluye `sessionInfo()` o equivalente;
- fija semillas cuando exista aleatoriedad;
- separa datos originales y productos derivados;
- no edites manualmente una tabla que pueda obtenerse desde código;
- no subas archivos ráster gigantes;
- documenta cualquier dato que requiera descarga externa.

En R puedes cerrar el documento con:

``` r
sessionInfo()
```

# Recomendaciones sobre herramientas

## GRASS GIS

GRASS dispone de una familia amplia de módulos para análisis de terreno
e hidrología. Entre otros, pueden resultar útiles `r.slope.aspect`,
`r.param.scale`, `r.watershed`, `r.stream.extract`, `r.geomorphon`,
`r.viewshed` y `r.sun`.

## WhiteboxTools

WhiteboxTools está diseñado como backend de análisis geoespacial y
contiene numerosos algoritmos de geomorfometría e hidrología. Puede
invocarse desde línea de comandos, Python o mediante el paquete
`whitebox` de R (Lindsay, 2016).

## Google Earth Engine

GEE es especialmente útil para:

- acceder a DEM globales sin descargas manuales;
- recortar áreas;
- efectuar análisis sencillos de pendiente/orientación;
- combinar topografía con cobertura, vegetación, agua u otras
  colecciones;
- exportar un AOI para procesamiento geomorfométrico especializado.

No asumas que `ee.Terrain` reproduce el algoritmo de GRASS, SAGA o
WhiteboxTools. Una comparación entre software sólo es válida si
documentas qué calcula cada uno.

# Organización sugerida en tres jornadas

## Día 1 — Pregunta, datos y análisis

Completa:

- elección del tema y AOI;
- búsqueda de bibliografía;
- adquisición/preparación de datos;
- primer análisis;
- control de calidad;
- borrador de figuras y tabla.

Al finalizar el día debes tener **evidencia suficiente para saber si la
pregunta es respondible**.

## Día 2 — Análisis definitivo y manuscrito

Completa:

- análisis definitivo;
- figuras;
- tabla;
- introducción;
- materiales y métodos;
- resultados;
- discusión;
- conclusiones;
- referencias;
- declaración de reproducibilidad.

## Día 3 — Revisión y defensa

Completa:

- auditoría de IA;
- revisión de citas y referencias;
- regeneración limpia del manuscrito;
- diapositivas;
- ensayo de la exposición.

# Lista de comprobación antes de entregar

- [ ] Mi trabajo contiene una **pregunta**, no sólo una operación SIG.
- [ ] Puedo explicar qué representa realmente mi DEM.
- [ ] Documenté resolución, CRS, algoritmo y parámetros.
- [ ] El análisis incluye una comparación o resultado cuantitativo.
- [ ] El manuscrito se genera desde RMarkdown.
- [ ] Tengo al menos dos figuras y una tabla.
- [ ] Todas las figuras/tablas son citadas en el texto.
- [ ] Mis resultados incluyen valores numéricos relevantes.
- [ ] Separé resultados de discusión.
- [ ] Todas las citas tienen referencia y viceversa.
- [ ] Verifiqué DOI/datos bibliográficos importantes.
- [ ] No subí archivos innecesariamente grandes.
- [ ] Documenté pasos manuales.
- [ ] Incluí declaración de reproducibilidad.
- [ ] Incluí la auditoría de IA o declaré que no utilicé IA.
- [ ] El PDF final compila sin errores.

# Criterios de evaluación del manuscrito

| Criterio                   | Nivel 1                       | Nivel 2                    | Nivel 3                            | Nivel 4                                              |
|----------------------------|-------------------------------|----------------------------|------------------------------------|------------------------------------------------------|
| Pregunta geomorfológica    | Ausente o puramente operativa | Implícita                  | Clara y respondible                | Clara, pertinente y bien justificada                 |
| Análisis geomorfométrico   | Incorrecto                    | Básico                     | Correcto                           | Correcto, comparativo y bien interpretado            |
| Datos, escala y algoritmos | No documentados               | Documentación parcial      | Adecuadamente documentados         | Decisiones justificadas y sensibilidad considerada   |
| Evidencia cuantitativa     | Ausente                       | Escasa                     | Suficiente                         | Sólida y directamente ligada a la pregunta           |
| Reproducibilidad           | No reproducible               | Parcial                    | Bien documentada                   | Flujo limpio, ejecutable y auditable                 |
| Redacción científica       | Deficiente                    | Comprensible               | Clara                              | Precisa, fluida y argumentativa                      |
| Figuras y tablas           | Incorrectas/ausentes          | Básicas                    | Correctas                          | Excelente integración y diseño científico            |
| Citas y referencias        | Deficientes                   | Parciales                  | Mayormente correctas               | Íntegras, pertinentes y verificadas                  |
| Discusión                  | Repite resultados             | Interpretación superficial | Interpreta y reconoce limitaciones | Integra mecanismo, escala, literatura y limitaciones |
| Auditoría de IA            | Ausente/inventada             | Genérica                   | Error concreto verificado          | Auditoría convincente y epistemológicamente útil     |

# Criterios de evaluación de la defensa

| Criterio                  | Nivel 1               | Nivel 2              | Nivel 3                | Nivel 4                             |
|---------------------------|-----------------------|----------------------|------------------------|-------------------------------------|
| Claridad del problema     | Confuso               | Parcial              | Claro                  | Muy claro y motivado                |
| Explicación del método    | No comprende el flujo | Comprensión parcial  | Explica correctamente  | Justifica decisiones y alternativas |
| Lectura de figuras/tablas | No interpreta         | Describe             | Interpreta             | Sintetiza evidencia con precisión   |
| Discusión de limitaciones | Ausente               | Genérica             | Adecuada               | Crítica y específica                |
| Auditoría de IA           | No demostrada         | Débil                | Verificada             | Demuestra error, causa y corrección |
| Respuestas                | No responde           | Respuestas limitadas | Responde correctamente | Argumenta y reconoce incertidumbre  |
| Manejo del tiempo         | Muy fuera del tiempo  | Algo fuera           | Adecuado               | Muy bien administrado               |

# Referencias de partida

No debes limitar tu búsqueda a esta lista. Úsala como punto de partida.

Hengl & Reuter (Hengl y Reuter, 2009) sigue siendo una obra fundamental
para conceptos, parámetros y aplicaciones. Para una perspectiva
matemática y multiescala más extensa consulta Florinsky (Florinsky,
2016), y para aplicaciones ambientales del modelado digital del terreno
consulta Wilson (Wilson, 2018).

Entre métodos y herramientas de interés se encuentran los geomórfonos
(Jasiewicz y Stepinski, 2013), Whitebox (Lindsay, 2016), SRTM (Farr
et al., 2007) y MERIT Hydro (Yamazaki et al., 2019).

**Busca además bibliografía reciente y específica de tu pregunta.** En
temas de geomorfometría, una referencia clásica explica el método, pero
la discusión del problema aplicado debe apoyarse también en literatura
actual.

<div id="refs" class="references csl-bib-body hanging-indent"
entry-spacing="0" line-spacing="2">

<div id="ref-farr2007srtm" class="csl-entry">

Farr, T. G., Rosen, P. A., Caro, E., Crippen, R., Duren, R., Hensley,
S., Kobrick, M., Paller, M., Rodriguez, E., Roth, L., Seal, D., Shaffer,
S., Shimada, J., Umland, J., Werner, M., Oskin, M., Burbank, D. y
Alsdorf, D. (2007). The Shuttle Radar Topography Mission. *Reviews of
Geophysics*, *45*(2). <https://doi.org/10.1029/2005RG000183>

</div>

<div id="ref-florinsky2016digital" class="csl-entry">

Florinsky, I. V. (2016). *Digital Terrain Analysis in Soil Science and
Geology* (2.ª ed.). Academic Press.

</div>

<div id="ref-hengl2009geomorphometry" class="csl-entry">

Hengl, T. y Reuter, H. I. (Eds.). (2009). *Geomorphometry: Concepts,
Software, Applications* (Vol. 33). Elsevier.

</div>

<div id="ref-jasiewicz2013geomorphons" class="csl-entry">

Jasiewicz, J. y Stepinski, T. F. (2013). Geomorphons—a pattern
recognition approach to classification and mapping of landforms.
*Geomorphology*, *182*, 147-156.
<https://doi.org/10.1016/j.geomorph.2012.11.005>

</div>

<div id="ref-lindsay2016whitebox" class="csl-entry">

Lindsay, J. B. (2016). Whitebox GAT: A case study in geomorphometric
analysis. *Computers & Geosciences*, *95*, 75-84.
<https://doi.org/10.1016/j.cageo.2016.07.003>

</div>

<div id="ref-wilson2018environmental" class="csl-entry">

Wilson, J. P. (2018). *Environmental Applications of Digital Terrain
Modeling*. John Wiley & Sons. <https://doi.org/10.1002/9781118938188>

</div>

<div id="ref-yamazaki2019merithydro" class="csl-entry">

Yamazaki, D., Ikeshima, D., Sosa, J., Bates, P. D., Allen, G. H. y
Pavelsky, T. M. (2019). MERIT Hydro: A High-Resolution Global
Hydrography Map Based on Latest Topography Dataset. *Water Resources
Research*, *55*, 5053-5073. <https://doi.org/10.1029/2019WR024873>

</div>

</div>
