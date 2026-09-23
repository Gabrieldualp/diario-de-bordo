---
title: "Formação da equipe e primeiros fluxos de integração — 23/09/2026"
authors: [Gabriel Sousa Silva]
tags: [formacao-equipe]
date: 2026-09-23
---

## Descreva como está sendo o processo de organização da sua equipe até agora — papéis, expectativas, primeiras decisões.

No começo, a equipe dividiu os estudos e depois definiu as partes do projeto:
extração, backend, banco e frontend. Fiquei mais responsável pelo backend e
pela extração. Essa divisão ajudou a organizar o trabalho, mas também mostrou
que não basta cada pessoa terminar sua parte isoladamente: precisamos combinar
bem como uma camada conversa com a outra.

Por isso, além do código, registrei o contrato de importação do cardápio e as
mudanças que o banco precisa receber. Quero continuar fazendo isso nas próximas
sprints, principalmente antes de depender da implementação de outra pessoa.

## Que sensações ou pensamentos você tem tido em relação ao início desta disciplina e ao projeto que vocês vão desenvolver?

O projeto parece mais próximo de algo real do que trabalhos que já fiz antes.
O cardápio do RU não tem API e os PDFs podem mudar a qualquer semana, então a
extração foi a parte que mais me deixou atento. Quando testei com os PDFs reais
dos cinco campi e consegui sincronizar os dados, o projeto ficou mais concreto.

Também percebi que testes passando não significam que tudo está resolvido. A
validação com banco e frontend ainda é importante. Quero acompanhar melhor essa
integração para entender como a API funciona para quem vai consumi-la.

## Que conhecimentos, ferramentas ou práticas você sente que já domina, e quais ainda são novidade para você neste momento?

Tenho mais segurança com Python, Git e testes. Nesta fase, pratiquei FastAPI,
Pydantic, `pytest`, Docker e cobertura de testes enquanto trabalhava no backend
e na extração. A parte mais nova para mim foi lidar com PDF: pequenas mudanças
no layout podem alterar completamente a leitura das tabelas.

Também aprendi que Docker e documentação fazem parte da entrega. Configurar o
ambiente e explicar o contrato para o banco foram tão necessários quanto criar
os endpoints. Ainda quero melhorar na revisão e na integração das mudanças da
equipe.
