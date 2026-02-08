---
name: Security & LGPD
description: Segurança da informação, proteção de dados e conformidade com a LGPD.
---

# Skill: Especialista em Segurança e LGPD (Privacy by Design)

## Goal
Implementar sistemas seguros desde a concepção, protegendo contra vulnerabilidades comuns e garantindo a privacidade dos dados pessoais conforme a LGPD.

## Instructions

### 1. Segurança de Código
- **Sanitização**: Sempre sanitizar strings de busca e inputs de usuários antes de processar ou exibir.
- **Prevenção de Injeção**: Utilizar o Prisma Client para prevenir SQL Injection por padrão. Nunca usar interpolação de strings em queries manuais.
- **Headers de Segurança**: Configurar headers como CSP (Content Security Policy) e HSTS para proteger o navegador do usuário.

### 2. Conformidade LGPD
- **Minimização de Dados**: Coletar apenas o estritamente necessário para a finalidade do sistema.
- **Criptografia**: Dados sensíveis (CPFs, e-mails, endereços) devem ser criptografados em repouso e em trânsito (HTTPS).
- **Gestão de Consentimento**: Garantir que as interfaces de coleta de dados informem claramente a finalidade e obtenham consentimento quando necessário.

### 3. Tratamento de Erros Seguro
- **Logs Internos**: Erros de banco de dados ou sistemas devem ser logados no servidor, mas nunca exibidos detalhadamente para o usuário final (evitar vazamento de stack traces).
- **Mensagens Genéricas**: No front-end, usar mensagens de erro genéricas ("Algo deu errado") para evitar que atacantes descubram a estrutura do sistema.

## Constraints
- **CRITICAL**: Nunca armazenar senhas em texto puro. Use hashing seguro (ex: `bcrypt` ou `argon2`).
- **Segredos**: Nunca commitar chaves de API, segredos do DB ou JWT secrets no repositório. Use variáveis de ambiente (`.env.local`).
- **Auditabilidade**: Manter logs de quem acessou/modificou dados sensíveis (Trilha de Auditoria).
