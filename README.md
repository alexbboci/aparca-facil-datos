# Aparca Fácil — catálogo público

Ubicaciones de aparcamiento accesible. No indica disponibilidad en tiempo real. Cobertura parcial: una zona sin registros puede tener plazas accesibles. Consulta siempre la señalización.

## Archivo
`Aparca-Facil-datos-publicos.json` contiene una revisión completa con los conjuntos `parking` y `vigo`. Una ubicación puede contener varias plazas (`capacity`). La fecha `publishedAt` es de publicación, no de visita.

## Fuentes y licencias
- Registros de OpenStreetMap: © colaboradores de OpenStreetMap, ODbL 1.0. https://www.openstreetmap.org/copyright
- Conjunto `vigo`: Concello de Vigo, catálogo parking-discapacitados, ODC-By 1.0. https://datos-ckan.vigo.org/dataset/parking-discapacitados — https://opendatacommons.org/licenses/by/1-0/
- Aportaciones aprobadas: identificadas como `community`. No implican comprobación independiente.
- Otras referencias públicas: identificadas como `public-research`, con fuente, URL y fecha documental por registro. Sus contenidos originales conservan sus derechos. No se reproducen fotografías.

Los conjuntos conservan sus fuentes y condiciones; este repositorio no sustituye las licencias originales ni otorga derechos sobre contenido de terceros. Mantén la atribución al reutilizar datos.

## Actualizaciones
Sustituir el JSON completo tras moderar aportaciones y comprobar coordenadas y duplicados. Incrementar `revision` y `publishedAt`. La app consulta este archivo al abrirse con caché de 15 minutos. No necesita un despliegue en Netlify por cada cambio de plazas.

Nunca incluir credenciales, propuestas privadas, datos personales de colaboradores ni fotografías pendientes de revisión.

## Madrid
Fuente: Ayuntamiento de Madrid, Plazas de estacionamiento para personas de movilidad reducida. Catálogo actualizado el 07/09/2026, cobertura hasta 04/09/2026. https://datos.madrid.es/dataset/208083-0-estacionamiento-pmr — CC BY 4.0: https://creativecommons.org/licenses/by/4.0/
Datos adaptados: selección conservadora de registros, identificación estable por coordenadas, normalización de nombres y capacidad. Coordenadas aproximadas del centro de cada reserva, no comprobadas presencialmente. Los casos con texto de señal, capacidad desconocida, áreas grandes o duplicados se han dejado fuera de esta primera importación. La ausencia de texto no garantiza ausencia de restricciones.

Alcobendas: 151 ubicaciones generales (197 plazas), revisión documental 14/10/2026. Ayuntamiento de Alcobendas, ODC-By: https://datos.gob.es/es/catalogo/l01280066-reservas-de-estacionamiento-para-personas-con-movilidad-reducida . Se excluyen reservas nominativas, condiciones dudosas y coordenadas incoherentes. La fecha original de cada ficha figura en su nota; no implica comprobación presencial. No se publican matrículas ni números de tarjeta.

## Ampliación regional — 14/10/2026
365 ubicaciones nuevas de OpenStreetMap en 19 municipios de los alrededores de Madrid y 305 en 35 municipios de la provincia de Barcelona (13 en la capital). Extractos Geofabrik del 13/10/2026: https://download.geofabrik.de/europe/spain/madrid.html y https://download.geofabrik.de/europe/spain/cataluna.html . ODbL 1.0, © colaboradores de OpenStreetMap. Se seleccionan plazas explícitamente mapeadas, con coordenadas del punto o un punto interior de su polígono; nombres de calles cercanas orientativos. Se excluyen accesos restringidos, aparcamientos interiores identificados y condiciones dudosas. La ausencia de restricciones en los datos no garantiza el acceso. Sin comprobación presencial.

## Ampliación de Galicia — 14/10/2026
14 ubicaciones adicionales: 10 en Lugo y 4 en Vigo. Fuente: OpenStreetMap, extracto de Galicia descargado el 13/10/2026 (https://download.geofabrik.de/europe/spain/galicia.html), ODbL 1.0. Revisión de horarios sin restricciones (24/7), acceso y posibles duplicados. Se conservan fechas originales y capacidades desconocidas como null. Sin comprobación presencial. Galicia suma 1.749 ubicaciones; cobertura parcial.

## Reservas completas PMR — 14/10/2026
8 ubicaciones adicionales de OpenStreetMap en Arteixo, Boiro, Santiago de Compostela, Ribadeo, Vilaboa y Cangas. 24 plazas de capacidad declarada entre siete ubicaciones; una octava sin capacidad conocida. Coordenadas del punto o interior de pequeñas áreas reservadas íntegramente para PMR, no del centro de un aparcamiento general. Se contrastaron límites municipales, accesos, tamaño y duplicados con el catálogo. ODbL 1.0; extracto de Geofabrik de Galicia descargado el 13/10/2026. No comprobadas presencialmente. Total Galicia tras esta actualización: 1.757 ubicaciones.

## València — 17/10/2026

2.566 ubicaciones con 2.779 plazas declaradas. Fuente: Ayuntamiento de València, Geoportal, capa «Aparcamientos personas movilidad reducida». Licencia CC BY 4.0: https://creativecommons.org/licenses/by/4.0/deed.es . Catálogo: https://datos.gob.es/es/catalogo/l01462508-aparcamientos-personas-movilidad-reducida . Descarga completa comprobada frente a los identificadores del servicio municipal el 17/10/2026. Adaptaciones: selección de identificador, coordenadas y capacidad, normalización al esquema de la aplicación y nombres descriptivos generados. No incluye ocupación en tiempo real. Sin verificación presencial; consulta la señalización. La fecha de consulta no implica que todas las plazas hayan sido comprobadas ese día. No se garantiza cobertura exhaustiva ni ausencia de restricciones no descritas por la fuente.


## Zaragoza — 17/10/2026

1.135 ubicaciones con 1.270 plazas declaradas. Origen de los datos: Ayuntamiento de Zaragoza, https://www.zaragoza.es/web/espacio-de-datos/servicio/catalogo/307 . Reutilización según https://www.zaragoza.es/sede/portal/aviso-legal . Última actualización indicada en el catálogo: 29/04/2022; fecha de actualización de la ficha: 24/09/2026. API consultada el 17/10/2026: 1.236 registros descargados, con paginación completa e identificadores únicos. Selección de reservas PMR generales permanentes; 101 registros excluidos por categoría, horario limitado o dudoso o capacidad inválida. Adaptaciones: selección conservadora, normalización de direcciones y transformación al esquema de la app. Sin comprobación presencial; consulta la señalización. Proyecto independiente, sin patrocinio del Ayuntamiento.


## Donostia / San Sebastián — 17/10/2026

829 ubicaciones generales. Fuente: Ayuntamiento de Donostia / San Sebastián, Aparcamientos de movilidad reducida, https://donostia.eus/datosabiertos/catalogo/aparcamiento-movreducida . Catálogo modificado el 15/05/2026, consultado el 17/10/2026. Datos y adaptación de los registros con prefijo `donostia-official/` bajo CC BY-SA 3.0: https://creativecommons.org/licenses/by-sa/3.0/ . Se conservan como subconjunto identificable con su propia licencia. Adaptaciones: selección GENERAL, nombres y coordenadas al esquema de la app; capacidad desconocida, sin deducirla de la longitud. Se excluyen 78 reservas por matrícula. Completitud contrastada entre descarga municipal y capa oficial de GeoDonostia. Sin comprobación presencial ni información de ocupación; consulta la señalización.


## Tenerife — 17/10/2026

1.002 ubicaciones en 31 municipios. Fuente: Cabildo de Tenerife / SINPROMI, Mapa de accesibilidad de la isla de Tenerife: https://datos.tenerife.es/ckan/dataset/97d6af67-4c9b-41ef-a1fd-cb7c55dbff95 . Licencia CC BY indicada en el catálogo: https://opendefinition.org/licenses/cc-by/ . Recurso actualizado el 04/06/2026; se conserva la fecha original de cada punto en sourceUpdated (no equivale a verificación propia). Selección de señalización horizontal afirmativa y sin límite de tiempo indicado; se dejan fuera 126 registros por restricciones, duplicados, fechas futuras o municipio sin resolver. Municipio normalizado a partir de la clasificación municipal de las referencias fotográficas de SINPROMI; no se reproducen fotografías. No se deduce una capacidad numérica. La nota conserva la información sobre comunicación con itinerario peatonal. Sin comprobación presencial propia, sin información de ocupación y sin garantía de cobertura completa.


## Asturias y Cantabria — 17/10/2026

261 ubicaciones explícitas de OpenStreetMap: 115 en 12 municipios de Asturias y 146 en 11 municipios de Cantabria. Se recorrieron los límites de los 78 y 102 municipios respectivos; ausencia de puntos no implica ausencia de plazas. Extractos de Geofabrik: https://download.geofabrik.de/europe/spain/asturias.html y https://download.geofabrik.de/europe/spain/cantabria.html . © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Se conserva la fecha de edición de cada punto, no equivalente a una visita. Adaptaciones: punto cartografiado o interior del polígono reservado PMR, municipio por límites administrativos y calle cercana orientativa. Se excluyen accesos restringidos, aparcamientos interiores, horarios o pagos dudosos y posibles duplicados. 154 plazas de capacidad conocida; 117 ubicaciones sin capacidad publicada. Sin comprobación presencial.


## Navarra y La Rioja — 17/10/2026

523 ubicaciones explícitas de OpenStreetMap: 417 en 23 municipios de Navarra y 106 en 12 municipios de La Rioja. Extractos de Geofabrik con datos hasta el 16/10/2026: https://download.geofabrik.de/europe/spain/navarra.html y https://download.geofabrik.de/europe/spain/la-rioja.html . © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . 461 plazas de capacidad conocida y 190 ubicaciones de capacidad desconocida. Se revisaron accesos, condiciones, duplicados, geometría y posición interior de los marcadores de polígonos. Se dejaron fuera dos áreas de Logroño de más de 250 m² para comprobar la posición de las plazas individuales. Municipio por límites administrativos; calle cercana orientativa. Sin comprobación presencial; cobertura parcial.


## Murcia y Baleares — 17/10/2026

274 ubicaciones explícitas de OpenStreetMap: 23 en 7 municipios de Murcia y 251 en 21 municipios de Illes Balears. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Extractos de Geofabrik: https://download.geofabrik.de/europe/spain/murcia.html y https://download.geofabrik.de/europe/spain/islas-baleares.html . 118 plazas de capacidad conocida, 186 ubicaciones de capacidad desconocida. Adaptaciones: selección de puntos o polígonos reservados PMR, municipio por límites administrativos y calle cercana orientativa. Se comprueban geometrías y posiciones, accesos, restricciones, condiciones de pago y duplicados. Sin comprobación presencial; cobertura parcial, incluso en los municipios recorridos sin resultados.


## País Vasco y Aragón — 17/10/2026

1.358 ubicaciones explícitas de OpenStreetMap: 1.193 en País Vasco y 165 en Aragón. Extractos de Geofabrik con datos hasta el 16/10/2026: https://download.geofabrik.de/europe/spain/pais-vasco.html y https://download.geofabrik.de/europe/spain/aragon.html . © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . 995 plazas de capacidad conocida y 483 ubicaciones de capacidad desconocida. Se conservaron los inventarios municipales de Donostia y Zaragoza sin añadir puntos OSM de esas ciudades; así se evita reintroducir reservas personales o condicionadas. Se comprobaron 1.013 polígonos, su geometría y la posición interior del marcador, además de accesos, condiciones y duplicados. Municipio por límites administrativos; calle cercana orientativa. Sin comprobación presencial; cobertura parcial.


## Extremadura — ampliación OSM del 17/10/2026

41 ubicaciones en 17 municipios, con 42 plazas de capacidad conocida y 8 ubicaciones sin capacidad especificada. Fuente: https://download.geofabrik.de/europe/spain/extremadura.html . Fecha del extracto: 2026-10-16T20:21:21Z. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Se excluyen accesos restringidos, interiores, condiciones dudosas, duplicados y geometrías demasiado grandes; los marcadores de polígonos se sitúan dentro de ellos. Calle cercana orientativa; sin comprobación presencial. València y Sevilla se reservan para sus inventarios municipales. Cobertura parcial.


## Comunitat Valenciana — ampliación OSM del 17/10/2026

412 ubicaciones en 57 municipios, con 254 plazas de capacidad conocida y 212 ubicaciones sin capacidad especificada. Fuente: https://download.geofabrik.de/europe/spain/valencia.html . Fecha del extracto: 2026-10-16T20:21:21Z. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Se excluyen accesos restringidos, interiores, condiciones dudosas, duplicados y geometrías demasiado grandes; los marcadores de polígonos se sitúan dentro de ellos. Calle cercana orientativa; sin comprobación presencial. València y Sevilla se reservan para sus inventarios municipales. Cobertura parcial.


## Castilla y León — ampliación OSM del 17/10/2026

467 ubicaciones en 42 municipios, con 455 plazas de capacidad conocida y 184 ubicaciones sin capacidad especificada. Fuente: https://download.geofabrik.de/europe/spain/castilla-y-leon.html . Fecha del extracto: 2026-10-16T20:21:21Z. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Se excluyen accesos restringidos, interiores, condiciones dudosas, duplicados y geometrías demasiado grandes; los marcadores de polígonos se sitúan dentro de ellos. Calle cercana orientativa; sin comprobación presencial. València y Sevilla se reservan para sus inventarios municipales. Cobertura parcial.


## Andalucía — ampliación OSM del 17/10/2026

461 ubicaciones en 42 municipios, con 251 plazas de capacidad conocida y 272 ubicaciones sin capacidad especificada. Fuente: https://download.geofabrik.de/europe/spain/andalucia.html . Fecha del extracto: 2026-10-16T20:21:21Z. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Se excluyen accesos restringidos, interiores, condiciones dudosas, duplicados y geometrías demasiado grandes; los marcadores de polígonos se sitúan dentro de ellos. Calle cercana orientativa; sin comprobación presencial. València y Sevilla se reservan para sus inventarios municipales. Cobertura parcial.


## Cáceres — 17/10/2026

660 ubicaciones del inventario municipal. Fuente: Ayuntamiento de Cáceres, https://ide.caceres.es/geonetwork/srv/spa/catalog.search#/metadata/f9c9c0fa-201e-4cdc-a784-de8a733a1f84 . Metadatos actualizados el 07/05/2025 y servicio consultado el 17/10/2026; no equivalen a una visita. Descarga completa de 755 registros; se excluyen 82 de gestión privada, una reserva personal y 12 con discrepancias entre coordenadas. Se transforman las geometrías nativas EPSG:25829 a WGS84 para evitar el redondeo de la exportación geográfica, y se contrastan con los atributos de coordenadas. Capacidad no especificada por registro. Los metadatos indican que no se aplican condiciones de uso adicionales; el portal https://ide.caceres.es/descargas/movilidad-catalogo atribuye sus contenidos a licencias Creative Commons Reconocimiento 4.0 y 3.0. Se conserva la atribución al Ayuntamiento. No se incluyen matrículas, fotografías ni información personal. Sin comprobación presencial; consulta la señalización.

## Sevilla — 17/10/2026

444 ubicaciones y 465 plazas declaradas. Fuente: Ayuntamiento de Sevilla, Gerencia de Urbanismo, mapa oficial https://www.urbanismosevilla.org/areas/sostenibilidad-innovacion/oficina-de-accesibilidad/plazas-aparcamiento-reservado-pmr . La política municipal de datos espaciales abiertos permite su reutilización: https://www.urbanismosevilla.org/areas/sostenibilidad-innovacion/ide/portal-de-datos-abiertos . Descarga paginada completa de 2.445 registros, contrastada con el contador del servicio e identificadores únicos. Última edición de la capa: 21/04/2023. Selección de viario público sin baja indicada y con evaluación favorable del espacio de transferencia en el inventario. Se excluyen 46 bajas, 388 registros fuera del viario público o con situación desconocida y 1.567 con deficiencias de transferencia o sin evaluación conocida. Adaptación de dirección, punto y capacidad. Evaluación histórica municipal; no es verificación propia ni garantía del estado actual. Sin comprobación presencial; cobertura parcial.


## Canarias — ampliación OSM del 17/10/2026

238 ubicaciones adicionales en 43 municipios, con 128 plazas de capacidad conocida y 127 ubicaciones sin capacidad especificada. Fuente: https://download.geofabrik.de/africa/canary-islands.html . Fecha del extracto: 2026-10-16T20:21:21Z. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Contraste con el catálogo previo para evitar duplicados; control de accesos, condiciones y geometrías. Posición cartografiada o interior del polígono reservado; calle cercana orientativa. Sin comprobación presencial, cobertura parcial.


## Castilla-La Mancha — ampliación OSM del 17/10/2026

62 ubicaciones adicionales en 19 municipios, con 86 plazas de capacidad conocida y 24 ubicaciones sin capacidad especificada. Fuente: https://download.geofabrik.de/europe/spain/castilla-la-mancha.html . Fecha del extracto: 2026-10-16T20:21:21Z. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Contraste con el catálogo previo para evitar duplicados; control de accesos, condiciones y geometrías. Posición cartografiada o interior del polígono reservado; calle cercana orientativa. Sin comprobación presencial, cobertura parcial.


## Cataluña — ampliación OSM del 17/10/2026

288 ubicaciones adicionales en 30 municipios, con 123 plazas de capacidad conocida y 172 ubicaciones sin capacidad especificada. Fuente: https://download.geofabrik.de/europe/spain/cataluna.html . Fecha del extracto: 2026-10-13T20:21:31Z. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Contraste con el catálogo previo para evitar duplicados; control de accesos, condiciones y geometrías. Posición cartografiada o interior del polígono reservado; calle cercana orientativa. Sin comprobación presencial, cobertura parcial.

## Pamplona / Iruña — 17/10/2026

918 ubicaciones adicionales procedentes del Ayuntamiento de Pamplona / Iruñeko Udala. Catálogo oficial y licencia CC BY 4.0: https://datosabiertos.navarra.es/es/dataset/spapamplona_segu_pto_aparcminus . Licencia: https://creativecommons.org/licenses/by/4.0/ . Inventario actualizado en octubre de 2025 según los metadatos del WFS, consultado el 17/10/2026. Los 998 puntos de la descarga SHP se contrastan con los 998 del WFS; coordenadas nativas EPSG:25830 transformadas a WGS84. Se excluyen 74 coincidencias próximas a ubicaciones existentes, dos duplicados próximos y cuatro puntos fuera del límite municipal consultado. Se conservan los nombres de calle de la fuente; no se inventa la capacidad. No es una comprobación presencial y no indica ocupación. Cobertura parcial; consulta la señalización vigente. Datos adaptados por Aparca Fácil, sin respaldo institucional implícito.


## Pequeñas reservas completas PMR — 17/10/2026

29 ubicaciones adicionales con 104 plazas de capacidad declarada: Asturias (9), Cantabria (2), Navarra (3), La Rioja (1), Murcia (7) e Illes Balears (7). Se seleccionan puntos o pequeñas áreas que OpenStreetMap identifica íntegramente como reservadas para PMR; no se utiliza el centro de aparcamientos generales. Geometrías válidas y puntos interiores, máximo 250 m² y control de superficie por plaza. Se comprueban municipio, capacidad, restricciones y duplicados. No son visitas ni garantías de disponibilidad. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright .

- asturias: https://download.geofabrik.de/europe/spain/asturias.html — extracto 2026-10-16T20:21:21Z.

- cantabria: https://download.geofabrik.de/europe/spain/cantabria.html — extracto 2026-10-16T20:21:21Z.

- navarra: https://download.geofabrik.de/europe/spain/navarra.html — extracto 2026-10-16T20:21:21Z.

- la-rioja: https://download.geofabrik.de/europe/spain/la-rioja.html — extracto 2026-10-16T20:21:21Z.

- murcia: https://download.geofabrik.de/europe/spain/murcia.html — extracto 2026-10-16T20:21:21Z.

- islas-baleares: https://download.geofabrik.de/europe/spain/islas-baleares.html — extracto 2026-10-16T20:21:21Z.


## Girona — 17/10/2026

314 ubicaciones adicionales con 436 plazas declaradas. Fuente: Ajuntament de Girona / UMAT, https://umat.girona.cat/apps/api/descarrega/items/184/ . Datos de dominio público y reutilización gratuita según https://umat.girona.cat/legal.html . De 1.049 áreas de estacionamiento del servicio se seleccionan las 322 clasificadas como Mobilitat reduïda; descarga completa e identificadores contrastados. Se incorporan polígonos de titularidad pública, gratuitos, en superficie, de geometría válida y tamaño compatible con la capacidad declarada. Se excluyen cuatro casos de pago o coste desconocido, dos coincidencias con el catálogo, un duplicado próximo y una geometría pendiente. Marcador interior del polígono reservado transformado de EPSG:25831 a WGS84, no posición de cada plaza individual. Fecha de actualización individual no publicada; consulta documental el 17/10/2026, sin comprobación presencial ni respaldo institucional implícito. Consulta la señalización.

## Jaca y Urduliz — 17/10/2026

Dos reservas completas PMR adicionales, una plaza declarada en cada ubicación. Fuente: OpenStreetMap, © colaboradores, ODbL 1.0 https://www.openstreetmap.org/copyright . Pequeños polígonos válidos con marcador interior; control de acceso, condiciones, límites municipales y duplicados. Sin comprobación presencial.

- pais-vasco: https://download.geofabrik.de/europe/spain/pais-vasco.html — extracto 2026-10-16T20:21:21Z.

- aragon: https://download.geofabrik.de/europe/spain/aragon.html — extracto 2026-10-16T20:21:21Z.


## Ampliación de reservas completas PMR — 17/10/2026

219 ubicaciones adicionales, con 493 plazas declaradas. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Se seleccionan puntos y pequeñas áreas reservadas íntegramente para PMR; no centros de aparcamientos generales. Se revisan restricciones, duplicados, capacidad y límites municipales. Los polígonos se contrastan con la geometría original, con marcador interior y tamaño máximo de 250 m². Municipio por límites administrativos y calle cercana orientativa. Sin comprobación presencial ni garantía de disponibilidad; cobertura parcial.

- valencia: 7 ubicaciones, 21 plazas declaradas. https://download.geofabrik.de/europe/spain/valencia.html — extracto 2026-10-16T20:21:21Z.
- extremadura: 1 ubicaciones, 3 plazas declaradas. https://download.geofabrik.de/europe/spain/extremadura.html — extracto 2026-10-16T20:21:21Z.
- castilla-y-leon: 20 ubicaciones, 62 plazas declaradas. https://download.geofabrik.de/europe/spain/castilla-y-leon.html — extracto 2026-10-16T20:21:21Z.
- andalucia: 141 ubicaciones, 260 plazas declaradas. https://download.geofabrik.de/europe/spain/andalucia.html — extracto 2026-10-16T20:21:21Z.
- castilla-la-mancha: 7 ubicaciones, 23 plazas declaradas. https://download.geofabrik.de/europe/spain/castilla-la-mancha.html — extracto 2026-10-16T20:21:21Z.
- canary-islands: 21 ubicaciones, 80 plazas declaradas. https://download.geofabrik.de/africa/canary-islands.html — extracto 2026-10-16T20:21:21Z.
- cataluna: 22 ubicaciones, 44 plazas declaradas. https://download.geofabrik.de/europe/spain/cataluna.html — extracto 2026-10-13T20:21:31Z.


## Reservas completas en la Comunidad de Madrid — 17/10/2026

12 ubicaciones adicionales con 15 plazas declaradas: Valdemoro (7), Collado Villalba (3), Loeches (1) y Majadahonda (1). Fuente: https://download.geofabrik.de/europe/spain/madrid.html — extracto 2026-10-13T20:21:31Z. © colaboradores de OpenStreetMap, ODbL 1.0: https://www.openstreetmap.org/copyright . Reservas completas PMR de tamaño limitado; posición cartografiada o interior de geometría contrastada. Se excluyen Madrid y Alcobendas para conservar la selección de sus inventarios oficiales. Control de municipio, acceso, capacidad y duplicados. Sin comprobación presencial; consulta la señalización.


## Manlleu y Roses — 17/10/2026

Manlleu: 60 ubicaciones adicionales con 68 plazas declaradas. Fuente: Ajuntament de Manlleu / Situam, https://observatori-manlleu-situam.hub.arcgis.com/datasets/4a5d7b0f3d53480595027f6fadfa5d02_0 . Se aplica CC BY 4.0 indicada en el servicio original: https://creativecommons.org/licenses/by/4.0/ . El catálogo agregado AOC etiqueta CC0; conservamos la atribución y la licencia del origen. Se descargan los 75 registros y se contrasta el conjunto completo de identificadores; geometría cotejada con LAT/LONG. Se excluyen 15 referencias a equipamientos y aparcamientos subterráneos para revisar acceso y posición. Última edición de los datos indicada por ArcGIS: 21/07/2023; la fecha más reciente del catálogo no implica revisión de las plazas.

Roses: 154 ubicaciones adicionales, capacidad desconocida. Fuente: Ajuntament de Roses / AOC, https://dadesobertes.seu-e.cat/dataset/roses-reserva-d-estacionament-de-vehicles-per-persones-amb-discapacitat-i-mobilitat-reduida . Licencia CC BY indicada por el catálogo: https://opendefinition.org/licenses/cc-by/ . Recurso actualizado según catálogo el 15/01/2026. De 212 registros se excluyen los 55 que contienen observaciones, incluidas reservas individualizadas, y tres coincidencias con ubicaciones existentes. La ausencia de observaciones no garantiza ausencia de restricciones actuales. No se reproducen matrículas ni datos personales.

Ambos conjuntos: coordenadas contrastadas con límites municipales, control de duplicados y adaptación al esquema de la app. Sin comprobación presencial ni respaldo institucional implícito. Consulta siempre la señalización; cobertura parcial.

## Salamanca — 17/10/2026

479 ubicaciones adicionales y 775 plazas declaradas. Fuente y autor del inventario: Ayuntamiento de Salamanca, «Aparcamiento Personas Movilidad Reducida», https://opendata.aytosalamanca.es/datosabiertos/catalogo/dataset/aparcamiento-para-personas-con-movilidad-reducida . Descarga WFS completa de 525 puntos, contrastada con el contador del servicio y las coordenadas EPSG:25830 transformadas a WGS84 (diferencia máxima inferior a 1 cm). Catálogo modificado el 04/11/2025; no se publica fecha de revisión individual. Consulta documental el 17/10/2026, sin comprobación presencial.

Se excluyen 30 referencias a equipamientos o accesos que necesitan revisión, 12 coincidencias próximas con el catálogo y cuatro sitios con capacidad superior a seis cuyo emplazamiento individual requiere comprobación. Municipio por límite administrativo. Consulta siempre la señalización y las restricciones vigentes.

El subconjunto identificable `salamanca-official/`, titulado «Selección de reservas PMR de Salamanca para Aparca Fácil — 17 de octubre de 2026», conserva la GNU Free Documentation License 1.3. Inventario original: Ayuntamiento de Salamanca; selección y modificaciones © Aparca Fácil 2026; editor de la adaptación: Aparca Fácil. Sin secciones invariantes ni textos de cubierta. El texto íntegro de la licencia, autores, historial de modificaciones y enlaces a la copia original se incluyen en `parking.documents.salamanca` dentro del JSON público. Los registros, su metadata y licencia constituyen el documento reutilizable; los otros conjuntos independientes de esta recopilación mantienen sus propias condiciones. Proyecto independiente sin respaldo institucional. El archivo JSON descargable es la copia editable, sin restricciones adicionales de reproducción.
