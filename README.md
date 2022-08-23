
## ESP32CAM-FLOW-DHT11-MQTT-JSON
Actualizado 23-Agosto-022 por: [Laura Balandrán C.](https://github.com/LauraBalandran/ESP32CAM-FLOW-DHT11-MQTT-JSON)
*Este repositorio contiene archivos utilizados del ejercicio 3 de la clase 16 agosto 022- Diplomado Internet de las Cosas - *Samsung_ Innovation Campus*, que envía datos del sensor DHT11 (temperatura- humedad) por MQTT a NodeRed" y conexiones por API*

**Descripción de la Aplicación Estación de Clima:**
**1.-** Obtener información de temperatura y humedad relativa del sensor Dhttps://docs.google.com/spreadsheets/d/1s_RaDnrUEG3wdS_fm7fdf1gNFYoXVmumj7km8WwM8m0/edit?usp=sharingHT11 con el micro controlador ESP32CAM. (*Programa cargado por la IDE Arduino)*

**2.-** Enviar los valores del sensor por MQTT de forma local en JSON, con el objetivo de enviar varias variables en el mismo mensaje.

**3.-** Generar un Flow (*NodeRed*) que obtenga por MQTT los valores enviados por el sensor, realice una gráfica del histórico y muestre indicadores de valores instantáneos.

**4.-** Generar un flow, basado en el [flow 5](https://github.com/hugoescalpelo/flow5-openweather-g7), el cual realice lo siguiente:

 - Obtener valor de temperatura, humedad relativa, Calidad del Aire, Indice Ultra Violeta por API de openweathermap.org 
 - Suscribirse a un Broker MQTT público para poder obtener la información de datos climáticos de todos los alumnos del grupo 7. 
 - Reportar por MQTT los datos obtenidos por API para que puedan ser visualizados por el resto
   de los alumnos.

##  Consideraciones para la API
- Modificar Coordenadas geográficas para obtener los datos climáticos por API

- Modificar la API Key para poder obtener información de openweathermap.org

- Temas MQTT locales y públicos donde se reportan los datos obtenidos por API y por sensores

  

#  Vista previa del resultado

  Dashboard Estación de Clima [Vista previa](https://github.com/LauraBalandran/ESP32CAM-FLOW-DHT11-MQTT-JSON/blob/main/Dashboard-DHT11-SensoresAPI.png)
