---

title: "Week 10 - 11"

date: 2026-05-04

image: "/images/comingsoon.JPG"

subtitle: "Heart Rate Implementation"

draft: false
---
### Implementação da Frequência Cardíaca
Estas semanas começámos a montagem física do nosso protótipo implementando o primeiro sinal biomédico que tinhamos proposto adquirir: a Frequência Cardíaca.

### Ligação entre hardware e software
Foram realizados os primeiros testes de comunicação entre os sensores biomédicos e a interface clínica. Trabalhámos na transmissão em tempo real dos dados recolhidos pelo sistema para garantir estabilidade e sincronização entre os diferentes módulos. 

### Desafios enfrentados
O primeiro desafio surgiu logo na ligação do ESP32 ao computador. Inicialmente não conseguíamos programar a placa nem estabelecer comunicação corretamente com o PC, o que atrasou o início dos testes. Depois de analisarmos o problema, conseguimos resolver através da configuração correta da ligação, drivers/porta série e procedimento de upload, permitindo finalmente programar o ESP32.

### O Que Virá a Seguir?
Na próxima semana iremos avançar para a implementação da captação dos sons cardíacos e continuar os testes de integração entre o hardware e a interface clínica.