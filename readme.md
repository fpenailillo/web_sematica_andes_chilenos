Web Semántica y Datos Abiertos — Montañismo Andino
Magíster en Tecnologías de la Información · Q1 2026
Dominio: Rutas de montañismo en los Andes (Andeshandbook.org)
Datos abiertos: Datos medioambientales del MMA/SINIA de Chile
Validación RDF: Rudof — J.E. Labra Gayo
Referencia principal: "Web Semántica: Comprendiendo el cambio hacia la Web 3.0" — Jose Emilio Labra Gayo.

Equipo:

Introducción
El montañismo en los Andes constituye una actividad que genera un volumen creciente de datos: rutas con sus características técnicas, registros de ascensión, condiciones climáticas, estado medioambiental y presencia de áreas protegidas. Históricamente, esta información ha estado dispersa en portales web, hojas de cálculo y bases de datos heterogéneas, sin interoperabilidad entre ellas.

Este proyecto aplica los principios de la Web Semántica y los Datos Abiertos para construir un Grafo de Conocimiento (Knowledge Graph) sobre el dominio del montañismo andino chileno. La propuesta integra cuatro fuentes de datos:

Fuente	Tipo	Descripción
Andeshandbook.org	Privado/scrapeado	Rutas de montaña: elevación, dificultad, actividades, sector geográfico
SINIA-MMA Chile	Datos abiertos	Estaciones de monitoreo de calidad del aire cercanas a zonas cordilleranas
SNASPE-CONAF	Datos abiertos	Áreas silvestres protegidas del Estado: parques nacionales, reservas
RETC-MMA Chile	Datos abiertos	Registros de emisiones de contaminantes por establecimientos industriales
La integración de estas fuentes en un único grafo RDF permite responder preguntas complejas que ninguna fuente podría responder de forma aislada: ¿Qué rutas de alta montaña se encuentran dentro de áreas protegidas con estaciones de monitoreo de calidad del aire en su entorno? o ¿Qué fuentes industriales registradas en el RETC podrían afectar la calidad del aire en rutas sobre 4.000 m.s.n.m.?

Herramientas y estándares utilizados
RDF (Resource Description Framework): modelo de datos en tripletas (sujeto, predicado, objeto) para representar el conocimiento del dominio
Turtle: serialización legible del grafo RDF
ShEx (Shape Expressions): validación declarativa de la estructura del grafo con Rudof
SHACL (Shapes Constraint Language): validación alternativa recomendada por el W3C
SPARQL: lenguaje de consulta sobre el grafo local y federado (Wikidata)
Solid/POD: arquitectura descentralizada para datos personales enlazados
Estructura del Notebook
Tarea 1: Construcción del grafo RDF y validación (ShEx + SHACL)
Tarea 2: Consultas SPARQL sobre el grafo local + federadas con Wikidata + comparación con LLMs
Tarea 3: Análisis de integración KG + LLMs (patrón GraphRAG)
Tarea 4: Datos abiertos, privacidad y el proyecto Solid aplicado al montañismo
