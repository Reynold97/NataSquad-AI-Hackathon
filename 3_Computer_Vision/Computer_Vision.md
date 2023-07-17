# Problema 8 Computer Vision.

## Introducción

La visión por computadora es un campo de la inteligencia artificial que se ocupa de capacitar a los sistemas para que comprendan y procesen imágenes y videos de la misma manera que lo hacen los seres humanos. En este caso, los participantes deberán desarrollar modelos de clasificación de imágenes capaces de identificar con precisión el estado de frescura de diferentes tipos de frutas y verduras.

## Importancia

La capacidad de contar con un modelo que pueda anticipar la frescura de las frutas y verduras tiene importantes consecuencias para las empresas. En el sector alimentario, la calidad de los productos es fundamental tanto para la satisfacción del cliente como para la seguridad alimentaria. Contar con un sistema automatizado que pueda detectar y clasificar de manera precisa los alimentos frescos y en mal estado permite a las empresas tomar decisiones informadas sobre el manejo de la cadena de suministro, la gestión del inventario y la entrega de productos de calidad a los consumidores. Además, contribuye a reducir el desperdicio de alimentos al identificar y descartar los alimentos en mal estado de manera oportuna.

## Desarrollo del problema técnico

Los participantes deberán utilizar un conjunto de datos que contiene una amplia variedad de imágenes de frutas y verduras capturadas en diferentes condiciones de iluminación, ángulos y fondos. Cada imagen está etiquetada para indicar si el artículo es fresco o podrido/pasado. El desafío consiste en desarrollar un modelo de clasificación de imágenes que pueda identificar correctamente el estado de frescura de los diferentes tipos de productos.
Los participantes deberán entrenar y evaluar sus modelos de aprendizaje profundo, como redes neuronales convolucionales (CNN), para lograr la máxima precisión en la clasificación. Se anima a explorar y utilizar modelos pre entrenados y realizar ajuste fino. El objetivo final es desarrollar un modelo de clasificación de imágenes preciso y robusto que pueda aplicarse en diversas aplicaciones.

#### Tip: Respetar y explicar los supuestos de los modelos utilizados.

El juego de datos de prueba (test dataset) para la evaluación de los modelos será el último 10% del juego de datos. Se evaluarán las siguientes métricas: 

Accuracy, Recall, Precision, F1-score, Confusion Matrix, AUC-ROC Curve.

## Información sobre el conjunto de datos.

Variedad de imágenes: el conjunto de datos contiene una cantidad sustancial de imágenes, con una variación significativa en las condiciones de iluminación, los ángulos y los fondos. Esta diversidad ayuda a imitar escenarios del mundo real y desafía los modelos de clasificación para que sean sólidos y precisos en diversas condiciones.

Niveles de frescura: el conjunto de datos proporciona una distinción clara entre los estados fresco y podrido/rancio, lo que permite el entrenamiento de modelos capaces de identificar con precisión el nivel de descomposición en frutas y verduras.

Anotación: Cada imagen en el conjunto de datos está cuidadosamente etiquetada con las anotaciones apropiadas que indican si el elemento está fresco o podrido/rancia. Esto permite el aprendizaje supervisado y facilita el desarrollo de modelos de clasificación.

Imágenes de alta calidad: el conjunto de datos incluye imágenes de alta resolución capturadas con cámaras de nivel profesional. Las imágenes se editan meticulosamente para garantizar la claridad y eliminar el ruido, lo que brinda una base sólida para entrenar modelos de clasificación confiables.

Gran escala: con miles de imágenes disponibles, el conjunto de datos ofrece un volumen significativo de datos adecuados para entrenar modelos de aprendizaje profundo. Esto permite una capacitación y validación más amplias, lo que lleva a modelos de clasificación más sólidos y precisos.