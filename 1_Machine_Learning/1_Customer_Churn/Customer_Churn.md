# Problema 1 Customer Churn.

## Introducción

La rotación de clientes, conocida como "Churn", es un fenómeno que ocurre cuando un cliente decide terminar su relación con una empresa. Esto puede suceder por una variedad de razones, desde la insatisfacción con un producto o servicio, hasta el atractivo de la competencia. En este hackatón, nos centraremos en el problema del churn en una empresa anónima, cuyo objetivo es predecir el comportamiento de los clientes para retenerlos.

## Importancia

El churn es un problema costoso para cualquier empresa. La pérdida de un cliente significa no solo la pérdida de ingresos futuros, sino también la inversión que se hizo para adquirir a ese cliente en primer lugar. Además, atraer a nuevos clientes puede costar hasta cinco veces más que retener a los existentes. Por tanto, tener un modelo que pueda predecir el churn puede ser extremadamente valioso. Un modelo de predicción de churn puede ayudar a una empresa a identificar a los clientes en riesgo de abandonar, permitiendo la implementación de medidas para mejorar su satisfacción y fidelidad, y, por ende, reducir la tasa de churn.

## Desarrollo del problema técnico

Los participantes del hackatón tendrán que desarrollar un modelo de Machine Learning que sea capaz de predecir si un cliente abandonará la empresa en base a una serie de características. Este es un problema de clasificación binaria, donde el objetivo es predecir si un cliente se quedará (Churn = No) o se irá (Churn = Sí).

Se proporcionará un conjunto de datos, en el cual cada fila representa a un cliente y cada columna contiene atributos de los clientes. Los datos incluyen información sobre los servicios a los que cada cliente se ha suscrito, información de la cuenta del cliente, y datos demográficos de los clientes.

#### Tip: Respetar y explicar los supuestos de los modelos utilizados.

El juego de datos de prueba (test dataset) para la evaluación de los modelos será el último 10% del juego de datos. Se evaluarán las siguientes métricas: 

Accuracy, Recall, Precision, F1-score, Confusion Matrix, AUC-ROC Curve.

## Información sobre el conjunto de datos.

Las características disponibles en el conjunto de datos son las siguientes:

•	customerID: ID del cliente

•	gender: Género del cliente

•	SeniorCitizen: Si el cliente es un ciudadano mayor o no

•	Partner: Si el cliente tiene un socio o no

•	Dependents: Si el cliente tiene dependientes o no

•	tenure: Número de meses que el cliente ha estado con la compañía

•	PhoneService: Si el cliente tiene un servicio telefónico o no

•	MultipleLines: Si el cliente tiene múltiples líneas o no

•	InternetService: Proveedor de servicios de internet del cliente

•	OnlineSecurity: Si el cliente tiene seguridad en línea o no

•	OnlineBackup: Si el cliente tiene respaldo en línea o no
•	DeviceProtection: Si el cliente tiene protección de dispositivo o no

•	TechSupport: Si el cliente tiene soporte técnico o no

•	StreamingTV: Si el cliente tiene TV en streaming o no

•	StreamingMovies: Si el cliente tiene películas en streaming o no

•	Contract: El término del contrato del cliente

•	PaperlessBilling: Si el cliente tiene facturación electrónica o no

•	PaymentMethod: El método de pago del cliente

•	MonthlyCharges: La cantidad que se le cobra al cliente mensualmente

•	TotalCharges: La cantidad total que se le ha cobrado al cliente

•	Churn: Si el cliente abandonó 
