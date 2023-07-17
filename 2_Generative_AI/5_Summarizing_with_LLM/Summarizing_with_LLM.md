# Problema 5 Summarizing with LLM

## Introducción

 Un LLM (Large Language Model) es una forma avanzada de Inteligencia Artificial que ha sido entrenada en un vasto corpus de texto. Estos modelos son capaces de generar texto coherente y relevante en respuesta a una variedad de entradas, lo que los hace increíblemente versátiles. Los participantes en este desafío tendrán la oportunidad de explorar y explotar el potencial de los LLM para una de sus aplicaciones más poderosas, el resumen y la extracción de información. Para ello deberán trabajar con un stack de tecnologías modernas y que están en constante desarrollo, como OpenAi, Langchain, Hugginface y bases de datos vectoriales.

## Importancia

 En el mercado actual el trabajo con LLM es de vital importancia para las empresas, desde la creación de chatbots personalizados para atención al cliente, interacción con documentos y bases de datos internas, estructuración de información a partir de datos no estructurados y más.

## Desarrollo del problema técnico

Resumir bibliografías

Los LLM como ChatGPT han demostrado ser una gran herramienta para la investigación y el aprendizaje, sin embargo, el fenómeno llamado alucinaciones plantea dudas sobre su fiabilidad. Particularmente cuando se trata de investigación científica, este es un tema importante a abordar. En el contexto de la investigación científica, los LMM se utilizan para diferentes tareas, tales como: generación de texto, resumen o simplificación de documentos complejos. En los últimos meses se ha visto una proliferación de herramientas que abordan casos de uso de LLM en el contexto de la investigación científica.

La gestión de las referencias bibliográficas es una tarea básica de todo investigador, independientemente de su disciplina. Por eso, el trabajo diario con herramientas como Endnote o Zotero es una actividad muy común en el campo. BibTeX es un formato de archivo para almacenar referencias bibliográficas comúnmente utilizado con LaTeX para escribir documentos científicos. La mayoría de las herramientas de gestión de referencias bibliográficas (como Zotero, Mendeley, Endnote, etc.) admiten BibTeX para exportar y compartir bibliografías.
No es raro que un investigador encuentre en sus carpetas archivos BibTeX, sin el contexto adecuado, de los cuales es difícil saber a priori si contienen alguna información relevante para su investigación actual. Por ello, les puede resultar útil una herramienta que a partir de un archivo BibTeX genere un resumen de todo el contenido incluido en esa bibliografía.

Se le solicita que cree un agente que reciba un archivo BibTeX como entrada y devuelva un informe de texto que:
• resumir todos los temas abordados en los documentos a los que se hace referencia
• resaltar los documentos, investigadores e instituciones considerados más importantes para cada tema

Algunos elementos a tener en cuenta:
• BibTeX es un formato que almacena los metadatos de los documentos (papers, actas de congresos, libros, informes, etc…), el agente debe encargarse de buscar y descargar los archivos, en caso de ser necesario.
• Existe un amplio ecosistema de recursos en Internet en torno a la investigación científica, una lista no exhaustiva incluye:
◦ https://www.crossref.org
◦ https://openalex.org
◦ https://opencitations.net
◦ https://scholar.google.com
◦ https://zenodo.org/
◦ https://figshare.com/

Algunas herramientas que pueden resultarle útiles para crear el agente son:
• LangChain
• Índice Lama
• https://huggingface.co/
• https://www.trychroma.com/
• https://weaviate.io/
• https://faiss.ai/
• https://serpapi.com/
