# Problema 4: Detección de fraude con identificación de anomalías
## Introducción

La detección de fraude se refiere a la identificación de transacciones o comportamientos anormales por parte de los clientes. A menudo, este comportamiento anómalo puede indicar que algo no está bien con la transacción o el reclamo de seguro, lo que requiere una retención hasta que se pueda realizar una evaluación adicional.

## Importancia

En la era actual de los pagos digitales, donde se realizan trillones de transacciones con tarjeta por día, la detección de fraudes es un desafío importante. De acuerdo con el Índice de Violación de Datos, más de 5 millones de registros se están robando a diario, una estadística preocupante que muestra que el fraude es muy común tanto para los pagos de tipo "Card-Present" como "Card-not Present". Tener un modelo que pueda predecir o anticipar un posible fraude puede marcar una gran diferencia para una empresa, ya que puede ayudar a prevenir pérdidas económicas significativas y mantener la confianza de los clientes.

## Desarrollo del problema técnico

En este hackatón de IA, se les pide a los participantes que desarrollen un modelo de detección de fraude basado en la identificación de anomalías utilizando un conjunto de datos proporcionado. El modelo debe ser capaz de clasificar transacciones en fraudulentas o normales.

#### Tip: Respetar y explicar los supuestos de los modelos utilizados. Tenga en cuenta que el juego de datos es altamente no balanceado.

El juego de datos de prueba (test dataset) para la evaluación de los modelos será el último 10% del juego de datos. Se evaluarán las siguientes métricas: 

Accuracy, Recall, Precision, F1-score, Confusion Matrix, AUC-ROC Curve.

## Información sobre el conjunto de datos.

Este conjunto de datos, proveniente de un instituto anónimo, contiene las siguientes características:

distance_from_home: la distancia desde el hogar donde ocurrió la transacción.

distance_from_last_transaction: la distancia desde donde ocurrió la última transacción.

ratio_to_median_purchase_price: relación del precio de la transacción de compra al precio de compra mediano.

repeat_retailer: si la transacción ocurrió desde el mismo minorista.

used_chip: si la transacción se realizó a través de un chip (tarjeta de crédito).

used_pin_number: si la transacción ocurrió usando un número PIN.

online_order: si la transacción es una orden en línea.

fraud: si la transacción es fraudulenta.
