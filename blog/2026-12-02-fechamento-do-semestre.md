---
title: "Diário de bordo 5 — 02/12/2026"
authors: [Gabriel Sousa Silva]
tags: [fechamento-do-semestre]
date: 2026-12-02
---

## 1. O que esta disciplina aproximou do trabalho profissional que você imagina?

No começo, eu pensava mais em dividir as partes do sistema e fazer cada uma funcionar. Durante o semestre, percebi que o trabalho não termina quando o código fica pronto. Tivemos de escrever requisitos, discutir critérios de aceitação, revisar pull requests, corrigir o CI e conferir se a versão publicada era realmente a mesma que estava na `main`. Essa sequência tornou o projeto mais próximo do que imagino encontrar em um trabalho profissional.

O caso da publicação foi o melhor exemplo para mim. A aplicação estava acessível, mas ainda mostrava um commit antigo. Isso deixou claro que dizer que uma entrega está pronta exige alguma evidência. Não basta ter um arquivo de configuração ou um teste passando localmente; é preciso olhar o ambiente real e registrar o resultado.

## 2. Como a colaboração da equipe mudou do início ao fim?

No início, dividimos o trabalho entre extração, backend, banco e frontend. Essa divisão ajudou cada pessoa a começar, mas às vezes dificultou perceber como uma mudança afetava as outras partes. Quando o frontend começou a consumir a API e os dados reais entraram no banco, tivemos de conversar mais sobre formatos, datas, filtros e regras que antes pareciam pertencer a uma parte só.

Mais perto da segunda release, as issues e os pull requests passaram a organizar melhor essas conversas. Também tivemos muitas branches abertas ao mesmo tempo, o que trouxe conflitos e exigiu atualizações frequentes. A equipe melhorou na revisão, mas poderíamos ter mantido a documentação e a rastreabilidade em dia desde as primeiras sprints, em vez de recuperar parte delas perto das entregas.

## 3. O que você faria diferente se pudesse voltar ao início?

Eu começaria pelos requisitos e pelos critérios de aceitação antes de tentar implementar tantas coisas. Também criaria desde o início uma rotina para registrar as reuniões, atualizar cada sprint e testar a publicação. Várias dificuldades apareceram porque o código avançou mais rápido que a documentação ou porque deixamos uma verificação importante para perto da entrega.

Outra mudança seria usar as ferramentas de IA com mais cuidado. Elas ajudaram a revisar textos, criar testes e encontrar caminhos para alguns erros, mas percebi que aceitar uma resposta sem entender o motivo gera mais trabalho depois. Eu tentaria fazer perguntas menores, conferir cada alteração e explicar com minhas palavras o que foi feito antes de levar uma solução para o projeto.

## 4. O que você pretende levar desta experiência?

Quero levar o hábito de trabalhar com mudanças pequenas, branches separadas e testes ligados a problemas reais. Aprendi que cobertura alta é útil, mas precisa incluir banco, concorrência, privacidade, PDFs reais e outros cenários que representam o uso do sistema. Também quero continuar registrando as decisões, porque o código mostra o resultado, mas nem sempre mostra por que a equipe escolheu aquele caminho.

Termino a disciplina com mais segurança em Python, FastAPI, Git, testes e integração contínua. Ao mesmo tempo, passei a reconhecer melhor o que ainda preciso aprender, principalmente sobre publicação e operação de um sistema fora do ambiente local. Para mim, essa diferença entre saber implementar e saber comprovar que algo funciona foi um dos aprendizados mais importantes do projeto.
