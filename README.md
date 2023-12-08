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
+ **WebServer.h** -> Facilita na criação de um servidor web no ESP32

## Ajustes na Área de Trabalho.
Verifique se a IDE Arduino está reconhecendo a sua placa na aba ferramentas > Gerenciador de placas. Após instalar as bibliotecas usando o gerenciador de bibliotecas. Carregue o código fonte em seu microcontrolador.

##Ajustando o Broker
Após criação de conta no broker Hivemq é disponibilizado um cluster free. Entre no gerenciador de conta e atente-se as  configurações de conexão, essa, informa a porta disponibilizada e a url de acesso. Obs: a URL e porta deverão ser inseridas no código fonte para conexão entre a placa e o ESP. Crie uma credencial de acesso na aba "Access Management" e em seguida crie tópicos para serem alimentados na aba web cliente.








Se for replicar o código fielmente, consulte os pinos utilizados no código e faça a conexão com os conectores dos sensores. O pino usado no sensor de umidade do solo é o Analógico





  



