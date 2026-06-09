---

title: "Week 12"

date: 2026-05-11

image: "/images/comingsoon.JPG"

subtitle: "Heart Sound Implementation"

draft: false
---
### Aquisição dos Sons Cardíacos
Esta semana foi dedicada ao desenvolvimento do módulo de captação dos sons cardíacos. Começámos a testar diferentes abordagens para captar os sinais acústicos do coração com maior clareza e menor ruído possível.

### Processamento e Qualidade do Sinal
Foram realizados testes de filtragem e processamento do sinal áudio captado, permitindo melhorar a qualidade dos sons cardíacos obtidos. Este processo foi essencial para reduzir interferências externas e aumentar a precisão do sistema. Contudo, neste momento ainda não temos uma qualidade como a que desejávamos.

### Integração com a Interface Clínica
Iniciámos também a integração dos sons cardíacos na interface clínica, permitindo a sua visualização e reprodução em simultâneo com os restantes sinais biomédicos monitorizados.

### Desafios enfrentados
Um desafio importante e complicado foi a transmissão do áudio cardíaco para a interface. Tivemos de testar várias abordagens até encontrar uma solução adequada para enviar o som em tempo real. A dificuldade principal foi conseguir transmitir áudio com baixa latência e num formato compatível com a interface, sem comprometer o funcionamento dos restantes sensores.
Durante os testes com o microfone, percebemos também que apenas o microfone não era suficiente para captar o som cardíaco com a qualidade pretendida. O sinal captado tinha muito ruído ambiente e ruído de contacto, tornando difícil distinguir claramente os sons cardíacos. Para resolver este problema, concluímos que seria necessário usar um estetoscópio acoplado mecanicamente ao microfone, de forma a melhorar a captação do som cardíaco e reduzir o ruído exterior. Assim, comprámos um estetoscópio para criar esse acoplamento mecânico e tornar a auscultação mais eficaz.

### O Que Virá a Seguir?
Nas próximas semanas iremos continuar a melhorar a aquisição dos sinais biomédicos já implementados e começar a implementar novos sinais, tal como a Frequência Respiratória e a aquisição de Sons Respiratórios. Paralelamente, começaremos a desenvolver os materiais de divulgação.