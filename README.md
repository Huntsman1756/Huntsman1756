# h1756

**Datos regulatorios españoles listos para consultar: CNMV, ESMA, GLEIF y Banco de España, con la fuente oficial y la fecha de cada dato.**

Opero un conjunto de webs que reconstruyen registros financieros públicos de forma reproducible y enlazan cada cifra con el documento oficial del que sale. Para quién: gestoras, áreas de cumplimiento, research, fintechs y consultoras que necesitan estos datos limpios y fechados sin montar su propia captura.

## Webs que opero

| Web | Qué responde | Fuente oficial | Datos a |
|---|---|---|---|
| [ISIN España](https://isin-es.h1756.es/?utm_source=github&utm_medium=profile&utm_campaign=perfil-2026-12) | ¿Qué instrumentos tienen vínculo español (ISIN ES, emisor GLEIF español o cotización en plaza española)? | ESMA FIRDS · GLEIF · BORME | ![](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fisin-es.h1756.es%2Festado.json&query=%24.data_as_of&label=&color=0b7285) |
| [Registro DLT](https://isin-es.h1756.es/dlt?utm_source=github&utm_medium=profile&utm_campaign=perfil-2026-12) | ¿Qué emisiones en DLT están inscritas en las ERIR de la CNMV? | CNMV (ERIR) | ![](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fisin-es.h1756.es%2Festado.json&query=%24.data_as_of&label=&color=0b7285) |
| [OpenVenue](https://openvenue.h1756.es/?utm_source=github&utm_medium=profile&utm_campaign=perfil-2026-12) | Dado un ISIN: identidad en FIRDS, mercados europeos donde cotiza, emisor GLEIF, elegibilidad BCE | ESMA FIRDS · GLEIF · BCE | ![](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fopenvenue.h1756.es%2Festado.json&query=%24.data_as_of&label=&color=0b7285) |
| [Posiciones cortas](https://shorts.h1756.es/?utm_source=github&utm_medium=profile&utm_campaign=perfil-2026-12) | ¿Quién tiene posiciones cortas netas notificadas y sobre qué emisor, desde 2010? | CNMV | ![](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fshorts.h1756.es%2Festado.json&query=%24.data_as_of&label=&color=0b7285) |
| [Hechos relevantes de fondos](https://fondos-watch.h1756.es/?utm_source=github&utm_medium=profile&utm_campaign=perfil-2026-12) | ¿Qué ha comunicado la CNMV sobre un fondo, SICAV o IIC? | CNMV | ![](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Ffondos-watch.h1756.es%2Festado.json&query=%24.data_as_of&label=&color=0b7285) |
| [Sanciones](https://sanciones.h1756.es/?utm_source=github&utm_medium=profile&utm_campaign=perfil-2026-12) | ¿Qué sanciones han publicado el Banco de España y la CNMV, con historial de cambios? | Banco de España · CNMV | ![](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fsanciones.h1756.es%2Festado.json&query=%24.data_as_of&label=&color=0b7285) |
| [Cuentas de cotizadas](https://cuentas.h1756.es/?utm_source=github&utm_medium=profile&utm_campaign=perfil-2026-12) | Cuentas de las cotizadas españolas por ejercicio; si un concepto no se publica, dice «no publicado», nunca 0 | Informes ESEF (filings.xbrl.org) · GLEIF | ![](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fcuentas.h1756.es%2Festado.json&query=%24.data_as_of&label=&color=0b7285) |
| [IA en la banca](https://banca-ia.h1756.es/?utm_source=github&utm_medium=profile&utm_campaign=perfil-2026-12) | Lo que declaran los bancos sobre IA frente a los datos oficiales de empleo y oficinas | Banco de España · AEB · INE | ![](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fbanca-ia.h1756.es%2Festado.json&query=%24.data_as_of&label=&color=0b7285) |

La columna «Datos a» se lee en directo del `estado.json` público de cada web: si una fuente se retrasa, se ve aquí.

## Conéctalo a tu asistente de IA

Servidor MCP público en el [Registro Oficial de MCP](https://registry.modelcontextprotocol.io/v0.1/servers?search=es.h1756.mcp&version=latest) como `es.h1756.mcp/h1756-mcp`, con endpoint `mcp.h1756.es/mcp`. Resuelve entidades por nombre, ISIN o LEI, saca la ficha de un instrumento (FIRDS, GLEIF), el perfil de una entidad y las sanciones publicadas, y cita la fuente oficial en cada respuesta.

## Cómo comprobarlo

- Cada registro enlaza el documento oficial del que procede; cada web tiene su página de metodología.
- Las cifras se pueden recontar contra el fichero oficial (por ejemplo, el Excel de posiciones cortas que publica la CNMV).

## Otras webs

Más proyectos con datos públicos (empleo, oposiciones, becas, ayudas, transporte, listas de espera) en [h1756.es](https://h1756.es/?utm_source=github&utm_medium=profile&utm_campaign=perfil-2026-12).

El código es privado. Los datos conservan las condiciones de sus editores oficiales.

**Contacto:** [@rllzops en X](https://x.com/rllzops)
