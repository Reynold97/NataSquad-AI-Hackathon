# Problema 2: Time Series Forecasting

## Introducción 

El pronóstico de series temporales es una técnica analítica esencial que se basa en el uso de datos históricos para predecir futuros comportamientos. Este método se basa en la premisa de que las tendencias y patrones observados en el pasado pueden ayudar a predecir eventos futuros. En este problema, se pide a los participantes que apliquen este enfoque para predecir el horizonte de pronóstico 'H', es decir, los siguientes períodos (días, horas, semanas, etc.) basándose en los patrones de los datos históricos de demanda de electricidad.

## Importancia 

El pronóstico de series temporales es de vital importancia para las organizaciones, ya que las decisiones estratégicas, la contratación de nuevos empleados, la compra de materiales a través de la cadena de suministro, entre otros, dependen en gran medida de la precisión de estos pronósticos. En el sector energético, por ejemplo, anticipar correctamente la demanda de electricidad puede permitir una gestión más eficiente de los recursos y un ahorro significativo. Por otro lado, un pronóstico inexacto puede llevar a una mala gestión, a un exceso de producción o a la falta de suministro, lo que podría resultar en pérdidas económicas considerables. Por lo tanto, el desarrollo de modelos precisos para pronosticar la demanda de electricidad puede tener un impacto significativo y positivo en la eficiencia operacional y en la rentabilidad de las empresas.

## Desarrollo del problema técnico 

Para este problema, los participantes recibirán un conjunto de datos tomado del National Grid ESO, el operador del sistema eléctrico de Gran Bretaña. Este conjunto de datos incluye información sobre la demanda de electricidad en Gran Bretaña desde el año 2009. Los datos se actualizan dos veces por hora, lo que se traduce en 48 entradas por día. Esta frecuencia de actualización hace que el conjunto de datos sea especialmente adecuado para el pronóstico de series temporales.

Los participantes deberán usar estos datos para desarrollar un modelo que pueda predecir la demanda de electricidad para el año 2023. La variable objetivo es TSD (Transmission System Demand). También se les insta a considerar factores externos que puedan influir en la demanda de electricidad, como las fluctuaciones de temperatura y otras variables climáticas, aunque no es necesario.

#### Tip: Respetar y explicar los supuestos de los modelos utilizados.

El juego de datos de prueba (test dataset) para la evaluación de los modelos será el fragmento de serie temporal correspondiente al 2023. Se recomienda hacer un pronóstico de todo el año 2023. Se evaluarán las siguientes métricas: 

MSE, RMSE, MAE, Análisis de residuos.

## Información sobre el conjunto de datos.

El conjunto de datos consta de tres tipos de archivos:
Historic_demand_year_20xx.csv: demanda de electricidad en ese año
Historic_demand_year_2009_2022.csv: todos los conjuntos de datos anuales combinados en uno
Historic_demand_year_2009_2022_noNaN.csv: igual que arriba, pero los valores de NaN se han eliminado y la fecha incluye la hora en lugar de solo el día

Columnas
Las columnas en el conjunto de datos son:

SETTLEMET_DATA: fecha en formato dd/mm/aaaa

SETTLEMENT_PERIOD: período de media hora para el resultado histórico ocurrido

ND (Demanda Nacional). La Demanda Nacional es la suma de la generación medida, pero excluye la generación requerida para satisfacer la carga de la estación, el bombeo de almacenamiento por bombeo y las exportaciones de interconectores. La demanda nacional se calcula como la suma de la generación basada en la medición de generación operativa de National Grid ESO. Medido en MW.

TSD (Demanda del Sistema de Transmisión). La Demanda del Sistema de Transmisión es igual a la ND más la generación adicional requerida para satisfacer la carga de la estación, el bombeo de almacenamiento y las exportaciones de interconectores. Medido en MW.

INGLATERRA_GALES_DEMANDA. Demanda de Inglaterra y Gales, como ND anterior pero sobre la base de Inglaterra y Gales. Medido en MW.

EMBEDDED_WIND_GENERATION. Esta es una estimación de la generación eólica GB de parques eólicos que no tienen instalado medidores del Sistema de Transmisión. Estos parques eólicos están integrados en la red de distribución y son invisibles para National Grid ESO. Su efecto es suprimir la demanda de electricidad durante los períodos de viento fuerte. Se desconoce la salida real de estos generadores, por lo que se proporciona una estimación basada en el mejor modelo de National Grid ESO. Medido en MW.

CAPACIDAD_EÓLICA_INTEGRADA. Esta es la mejor vista de National Grid ESO de la capacidad eólica integrada instalada en GB. Esto se basa en información disponible públicamente recopilada de una variedad de fuentes y no es la opinión definitiva. Es consistente con la estimación de generación proporcionada anteriormente. Medido en MW

GENERACIÓN_SOLAR_INTEGRADA. Esta es una estimación de la generación solar GB a partir de paneles fotovoltaicos. Estos están integrados en la red de distribución y son invisibles para National Grid ESO. Su efecto es suprimir la demanda de electricidad durante los períodos de alta radiación. Se desconoce la salida real de estos generadores, por lo que se proporciona una estimación basada en el mejor modelo de National Grid ESO. Medido en MW.

CAPACIDAD_SOLAR_INTEGRADA. Como capacidad eólica embebida arriba, pero para generación solar. Medido en MW.

NON_BM_STOR (Reserva Operativa a Corto Plazo del Mecanismo de No Equilibrio). Para unidades que no están incluidas en la definición del generador ND. Esto puede ser en forma de generación o reducción de la demanda. Medido en MW.

BOMBEO_ALMACENAMIENTO_BOMBEO. La demanda por bombeo en las unidades de almacenamiento de hidrobombas; el -ve significa carga de bombeo.

IFA_FLOW (Flujo de interconector IFA). El flujo encendido en el respectivo interconector. -ve significa exportar energía desde GB; +ve significa potencia de importación en GB. Medido en MW.

IFA2_FLOW (Flujo de interconector IFA). El flujo en el respectivo interconector. -ve significa exportar energía desde GB; +ve significa potencia de importación en GB. Medido en MW.

MOYLE_FLOW (FLUJO del interconector Moyle). El flujo en el respectivo interconector. -ve significa exportar energía desde GB; +ve significa potencia de importación en GB. Medido en MW.

EAST_WEST_FLOW (flujo de interconexión este-oeste). El flujo en el respectivo interconector. -ve significa exportar energía desde GB; +ve significa potencia de importación en GB. Medido en MW.

NEMO_FLOW (flujo del interconector Nemo). El flujo en el respectivo interconector. -ve significa exportar energía desde GB; +ve significa potencia de importación en GB. Medido en MW.

NSL_FLOW (Flujo de interconexión del enlace del Mar del Norte). El flujo en el respectivo interconector. -ve significa exportar energía desde GB; +ve significa potencia de importación en GB. Medido en MW.

ELCLINK_FLUJO. Blanco

