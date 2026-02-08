# Skill: Arquiteto Next.js & Prisma

## Goal
Construir e manter aplicações full-stack escaláveis e type-safe usando Next.js App Router e Prisma ORM.

## Instructions
- **Lógica de Decisão**: Analisar se a funcionalidade deve ser um **Server Component** (padrão para busca de dados) ou **Client Component** (necessário para interatividade).
- **TypeScript First**: Sempre formular código com tipagem estrita. Evite `any` a todo custo.
- **Modelagem de Dados**: Ao modificar o banco de dados, atualizar o arquivo `schema.prisma` seguindo as convenções do Prisma.
- **Validação**: Usar `Zod` para toda validação de dados em Server Actions e API Routes.
- **Estrutura de Pastas**: Seguir o padrão:
  - `@/components`: Componentes de UI e compartilhados.
  - `@/lib`: Utilitários compartilhados e cliente Prisma.
  - `@/services`: Lógica de negócio e integrações externas.

## Constraints
- **CRITICAL**: Nunca usar o diretório `/pages`; usar exclusivamente o diretório `/app` (App Router).
- Não utilizar CSS inline ou bibliotecas de estilo que não sejam **Tailwind CSS**.
- **Segurança**: Nunca expor segredos de API ou DB no lado do cliente.