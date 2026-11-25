---
title: "Diário de bordo 2 — 07/10/2026"
authors:
  - Gabriel Sousa Silva
tags:
  - entre-releases
date: 2026-10-07
---

## 1. Olhando para a release que acabou de ser entregue, o que você diria que funcionou bem e o que não funcionou na sua equipe?

Até o dia 07/10, percebi que a equipe conseguiu avançar bastante na parte técnica. A extração dos cardápios passou a ser testada com PDFs reais, o front começou a consumir os dados da API e o projeto ganhou validações no CI. Também conseguimos organizar melhor a documentação depois da primeira entrega.

O principal problema foi termos deixado algumas definições importantes para perto da release. Os requisitos estavam escritos, mas ainda faltavam critérios de aceitação, regras de negócio e uma ligação mais clara entre o que estava documentado e o que seria implementado. Isso dificultou mostrar a organização do projeto, mesmo com partes do sistema já funcionando.

Também começaram a aparecer diferenças no comprometimento da equipe. Algumas tarefas demoravam para avançar ou ficavam sem uma resposta clara, e quem estava acompanhando mais de perto acabava ajudando em partes que não estavam na divisão inicial. Naquele momento, ainda tentamos resolver isso apenas terminando o que faltava. Não conversamos o suficiente sobre por que o trabalho estava começando a se concentrar em algumas pessoas.

## 2. Como o feedback recebido tem influenciado o que vocês estão fazendo agora?

O feedback da professora mostrou que não bastava listar as funcionalidades. Como fiquei responsável pelos requisitos, revisei a redação para manter o padrão de verbo mais objeto e detalhei os critérios de aceitação e as regras de negócio. Também procurei deixar mais claro como cada requisito poderá ser verificado durante o desenvolvimento.

Um ponto que discutimos foi a avaliação das refeições. Decidimos manter a regra simples: o usuário poderá avaliar a refeição enquanto ela estiver disponível no cardápio daquele dia. A avaliação fica relacionada ao campus, à data e ao tipo de refeição, então uma preparação repetida em outra semana não aparece automaticamente com a média anterior. Essa decisão deixou o requisito mais fácil de entender e testar.

## 3. O que mudou, para você, entre o início da disciplina e este momento — tecnicamente e no seu jeito de trabalhar em equipe?

No começo eu estava mais concentrado em fazer a funcionalidade existir. Agora entendo melhor que também precisamos registrar as decisões, definir como cada requisito será aceito e manter a documentação coerente com o sistema. Passei a observar com mais atenção a relação entre requisitos, regras de negócio, testes e implementação.

Também evoluí no uso de branches e pull requests para organizar as alterações. A revisão dos requisitos virou uma entrega separada, o que facilitou conferir o texto antes de incorporá-lo ao projeto. Para as próximas etapas, quero atualizar a documentação junto com o desenvolvimento, sem deixar esse trabalho acumular perto da entrega.

No trabalho em equipe, comecei a perceber que dividir as áreas no início não era suficiente. Era necessário acompanhar se cada pessoa ainda conseguia cumprir sua parte e avisar quando precisasse de ajuda. Eu ainda tinha dificuldade de cobrar uma resposta sem parecer que estava criando conflito, então muitas vezes preferia assumir uma tarefa. Hoje vejo que conversar sobre isso antes teria sido melhor para todos.
