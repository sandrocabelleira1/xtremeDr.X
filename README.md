# Xtreme Dr. X — assistente de instalação com IA

Aplicação web para apoiar a instalação e o diagnóstico do Quickshifter Xtreme. O assistente responde perguntas e analisa fotos e vídeos enviados pelo usuário, combinando IA generativa com uma interface de chat.

> **Status do código:** este repositório público apresenta o estudo de caso. O código da aplicação está em revisão de segurança antes de ser publicado.

## O que o projeto demonstra

- Fluxos de IA com entradas e saídas estruturadas usando Genkit e Gemini 2.5 Flash.
- Análise multimodal de imagens e vídeos com contexto de conversa.
- Aplicação web full stack com Next.js e TypeScript.
- Autenticação de usuários e persistência de dados com Firebase Auth e Firestore.
- Checkout com Stripe e processamento de webhook com validação de assinatura.

## Arquitetura resumida

1. A interface Next.js recebe a pergunta e, opcionalmente, uma mídia.
2. Um fluxo Genkit organiza o contexto e encaminha a solicitação ao Gemini.
3. O resultado estruturado volta para o chat.
4. Firebase Auth e Firestore cuidam das contas e dos dados do produto.
5. Stripe processa a compra de créditos; o webhook confirma o evento antes da atualização correspondente.

## Tecnologias

- Next.js 15, React e TypeScript
- Genkit e Gemini 2.5 Flash
- Firebase Auth, Firestore e Firebase Admin
- Stripe Checkout e Webhooks
- Tailwind CSS e componentes Radix UI

## Aprendizados e próximos passos

Este projeto explora como integrar um modelo generativo a uma experiência de produto real, incluindo contexto multimodal, autenticação, persistência e pagamentos. Antes de liberar o código-fonte, estou revisando a autorização server-side do checkout e as regras de atualização de créditos no Firestore.

## Sobre a demonstração

Este repositório é uma apresentação técnica do projeto. Uma demonstração pública e o código-fonte serão adicionados após a revisão de segurança e a preparação dos materiais visuais.
