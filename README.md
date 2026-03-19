ETL Seguros Pipeline

Descripción del proyecto:

El presente proyecto tiene como objetivo desarrollar un proceso ETL (Extract, Transform, Load) aplicado a un conjunto de datos relacionados con el sector de seguros. A partir de archivos en formato CSV almacenados en un repositorio de GitHub, se realiza un flujo de trabajo que permite transformar datos crudos en información limpia y estructurada, lista para su análisis.

El proceso inicia con la extracción de los datasets desde la carpeta correspondiente dentro del repositorio. Posteriormente, mediante el uso de Python en Google Colab, se lleva a cabo la transformación de los datos, lo cual incluye diversas tareas de limpieza, estandarización y validación. Como resultado, los datos se organizan en dos grupos principales: registros válidos y registros rechazados, dependiendo de si cumplen o no con las reglas de calidad definidas.

Tecnologías utilizadas

Para la implementación del pipeline se emplearon herramientas y tecnologías ampliamente utilizadas en el área de ingeniería de datos. Entre ellas se encuentran Python como lenguaje principal, la librería Pandas para el procesamiento de datos, Google Colab como entorno de ejecución en la nube y GitHub para el almacenamiento y gestión del proyecto.

Estructura del proyecto

El repositorio está organizado de manera que facilite el manejo de los datos y el desarrollo del proceso ETL. En la carpeta data se encuentran tres subcarpetas: raw, donde se almacenan los datos originales; curated, que contiene los datos limpios y procesados; y rejects, donde se guardan los registros que no cumplen con los criterios de calidad.

Por otro lado, la carpeta notebooks incluye los cuadernos de Google Colab utilizados para procesar cada dataset de forma independiente, permitiendo un control más ordenado y modular del flujo de trabajo.

Proceso ETL

El proceso ETL desarrollado en este proyecto se divide en tres etapas principales. En la fase de extracción, los datos son obtenidos desde archivos CSV ubicados en el repositorio. Luego, en la fase de transformación, se aplican diferentes técnicas de limpieza y preparación de datos, tales como la normalización de nombres de columnas, eliminación de espacios innecesarios, conversión de valores vacíos a nulos, eliminación de registros duplicados, así como la transformación de formatos de fechas y valores numéricos.

Durante la etapa de validación, se implementan reglas básicas de calidad de datos para clasificar la información en dos grupos. Por un lado, los datos válidos, que cumplen con los requisitos establecidos, y por otro, los datos rechazados, que presentan inconsistencias como campos obligatorios vacíos, formatos incorrectos o valores inválidos.

Finalmente, en la fase de carga, los resultados del proceso son almacenados en archivos separados dentro de las carpetas curated y rejects, lo que permite mantener una clara distinción entre datos útiles y datos que requieren revisión.

Datasets utilizados

El proyecto trabaja con múltiples datasets relacionados entre sí dentro del contexto de seguros. Entre ellos se incluyen información de clientes, aseguradoras, corredores, tipos de seguro, pólizas y siniestros. Cada uno de estos conjuntos de datos es procesado de manera individual mediante su respectivo notebook, lo que facilita su análisis y transformación.

Resultados obtenidos

Como resultado final, se logra la implementación de un pipeline ETL funcional que permite procesar datos desde archivos CSV, aplicar técnicas de limpieza y validación, y organizar la información en estructuras más adecuadas para su posterior análisis. Este enfoque no solo mejora la calidad de los datos, sino que también establece una base sólida para futuros procesos de análisis o integración de información.
