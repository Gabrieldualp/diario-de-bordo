---
title: "Diário de bordo 4 — 18/11/2026"
authors: [Gabriel Sousa Silva]
tags: [verificacao-release-2]
date: 2026-11-18
---

## 1. Como foi trabalhar na reta final da segunda release?

Nessa reta final, passei boa parte do tempo resolvendo as issues separadamente e conferindo o que já estava pronto. Trabalhei com testes do backend, extração, privacidade, concorrência e leitura dos alérgenos nos PDFs reais. Ter uma branch para cada issue ajudou a não misturar as mudanças, mas também exigiu mais cuidado para atualizar cada branch e resolver diferenças com a `main`.

O que mais me chamou atenção foi a quantidade de detalhes que apareceram quando começamos a testar situações menos comuns. A aplicação podia funcionar no caminho normal e ainda falhar com duas avaliações ao mesmo tempo, com uma migração no PostgreSQL ou com um PDF escrito de outra forma. Isso me mostrou que chegar perto da entrega não significa apenas terminar novas funções. Muitas vezes, o trabalho mais importante é conferir se aquilo que já existe continua funcionando em condições diferentes.

## 2. Qual situação desta fase mais contribuiu para o seu aprendizado?

Uma situação marcante foi revisar os pull requests antes de integrar tudo. Alguns testes passavam no SQLite, mas precisavam ser conferidos também no PostgreSQL usado pelo projeto. Em outro caso, tivemos de testar a identidade anônima para garantir que uma pessoa não conseguisse consultar informações de outra. Também usamos PDFs reais dos cinco campi para verificar os alérgenos, em vez de confiar somente em exemplos preparados para os testes.

Essas revisões me fizeram prestar mais atenção no motivo de cada teste. Antes eu olhava principalmente se a cobertura chegava a 100%. Agora entendo melhor que a porcentagem sozinha não garante que os cenários importantes foram escolhidos. Passei a valorizar mais um teste que reproduz um problema real do que vários testes criados apenas para executar linhas do código.

## 3. O que ainda ficou difícil mesmo com o avanço do projeto?

A publicação continuou sendo a parte em que tive mais dificuldade. Conseguimos ativar o ambiente e deixar frontend, API e banco ligados, mas ainda era necessário conferir se a versão publicada correspondia ao commit mais recente. Foi nessa etapa que percebi como existe diferença entre a aplicação estar acessível e a release estar realmente comprovada.

Também vi que não adianta deixar essa conferência apenas para o final. Para uma próxima entrega, eu começaria a testar a hospedagem mais cedo e registraria cada resultado conforme ele acontecesse. Assim, problemas de acesso, variáveis do ambiente ou versões antigas teriam mais tempo para ser resolvidos e a documentação não precisaria ser reconstruída perto da apresentação.
