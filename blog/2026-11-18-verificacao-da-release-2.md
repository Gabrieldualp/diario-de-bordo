---
title: "Diário de bordo 4 — 18/11/2026"
authors: [Gabriel Sousa Silva]
tags: [verificacao-release-2]
date: 2026-11-18
---

## 1. Como foi trabalhar na reta final da segunda release?

Nessa reta final, passei boa parte do tempo resolvendo as issues separadamente e conferindo o que já estava pronto. Trabalhei com testes do backend, extração, privacidade, concorrência e leitura dos alérgenos nos PDFs reais. Ter uma branch para cada issue ajudou a não misturar as mudanças, mas também exigiu mais cuidado para atualizar cada branch e resolver diferenças com a `main`.

Nessa fase, a falta de participação de alguns integrantes ficou ainda mais evidente. A divisão original já tinha praticamente desaparecido, e quem estava disponível pegava a próxima issue que precisava ser resolvida. Isso ajudou o projeto a avançar, mas trouxe cansaço e a sensação de que poucas pessoas estavam assumindo a responsabilidade pelo resultado de toda a equipe.

O que mais me chamou atenção foi a quantidade de detalhes que apareceram quando começamos a testar situações menos comuns. A aplicação podia funcionar no caminho normal e ainda falhar com duas avaliações ao mesmo tempo, com uma migração no PostgreSQL ou com um PDF escrito de outra forma. Isso me mostrou que chegar perto da entrega não significa apenas terminar novas funções. Muitas vezes, o trabalho mais importante é conferir se aquilo que já existe continua funcionando em condições diferentes.

## 2. Qual situação desta fase mais contribuiu para o seu aprendizado?

Uma situação marcante foi revisar os pull requests antes de integrar tudo. Alguns testes passavam no SQLite, mas precisavam ser conferidos também no PostgreSQL usado pelo projeto. Em outro caso, tivemos de testar a identidade anônima para garantir que uma pessoa não conseguisse consultar informações de outra. Também usamos PDFs reais dos cinco campi para verificar os alérgenos, em vez de confiar somente em exemplos preparados para os testes.

Essas revisões me fizeram prestar mais atenção no motivo de cada teste. Antes eu olhava principalmente se a cobertura chegava a 100%. Agora entendo melhor que a porcentagem sozinha não garante que os cenários importantes foram escolhidos. Passei a valorizar mais um teste que reproduz um problema real do que vários testes criados apenas para executar linhas do código.

Também aprendi que revisar um pull request não é apenas conferir o código. Em vários momentos, a revisão serviu para entender o que outra pessoa tinha tentado fazer ou para terminar uma mudança que havia ficado incompleta. Quando poucos integrantes acompanhavam essas conversas, as mesmas pessoas acabavam revisando, decidindo e corrigindo. Isso mostrou como a falta de comprometimento de uma parte do grupo afeta até tarefas que parecem individuais.

## 3. O que ainda ficou difícil mesmo com o avanço do projeto?

A publicação continuou sendo a parte em que tive mais dificuldade. Conseguimos ativar o ambiente e deixar frontend, API e banco ligados, mas ainda era necessário conferir se a versão publicada correspondia ao commit mais recente. Foi nessa etapa que percebi como existe diferença entre a aplicação estar acessível e a release estar realmente comprovada.

Também vi que não adianta deixar essa conferência apenas para o final. Para uma próxima entrega, eu começaria a testar a hospedagem mais cedo e registraria cada resultado conforme ele acontecesse. Assim, problemas de acesso, variáveis do ambiente ou versões antigas teriam mais tempo para ser resolvidos e a documentação não precisaria ser reconstruída perto da apresentação.

Faltou também definir com antecedência quem teria acesso ao ambiente e quem ficaria responsável pela verificação final. Quando essa decisão não é tomada, a equipe pode ter o código pronto e ainda depender de uma pessoa que não está disponível naquele momento. Essa dificuldade reforçou para mim que organização, comunicação e comprometimento fazem parte da entrega tanto quanto a implementação.
