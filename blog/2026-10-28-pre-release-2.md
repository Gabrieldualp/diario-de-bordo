---
title: "Diário de bordo 3 — 28/10/2026"
authors:
  - Gabriel Sousa Silva
tags:
  - pre-release-2
date: 2026-10-28
---

## 1. Compare como você está se sentindo na preparação desta segunda entrega com a forma como se sentiu na primeira.

Na preparação da primeira entrega, eu estava mais preocupado em conseguir mostrar alguma coisa funcionando. Como várias partes ainda estavam separadas, parecia que qualquer problema perto da data poderia impedir a apresentação do projeto. Agora estou um pouco mais tranquilo porque já temos uma base mais concreta: o frontend consulta a API, as avaliações e reclamações começaram a ser integradas e os testes ajudam a perceber quando uma mudança quebra outra parte.

Mesmo assim, esta segunda preparação trouxe outro tipo de preocupação. Antes, o desafio era fazer as partes existirem; agora precisamos garantir que elas funcionem juntas e que a documentação diga a mesma coisa que o sistema realmente faz. Isso ficou claro quando revisamos as issues de sincronização e publicação. Ter o código, o Docker e os testes prontos não significa que a aplicação já esteja publicada ou que uma rotina esteja realmente executando a cada seis horas. Passei a prestar mais atenção nessa diferença entre uma funcionalidade preparada e uma funcionalidade comprovada em uso.

Comparando as duas entregas, sinto que agora consigo enxergar melhor o que ainda falta, sem achar que todo erro significa que o projeto está dando errado. Quero manter esse cuidado de testar e registrar as limitações, mas também evitar deixar a integração e a verificação do ambiente para os últimos dias.

Ao mesmo tempo, fiquei mais preocupado com a participação da equipe. A divisão entre as áreas já não funcionava como no começo, porque algumas pessoas estavam menos presentes e as tarefas pendentes passavam para quem ainda acompanhava o projeto. Isso aumentou a sensação de que qualquer ausência perto da entrega poderia sobrecarregar ainda mais quem estava tentando fechar as issues.

## 2. Descreva como as decisões técnicas estão sendo tomadas na sua equipe nesta fase — quem decide, como se chega a um consenso.

Nesta fase, as decisões ficaram mais ligadas às issues e aos critérios de aceitação. Em vez de alguém simplesmente implementar uma ideia, primeiro tentamos entender o que o requisito realmente pede e qual solução cabe no tempo da disciplina. Um exemplo foi a avaliação das refeições. Discutimos se uma refeição repetida em outra semana deveria carregar a média anterior, mas decidimos manter a avaliação ligada ao campus, à data e ao tipo de refeição. Essa opção foi mais simples e evitou misturar experiências de dias diferentes.

Também percebi que as decisões estão ficando mais visíveis nos pull requests. As mudanças de requisitos, horários, identidade anônima, filtros e sincronização foram separadas em branches próprias. Isso facilitou comparar o que foi alterado, revisar os testes e corrigir problemas do CI antes de levar tudo para a `main`.

Por outro lado, nem sempre o consenso envolvia realmente o grupo inteiro. Quando alguns integrantes não respondiam ou não acompanhavam as issues, quem estava presente precisava escolher uma solução e continuar para não perder o prazo. As decisões acabaram ficando concentradas nas mesmas pessoas. Os registros nos documentos ajudaram a explicar o caminho seguido, mas não substituíram a participação que faltou durante a discussão.

Para mim, o consenso tem funcionado melhor quando a pergunta é concreta. Escolher entre uma solução simples e outra mais completa fica mais fácil quando olhamos para os critérios, o prazo e o que conseguimos testar. Nas próximas decisões, quero continuar registrando esse motivo, porque só o código final nem sempre explica o que a equipe discutiu.

## 3. Que lacunas técnicas ainda te incomodam, e o que você tem feito, ou pretende fazer, a respeito?

A principal lacuna que ainda me incomoda é a parte de publicação e operação do sistema. Hoje me sinto mais confortável com Python, FastAPI, testes e Git, mas ainda tenho menos segurança quando entram hospedagem, variáveis secretas, workflows agendados e a comunicação entre frontend, backend e banco fora do ambiente local. Trabalhar nas issues de última importação, publicação HTTPS e sincronização automática me ajudou a entender melhor esses pontos, principalmente a necessidade de não colocar tokens no repositório e de guardar evidências das execuções.

Outra dificuldade é não confiar apenas no resultado verde dos testes. Tivemos casos em que a cobertura estava em 100%, mas o formato de um PDF real ainda causava problema. Também vimos que uma URL planejada para publicação podia continuar retornando erro porque o ambiente ainda não havia sido ativado. Isso me mostrou que testes automatizados são importantes, mas precisam ser acompanhados por uma verificação próxima da situação real.

Tenho tentado diminuir essas lacunas lendo os logs do CI, entendendo por que cada workflow existe e escrevendo testes para os limites dos requisitos, não só para o caminho que funciona. Também quero compreender melhor cada alteração antes de aceitar uma solução sugerida por uma ferramenta ou por IA. Para a próxima etapa, pretendo acompanhar uma publicação completa e uma execução real da sincronização, desde a configuração dos segredos até a conferência dos dados na interface.

Essa etapa também depende de organização entre as pessoas, porque nem todos possuem os mesmos acessos ou conhecem a configuração da hospedagem. Quando não existe um responsável claro e alguém se ausenta, até uma tarefa pequena pode ficar parada. Por isso, além de aprender a parte técnica, quero melhorar a forma de combinar responsabilidades e registrar quem pode concluir cada etapa.
