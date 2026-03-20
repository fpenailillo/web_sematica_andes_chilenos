# 🏔️ Web Semántica y Datos Abiertos: Montañismo Andino
**Magíster en Tecnologías de la Información · Q1 2026**

> **Construcción de un Grafo de Conocimiento (Knowledge Graph) para la integración de rutas de montañismo en Chile con datos medioambientales e industriales abiertos.**

## 📖 Introducción
El montañismo en los Andes constituye una actividad que genera un volumen creciente de datos: detalles técnicos de las rutas, registros de ascensión, condiciones climáticas, estado medioambiental y superposición con áreas protegidas. Históricamente, esta información ha estado fragmentada en portales web, hojas de cálculo y bases de datos heterogéneas, careciendo de interoperabilidad.

Este proyecto aplica los principios de la **Web Semántica** y los **Datos Abiertos (Open Data)** para solucionar este problema. Mediante la construcción de un Grafo de Conocimiento, unificamos el dominio del montañismo andino chileno, permitiendo descubrir relaciones ocultas y evaluar el impacto ambiental en las rutas de montaña.

## 🎯 Casos de Uso y Preguntas de Competencia
La integración de estas fuentes en un único grafo RDF permite responder a preguntas analíticas complejas que ninguna de las fuentes podría resolver de forma aislada:
* *¿Qué rutas de alta montaña se encuentran dentro de áreas protegidas que además cuentan con estaciones de monitoreo de calidad del aire en su entorno?*
* *¿Qué fuentes industriales registradas en el RETC podrían estar afectando la calidad del aire en rutas ubicadas sobre los 4.000 m.s.n.m.?*

## 🗄️ Fuentes de Datos Integradas

| Fuente | Tipo de Acceso | Descripción en el Grafo |
| :--- | :--- | :--- |
| **Andeshandbook.org** | Privado / Web Scraping | Rutas de montaña: elevación, dificultad técnica, actividades y sector geográfico. |
| **SINIA - MMA Chile** | Datos Abiertos | Estaciones de monitoreo de calidad del aire cercanas a zonas cordilleranas. |
| **SNASPE - CONAF** | Datos Abiertos | Áreas Silvestres Protegidas del Estado (Parques Nacionales, Reservas). |
| **RETC - MMA Chile** | Datos Abiertos | Registros de emisiones de contaminantes por establecimientos industriales. |

## 🛠️ Herramientas y Estándares Utilizados
El proyecto se apoya fuertemente en los estándares del W3C y metodologías de vanguardia:

* **Modelamiento y Serialización:**
  * **RDF (Resource Description Framework):** Modelo de datos basado en tripletas (sujeto, predicado, objeto).
  * **Turtle:** Serialización humanamente legible del grafo RDF.
* **Validación de Datos:**
  * **ShEx (Shape Expressions):** Validación declarativa de la estructura del grafo utilizando **Rudof** *(Ref: J.E. Labra Gayo)*.
  * **SHACL:** Validación alternativa recomendada por el W3C.
* **Consultas e Integración:**
  * **SPARQL:** Lenguaje de consulta para el grafo local y consultas federadas (ej. integrando Wikidata).
* **Análisis Espacial y Visualización:**
  * **Python, Pandas y Folium:** Procesamiento de datos espaciales y proyección de los resultados de las consultas en mapas interactivos.
* **Arquitectura y Privacidad:**
  * **Solid / POD:** Arquitectura descentralizada para la gestión de datos personales enlazados aplicados al perfil del montañista.

## 📓 Estructura del Proyecto (Notebook)
El desarrollo práctico se encuentra documentado paso a paso:

1. **Tarea 1: Construcción y Validación.** Creación del grafo RDF a partir de las fuentes y validación estructural mediante ShEx y SHACL.
2. **Tarea 2: Exploración del Grafo.** Ejecución de consultas SPARQL sobre el modelo local, enriquecimiento mediante consultas federadas a Wikidata y comparación analítica con modelos de lenguaje (LLMs).
3. **Tarea 3: Inteligencia Artificial.** Análisis de la integración del Knowledge Graph con LLMs utilizando el patrón **GraphRAG** (Retrieval-Augmented Generation basado en grafos).
4. **Tarea 4: Ética y Arquitectura.** Discusión sobre datos abiertos, privacidad y la aplicación del proyecto Solid al ecosistema del montañismo.

## 👥 Equipo
* **[Tu Nombre]** - *Rol / Investigador*
* **[Nombre Integrante]** - *Rol*

> **Referencia Principal:** *"Web Semántica: Comprendiendo el cambio hacia la Web 3.0"* — Jose Emilio Labra Gayo.
