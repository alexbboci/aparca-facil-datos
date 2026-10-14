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
