## ESP32CAM-FLOW-DHT11-MQTT-JSON

Actualizado 23-Agosto-022 por: [Laura Balandrán C.](https://github.com/LauraBalandran/ESP32CAM-FLOW-DHT11-MQTT-JSON)
*Este repositorio contiene archivos utilizados del ejercicio 3 de la clase 16 agosto 022- Diplomado Internet de las Cosas - *Samsung_ Innovation Campus*, que envía datos del sensor DHT11 (temperatura- humedad) por MQTT a NodeRed" y conexiones por API.*

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

  ### Material Necesario

-   Micro controlador ESP32CAM
-   Convertidor de niveles FTDI
-   Cable USB-A a USB-mini
-   Jumpers MM
-   Protoboard
-   Sensor DHT11

**Software necesario**

Para poder hacer funcionar este proyecto, es necesario contar con el siguiente software:

-   [Ubuntu 20.04](https://releases.ubuntu.com/20.04/)
-   [Arduino IDE](https://www.arduino.cc/en/software)
    -   [Gestor de tarjetas ESP32](https://github.com/iotechbugs/esp32-arduino/blob/master/docs/arduino-ide/boards_manager.md)
    -   [Configuración de la IDE de Arduino para trabajar con el ESP32CAM](https://github.com/iotechbugs/esp32-arduino)
    -   [Biblioteca PubSubClient](https://github.com/knolleary/pubsubclient)
-   [Mosquitto MQTT Broker](https://mosquitto.org/download/)
    -   [Listener en puerto 1883 para 0.0.0.0 y conexiones no autentificadas activadas](https://mosquitto.org/man/mosquitto-conf-5.html)
-   [NodeJS](https://nodejs.org/es/)
    -   [NPM](https://www.npmjs.com/)
    -   [NodeRed](https://nodered.org/docs/getting-started/local)
    -   [Nodos Dashboard](https://flows.nodered.org/node/node-red-dashboard)

### [](https://github.com/hugoescalpelo/esp32cam-dht11-g7/blob/main/README.md#material-de-referencia)Material de referencia

En los siguientes enlaces puedes encontrar cursos en la plataforma de edu.codigoiot.com que te permitirán realiar las configuraciones necesarias

-   [Instalación de Virutal Box y Ubuntu 20.04](https://edu.codigoiot.com/course/view.php?id=812)
-   [Configuración de Arduino IDE para ESP32CAM](https://edu.codigoiot.com/course/view.php?id=850)
-   [Instalación de NodeRed](https://edu.codigoiot.com/course/view.php?id=817)
-   [Introducción a NodeRed](https://edu.codigoiot.com/course/view.php?id=278)
-   [Instalación de Mosquitto MQTT](https://edu.codigoiot.com/course/view.php?id=818)

### [](https://github.com/hugoescalpelo/esp32cam-dht11-g7/blob/main/README.md#servicios)Servicios

Para que este ejercicio funcione, necesitas los siguientes servicios

-   [HiveMQ](http://www.mqtt-dashboard.com/). Es un broker publico y no se necesita cuenta
-   [OpenWeatherMap](https://openweathermap.org/). Servicio meteorolígico gratuito. Se requiere cuenta, pero no se requiere ningun pago.

#  Vista previa del resultado

  [Vista previa](https://github.com/LauraBalandran/ESP32CAM-FLOW-DHT11-MQTT-JSON/blob/main/Dashboard-DHT11-SensoresAPI.png) Dashboard Estación de Clima 
  [Vista previa]() Video del funcionamiento General y Dashboard
  [Vista previa]() Video del funcionamiento de la Alerta temperatura