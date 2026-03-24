---

title: "Week 4"

date: 2026-03-17

image: "/images/week4.png"

subtitle: "ElectroCap Prototype Requirements List"

draft: false
---

<div class="project-card" style="max-width: 400px; min-width: 300px; position: relative; border-radius: 15px; overflow: hidden; box-shadow: 0 10px 20px rgba(0,0,0,0.1);">
    <img src="/images/week4.png" alt="Foto da Week 4" style="width: 100%; height: auto; display: block;">
    <a href="/docs/Requisitos_Prototipo_ElectroCapG22.pdf" download class="project-overlay" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0, 0, 0, 0.7); display: flex; flex-direction: column; justify-content: center; align-items: center; text-decoration: none; transition: opacity 0.3s ease; opacity: 0;">
        <span style="color: white; font-weight: bold; font-size: 1.2em; border: 2px solid white; padding: 10px 20px; border-radius: 30px;">
                📄 Download Requirements List
        </span>
    </a>
</div>

### Do Conceito à Prática: A Definição do ElectroCap
Na semana passada, percebemos que a chave não era recolher todos os dados possíveis, mas sim focar no que é clinicamente relevante, de forma simples e fiável. Agora, o desafio foi transformar essa visão numa estrutura palpável. 
A limitação das teleconsultas atuais é evidente: continuam frequentemente limitadas à comunicação áudio e vídeo, não permitindo ao médico aceder a sinais biomédicos em tempo real. Para colmatar esta falha, avançámos com a definição do Inside Health, um protótipo de telemonitorização biomédica que integra a aquisição sensorial, processamento local, comunicação remota e visualização clínica.

### O Que Vamos Medir?
Para que a teleconsulta deixe de depender apenas da observação visual, definimos que a primeira versão do protótipo terá de adquirir três parâmetros essenciais: frequência cardíaca, frequência respiratória e sons cardiorrespiratórios. 
Mas a tecnologia não pode ser um estorvo... Estabelecemos requisitos não funcionais rigorosos para garantir que o dispositivo é adequado para idosos: tem de ser leve (com menos de 300g), confortável para uso prolongado, possuir uma autonomia de pelo menos 4 horas e transmitir os dados com uma latência inferior a 1 segundo. 

### A Arquitetura do Sistema: O Fluxo Invisível
Como garantimos que a tecnologia funciona em segundo plano sem frustrar quem a usa? Através de uma arquitetura modular bem estruturada. 

Desenhámos o sistema em blocos essenciais:
* **Camada de aquisição:** Os sensores no dispositivo *wearable* (como o ADS1292R para eletrocardiograma e bioimpedância, e microfones MEMS para auscultação).
* **Processamento local:** Um microcontrolador que digitaliza, sincroniza e limpa o ruído dos sinais localmente.
* **Comunicação e Cloud:** O envio rápido e seguro dos dados sem fios para uma infraestrutura remota.
* **Interface Clínica:** Onde a magia acontece para o médico, que recebe informação estruturada e em tempo quase real durante a consulta.

### O Nosso Maior Desafio
O verdadeiro desafio de engenharia não é apenas ligar estes componentes. É conseguir a integração fiável de todo este fluxo num contexto doméstico. Os sinais fisiológicos são fracos e suscetíveis a ruído. Garantir a qualidade do sinal, sincronizar múltiplos sensores, manter a segurança dos dados e, acima de tudo, garantir a simplicidade de uso por pessoas com baixa literacia tecnológica é o que torna este projeto inovador.

### O Que Virá a Seguir?
Temos o "quê" (Requisitos) e o "como" (Arquitetura) bem definidos. O caminho agora é passar da especificação em papel para a integração dos subsistemas de hardware e software, dando os primeiros passos na construção física deste protótipo e testando as nossas escolhas na prática.
