---

title: "Week 13 - 14"

date: 2026-05-25

image: "/images/week13.png"

subtitle: "Improvement of Previous Implementations"

draft: false
---
### Melhorias nas Aquisições dos Sinais
Os nossos sinais biomédicos eram recebidos pela interface clínica ainda com muito ruído. Não estando contentes com este resultado dedicámos estas semanas ao aprimoramento da captação destes sinais.

### Desenvolvimento de Parcerias
Durante estas semanas contactámos o Hospital de Portalegre para testarmos o nosso produto. Neste momento ainda estamos a averiguar com a Direção Clínica do Hospital se seria possível realizar nas suas instituições os testes necessários, mas com o encaminhamento direto da Finao BioTech esperamos que a resposta seja positiva.

### Preparação para o EletroCap
Iniciámos também a preparação dos materiais de divulgação para o EletroCap, começando a estruturar o poster científico e o vídeo de apresentação do projeto. Nesta fase organizámos as principais ideias, objetivos e funcionalidades que queremos demonstrar.

### Desafios enfrentados
Quando começámos por desenvolver o código para aquisição do ECG e cálculo da frequência cardíaca fizémo-lo através da deteção direta dos picos do sinal. A ideia inicial era identificar os picos R do ECG e calcular o BPM com base no intervalo entre eles. No entanto, após a reunião com o professor, percebemos que esta abordagem não era a mais robusta, sobretudo devido ao ruído, instabilidade do sinal e possíveis falsas deteções. Por isso, alterámos a estratégia e passámos a usar um método baseado em autocorrelação, analisando uma janela temporal do ECG para estimar o período dominante do sinal cardíaco. Além disso, implementámos filtros para atenuar o ruído, remover variações lentas da baseline e melhorar a qualidade do sinal antes do cálculo da frequência cardíaca.
Ao implementarmos o sistema imbutido do estetoscópio no microfone tivemos outros problemas. O primeiro foi que o microfone dessoldou muitas vezes. Mesmo com cuidado, a pressão do tubo do estetoscópio era significativa e fez com que o microfone não suportasse e saltasse da placa. Foi algo que conseguimos resolver, mas perdemos dias a tentar encontrar uma solução. O segundo problema foi que a membrana que tínhamos era de fraca qualidade, não dava sequer para ouvir o coração. Resolvemos este problema substituindo a membrana por uma que foi fornecida ao grupo.

### Tentativa de Aquisição de novos Sinais
Tentámos ainda implementar a aquisição da Frequência Respiratória e da Auscutação Respiratória.
Rapidamente entendemos que o equipamento comprado para a obtenção da Frequência Respiratória era inadequado para obter o mesmo. Tentámos obter através do eletrocardiograma, pelas variações causadas pela movimentação do tórax no momento da respiração. Como o próprio eletrocardiograma teve muito ruído durante todos os nossos testes e alterações, decidimos que não colocar a Frequência Respiratória como um sinal que era possível obter a partir do nosso sistema porque era difícil encontrar o local exato da variação.
Em relação à obtenção da Auscutação Respiratória tivemos um problema semelhante: o microfone tem um nível de ruído elevado. Reduzimos o máximo que conseguíamos mas, ainda assim, o ruído era muito. Decidimos igualmente não colocar esse parâmetro, porque não o estávamos a obter da melhor forma!

### Problemas existentes
Neste momento, um dos desafios ainda em aberto está relacionado com o armazenamento dos dados no histórico da interface. Estamos a ter algumas dificuldades em garantir que os dados recolhidos ficam corretamente guardados e acessíveis posteriormente na plataforma. Esta parte ainda está em desenvolvimento, mas estamos a tentar resolver através da revisão da comunicação com o backend/base de dados e da forma como os dados são estruturados e enviados.

### O Que Virá a Seguir?
Nas próximas semanas iremos implementar a aquisição da frequência respiratória, um sinal biomédico também muito relevante numa consulta. Estaremos ainda a trabalhar nos materiais de divulgação para o EletroCap.