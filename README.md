# MAVT
Modulo de Atualização de Veículos de Trabalho - MAVT

📝 MAVT é um modulo de atualização idealizado para a atualização e modernização do trator Agrale 4100, visando o melhor aproveitamento da maquina com tecnologias inexistentes em sua época.
<br/> A principal qualidade de maquinas como o Agrale 4100 está na confiabilidade e durabilidade, sendo provadas com sua plena operação, mesmo após anos de uso severo em ambiente agressivo.
<br/> A durabilidade, confiabilidade e não-dependencia são os principais pilares do MAVT: ele deve ser uma ferramenta de auxilio e não um limitador para a operação.
<br/> O projeto foi iniciado em 08/2022 e ainda segue em desenvolvimento

📊 Status Atual: Ideação e pesquisas preliminares

## 🎯 Objetivos:
<!--ts-->

  * ### 🔬Monitorar
    * Temperatura do motor
    * RPM do motor
    * Horas de operação do motor
    * Tensão da bateria
    * Corrente de saída do alternador
    * Corrente de saída para implemento elétrico
    * Geo-localização
    * ...
  * ### 🖥️ Exibir
    * Temperatura do motor
    * RPM do motor
    * Horas de operação do motor
    * Horas restantes para a manutenção 10 horas
    * Horas restantes para a manutenção 50 horas
    * Horas restantes para a manutenção 70 horas (troca de oleo)
    * Horas restantes para a manutenção 200 horas
    * Horas restantes para a manutenção 400 horas
    * Horas restantes para a manutenção 2000 horas
    * Tensão da bateria
    * Alerta de bateria baixa
    * Corrente de saída do alternador
    * Alerta de baixa corrente de saída do alternator
    * Corrente de saída para implemento elétrico
    * Alerta de corrente de saída elevada para o implemento
    * Status da saída para implemento elétrico
    * ...
  * ### 🎚️ Controlar
    * Alimentação do implemento elétrico
    * Direção assistida
    * Embreagem assistida
    * Acelerador assistido
    * Implemento hidráulico assistido
    * ...
  * ### 📡 Enviar
    * Geo-localização
    * ...

<!--te-->

## 📚 Métodos preliminares
<!--ts-->

  * STM32 como co-processador, responsável por:
    * Ler os sensores relacionados a operação do motor
    * Controlar a IHM (display e botões)
    * Controlar assistentes de direção OU controlar módulos de assistentes de direção (expansões)
    * Enviar dados para o ESP32
    * ...
  * ESP32 como processador central
    * Receber dados do co-processador
    * Enviar e receber dados via WiFi
    * Enviar e receber dados via LoRa
    * Enviar e receber geo-localização
    * Gerenciar direção asssitida
    * Se comunicar com modulos de expansão
    * ...

<!--te-->


## ☢️ Desafios
<!--ts-->

 * Exposição ao sol
 * Exposição a terra
 * Eletrônica Automotive-rated
 * Classificação IP67
 * Falta de bateria
 * Cold-crank
 * Segurança de armazenamento de dados críticos (Horímetro)
 * Monitoramento in-loco dos sistemas de direção autônoma/assistida
 * Bloqueio e/ou desacoplamento dos sistemas de direção autônoma/assistida
 * Segurança do equipamento e de terceiros para com a direção autônoma/assistida
 * ...

<!--te-->
