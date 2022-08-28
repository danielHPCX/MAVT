# MAVT
Modulo de Atualização de Veículos de Trabalho

🎯 Objetivo:
🔬Monitorar
<!--ts-->
*Temperatura do motor
*RPM do motor
*Horas de operação do motor
*Tensão da bateria
*Corrente de saída do alternador
*Corrente de saída para implemento elétrico
*Geo-localização
*...
<!--te-->

🖥️ Exibir
Temperatura do motor
RPM do motor
Horas de operação do motor
Horas restantes para a manutenção 10 horas
Horas restantes para a manutenção 50 horas
Horas restantes para a manutenção 70 horas (troca de oleo)
Horas restantes para a manutenção 200 horas
Horas restantes para a manutenção 400 horas
Horas restantes para a manutenção 2000 horas
Tensão da bateria
Alerta de bateria baixa
Corrente de saída do alternador
Alerta de baixa corrente de saída do alternator
Corrente de saída para implemento elétrico
Alerta de corrente de saída elevada para o implemento
Status da saída para implemento elétrico
...
🎚️ Controlar
Alimentação do implemento elétrico
Direção assistida
Embreagem assistida
Acelerador assistido
Implemento hidráulico assistido
...
📡 Enviar
Geo-localização
...

📚 Métodos preliminares
STM32 como co-processador, responsável por:
Ler os sensores
Controlar a IHM (display e botões)
Controlar assistentes de direção OU controlar módulos de assistentes de direção (expansões)
Enviar dados para o ESP32
...
ESP32 como processador central
Receber os dados do co-processador
...

☢️ Desafios
Exposição ao sol
Exposição a terra
Eletrônica Automotive-rated
Classificação IP67
Falta de bateria
Cold-crank
Segurança de armazenamento de dados críticos (Horimetro)
Monitoramento in-loco dos sistemas de direção autônoma/assistida
Bloqueio e/ou desacoplamento dos sistemas de direção autônoma/assistida
Segurança do equipamento e de terceiros para com a direção autônoma/assistida
...
