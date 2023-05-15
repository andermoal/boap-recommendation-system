# boap-recommendation-system
Sistema de recomendación de documentos académicos electrónicos de la BOAP

Este proyecto implementa un sistema de recomendación de documentos académicos basado en técnicas de minería de texto y aprendizaje no supervisado. El sistema utiliza la API de Scopus para obtener los resúmenes de los documentos consultados por los usuarios, y posteriormente aplica técnicas como TF-IDF, similitud de cosenos y K-means para procesar y analizar la información.

## Funcionalidades principales

- Preprocesamiento del texto: se realiza una eliminación de signos de puntuación y se convierte el texto a minúsculas.
- Creación de la matriz de características: se utiliza TF-IDF para representar los documentos y extraer las características más relevantes.
- Selección de la cantidad óptima de clusters: se emplea el algoritmo K-means y el coeficiente de silueta para determinar el número adecuado de clusters.
- Identificación de temas: se asignan etiquetas a los documentos agrupados y se crean ecuaciones de búsqueda basadas en los términos más representativos de cada tema.
- Recomendación de documentos similares: se calcula la similitud coseno entre los documentos consultados y los documentos disponibles en Scopus, y se devuelve una lista de resultados recomendados.

## Uso del código

El archivo principal es `main.ipynb`, que contiene las funciones principales del sistema de recomendación. El flujo de ejecución incluye la preprocesamiento del texto, la creación de la consulta, la obtención de resúmenes de documentos y la búsqueda de documentos similares. Se proporcionan ejemplos de uso en el código.

## Evaluación de resultados

Dado que se utiliza aprendizaje no supervisado, la evaluación de resultados se basa en el coeficiente de silueta para determinar la calidad de los clusters generados. Además, se realiza una evaluación cualitativa a través de un taller con expertos en bibliotecología, donde se analizan aspectos como la calidad de las recomendaciones, la diversidad y otros criterios relevantes.

## Formulario de satisfacción al usuario

Se ha desarrollado un formulario de satisfacción al usuario que se enviará a los usuarios para evaluar constantemente el desempeño del modelo una vez esté en producción.