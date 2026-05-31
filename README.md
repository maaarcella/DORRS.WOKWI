# 🔐 Sistema Inteligente de Controle de Portas com ESP32, Servomotores e Display OLED

## Descrição

Este projeto consiste em um sistema de controle de acesso desenvolvido com ESP32 e MicroPython. A aplicação permite selecionar e controlar a abertura e o fechamento de três portas diferentes utilizando botões físicos, servomotores, LEDs indicadores e um display OLED para exibição das informações em tempo real.

Cada porta representa um ambiente específico da instituição, simulando um sistema automatizado de controle de acesso para laboratórios, salas administrativas e áreas restritas.

## Funcionalidades

* Seleção de três portas independentes;
* Controle de abertura e fechamento através de servomotores;
* Exibição das informações em display OLED;
* Indicação visual do status das portas;
* Controle por botões físicos;
* LEDs de sinalização para portas abertas e fechadas;
* Atualização em tempo real do estado de cada porta.

## Ambientes Controlados

### Porta 1

* Laboratório de Informática

### Porta 2

* Sala dos Professores

### Porta 3

* Almoxarifado

## Componentes Utilizados

* ESP32
* Display OLED SSD1306 (128x64)
* 3 Servomotores
* 4 Botões Push Button
* 2 LEDs indicadores
* Resistores
* Protoboard
* Jumpers

## Tecnologias Utilizadas

* MicroPython
* Biblioteca SSD1306
* Comunicação I2C
* Controle PWM
* GPIO (Entradas e Saídas Digitais)

## Como Funciona

O sistema opera através de quatro botões:

### Botão Verde

Seleciona a Porta 1 (Laboratório de Informática).

### Botão Azul

Seleciona a Porta 2 (Sala dos Professores).

### Botão Roxo

Seleciona a Porta 3 (Almoxarifado).

### Botão Vermelho

Realiza a abertura ou fechamento da porta selecionada.

Após selecionar uma porta, o display OLED exibe:

* Número da porta;
* Nome do ambiente;
* Situação atual da porta.

Quando o botão vermelho é pressionado:

* Se a porta estiver trancada, o servomotor libera o acesso e o status muda para "Aberta";
* Se a porta estiver aberta, o servomotor retorna à posição inicial e o status muda para "Trancada".

## Sinalização por LEDs

### LED Verde

Indica que a porta está aberta.

### LED Vermelho

Indica que a porta está trancada.

## Conceitos Aplicados

* Sistemas embarcados;
* Automação de acesso;
* Controle de servomotores via PWM;
* Comunicação I2C;
* Manipulação de displays OLED;
* Estruturas condicionais;
* Dicionários em Python;
* Programação em MicroPython;
* Integração entre hardware e software.

## Aprendizados

Durante o desenvolvimento deste projeto foram aplicados conhecimentos relacionados a:

* Programação de microcontroladores ESP32;
* Controle de servomotores;
* Utilização de displays OLED;
* Automação de processos;
* Controle de estados;
* Desenvolvimento de sistemas inteligentes embarcados.

## Melhorias Futuras

* Controle por senha;
* Leitor RFID;
* Controle via aplicativo móvel;
* Registro de acessos em banco de dados;
* Integração com Wi-Fi;
* Sistema de monitoramento remoto;
* Cadastro de usuários autorizados.

## Autor

Projeto desenvolvido para fins acadêmicos, explorando conceitos de automação, controle de acesso, eletrônica digital e programação embarcada utilizando ESP32 e MicroPython.
