# IOT - Projeto Irrigação Remota
**| ESP32 | MQTT | HiveMQ | MQTTDashBoard |**

## Protótipo Baseado em IoT Aplicado em Mini Hortas Urbanas
O sistema tem o propósito de monitorar temperaturas do ambiente e atuar caso necessário, ativando a irrigação remotamente. 

## Hardware Usados no Sistema
+ ESP 32 - DEVKIT
+ Sensor DHT11 (Umidade do Ar e Temperatura Ambiente)
+ Sensor Umidade do Solo
+ Módulo ReLê 1 canal 3V
+ válvula Solenoide 12V

## Software Usado 
+ Plataforma HiveMQ - (Broker Nuvem) -> Gerencia o envio das mensagens para os tópicos
+ MQTT DashBoard - (Aplicativo Android) -> Visualização dos Dados e acionamento da válvula

## Bibliotecas utilizadas no código
+ **Wifi.h** -> fornece funcionalidades para conectar o ESP32 a redes Wi-Fi e monitorar o status da conexão
+ **PubSubClient.h** - > implementa um cliente MQTT para comunicação com um Broker MQTTpermitindo que a que ESP32 publique mensagens e assineem tópicos para receber mensagens MQTT. **Publisher/Subscriber**
+ **DHTesp.h** -> Utilizado para facilitar o uso dos sensores DHT
+ **WiFiClientSecure.h** -> Permite estabelecer conexões seguras
+ **ArduinoJson.h** -> Permite que você analise e gere (serialize) dados JSON de maneira eficiente em ambientes com recursos limitados





  



