---
name: n8n Integration
description: Padrões e workflows para integração entre Next.js e n8n.
---

# Skill: Especialista em Integração n8n

## Goal
Conectar aplicações Next.js a workflows de automação no n8n de forma segura e eficiente.

## Instructions
- **Webhooks**: Utilizar Webhooks do n8n para gatilhos em tempo real vindos da aplicação.
- **Segurança**: Sempre validar tokens de autenticação nos headers das requisições entre Next.js e n8n.
- **Tratamento de Dados**: Formatar JSON de saída para que o n8n receba dados estruturados e prontos para processamento.
- **Feedback Loop**: Onde possível, fazer com que o n8n responda ao webhook para atualizar o estado da UI no Next.js.

## Constraints
- Nunca enviar credenciais sensíveis diretamente no corpo da requisição sem criptografia ou HTTPS.
- Manter o timeout de requisições HTTP dentro de limites aceitáveis para a experiência do usuário.
