# Problema 3: Segmentación de clientes

## Introducción

La segmentación de clientes es el proceso mediante el cual se agrupan los clientes en base a su comportamiento de compra común. Posteriormente, las empresas pueden dirigirse a estos segmentos y personalizar los mensajes de marketing. 

## Importancia

La segmentación de clientes es esencial para una empresa ya que aumenta los ingresos y mejora la satisfacción del cliente. Para un gerente de marketing directo, por ejemplo, resulta sumamente útil utilizar un sistema de inteligencia empresarial para informar sobre sus clientes. Al definir con precisión a sus mejores clientes basándose en parámetros como la Recency, Frecuency y Monetary Value (RFM), puede maximizar el retorno de la inversión en sus acciones de marketing. Un cliente que ordena con frecuencia, lo ha hecho recientemente y ha gastado una suma significativa de dinero es más probable que lo haga en el futuro que otros clientes.

## Desarrollo del problema técnico

En este hackatón de IA, se les desafía a los participantes a desarrollar un modelo que permita realizar una segmentación efectiva de los clientes. Utilizando algoritmos de agrupamiento y reducción de dimensionalidad, deberán lograr visualizar en 2D o 3D los distintos segmentos de clientes.

Además, deberán hacer un análisis RFM, derivando las nuevas variables de los datos de ventas, para determinar:

¿Cuánto tiempo ha pasado desde que el cliente hizo su última orden? (Recency)

¿Cuántas veces ha ordenado en el último año? (Frecuency)

¿Cuál ha sido el valor total de los productos ordenados en ese año? (Monetary Value)

Con base en estas variables, su modelo deberá poder segmentar los clientes en tipos como "nuevo cliente", "cliente muy bueno", etc. y permitir a los gerentes de marketing seleccionar a sus mejores clientes.

#### Tip: Respetar y explicar los supuestos de los modelos utilizados.

## Información sobre el conjunto de datos.

ORDERNUMBER: Número de identificación de la orden.

QUANTITYORDERED: Cantidad de productos que se han ordenado.

PRICEEACH: Precio de cada producto.

ORDERLINENUMBER: Número de línea de la orden.

SALES: Ingresos generados por la venta.

ORDERDATE: Fecha y hora en que se realizó la orden.

STATUS: Estado del envío de la orden (ej. "Enviado").

QTR_ID: Identificador del trimestre del año en que se realizó la orden.

MONTH_ID: Identificador del mes en que se realizó la orden.

YEAR_ID: Año en que se realizó la orden.

ADDRESSLINE1: Primera línea de la dirección del cliente.

ADDRESSLINE2: Segunda línea de la dirección del cliente (puede estar vacía).

CITY: Ciudad del cliente.

STATE: Estado o región del cliente.

POSTALCODE: Código postal del cliente.

COUNTRY: País del cliente.

TERRITORY: Territorio del cliente (puede estar vacío).

CONTACTLASTNAME: Apellido del contacto del cliente.

CONTACTFIRSTNAME: Nombre del contacto del cliente.

DEALSIZE: Tamaño de la transacción (ej. "Pequeño", "Mediano").
