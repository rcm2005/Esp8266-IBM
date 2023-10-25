# Projeto IoT com ESP8266 e MQTT
<img src="https://github.com/Pontessxx/Esp8266-IBM/blob/main/img-capa.jpg" style="transform: rotate(90deg);">
Este projeto é uma implementação de Internet das Coisas (IoT) usando o ESP8266 para controlar um dispositivo e coletar dados de um sensor. A comunicação entre o dispositivo e uma plataforma de backend é realizada através do protocolo MQTT.
<br>
<br>
link da demonstração : https://youtu.be/rdE8vRlFGoU

## Visão Geral

O objetivo deste projeto é controlar um dispositivo, neste caso, um LED RGB, com base na leitura de um sensor de poluição. A cor do LED muda de acordo com a qualidade do ar medida pelo sensor, e o estado do LED é publicado em um tópico MQTT para que seja acompanhado em tempo real.

## Recursos Necessários

### Hardware
- ESP8266 (NodeMCU)
- Sensor de Poluição
- LED RGB
- LED Indicador de Estado
- Cabos e protoboard para conexões

### Software
- Arduino IDE ou outra plataforma de desenvolvimento compatível com o ESP8266
- Bibliotecas necessárias, como a biblioteca `PubSubClient` para MQTT
- Servidor MQTT na plataforma de backend

## Configuração do Projeto

### Conexão do Hardware

O hardware do projeto é montado da seguinte forma:

- O sensor de poluição está conectado a uma porta analógica do ESP8266 (A0).
- O LED RGB é conectado a três portas digitais do ESP8266 (D1, D2, D3).
- Um LED indicador de estado é conectado a uma porta digital do ESP8266 (D4).

### Configuração do Software

- Você deve configurar suas credenciais de rede Wi-Fi (SSID e senha) no código.
- Configure as informações do seu servidor MQTT, incluindo endereço e porta.
- Defina os tópicos MQTT para subscrição e publicação.

## Funcionalidades do Projeto

O projeto possui as seguintes funcionalidades:

- Leitura do sensor de poluição para medir a qualidade do ar.
- Controle do LED RGB com base na leitura do sensor: vermelho para alta poluição, amarelo para poluição moderada e verde para baixa poluição.
- Publicação do estado do LED no tópico MQTT `/TEF/lamp118/attrs/color`.
- Publicação do estado do dispositivo no tópico MQTT `/TEF/lamp118/attrs`.
- Acompanhamento em tempo real do estado do dispositivo na plataforma de backend.

## Uso do Protocolo MQTT

O protocolo MQTT é usado para a comunicação entre o dispositivo e a plataforma de backend. Ele permite o monitoramento em tempo real do estado do dispositivo e a publicação de informações do sensor.

## Como Executar o Projeto

1. Carregue o código no ESP8266 usando a plataforma de desenvolvimento Arduino IDE.
2. Conecte o hardware conforme as instruções fornecidas na seção de configuração do projeto.
3. Monitore a saída no Serial Monitor da Arduino IDE para depuração e verificação do funcionamento do projeto.

## Instruções Adicionais

- Certifique-se de configurar uma plataforma de backend MQTT compatível para receber as mensagens do dispositivo.
- Mantenha as credenciais de segurança do dispositivo e da plataforma MQTT seguras.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para fazer melhorias ou adições a este projeto.

## Autores

- RM 98036 Henrique Pontes Oliveira
- RM 98460 Felipe Capriotti da Silva Santos
- RM 99679 Gustavo Kawamura Christofani
- RM 550908 Vinicius Santos Yamashita de Farias
- RM 99874 Rafael Carvalho Mattos


## Autores

- RM 98036 Henrique Pontes Oliveira
- RM 98460 Felipe Capriotti da Silva Santos
- RM 99679 Gustavo Kawamura Christofani
- RM 550908 Vinicius Santos Yamashita de Farias
- RM 99874 Rafael Carvalho Mattos

## Licença

Este projeto é licenciado sob a [Sua Licença] - veja o arquivo [LICENSE.md](LICENSE.md) para detalhes.




