---
name: SEO Best Practices
description: Diretrizes essenciais para otimização de mecanismos de busca (SEO) em aplicações Next.js.
---

# Skill: Especialista em SEO Next.js

## Goal
Garantir que todas as páginas e conteúdos da aplicação sejam perfeitamente indexáveis, relevantes e otimizados para mecanismos de busca, maximizando a visibilidade orgânica.

## Instructions

### 1. Metadados e Cabeçalhos
- **Metadata API**: Utilizar a Metadata API do Next.js (`generateMetadata` ou objeto `metadata` estático).
- **Títulos e Descrições**: Cada página deve ter um título único (50-60 caracteres) e uma meta description única (150-160 caracteres).
- **Open Graph**: Sempre incluir tags Open Graph (OG) para garantir que links compartilhados em redes sociais e WhatsApp tenham imagens e descrições atraentes.

### 2. Estrutura Semântica (HTML5)
- **Hierarquia de Hn**: Garantir exatamente um único `<h1>` por página, seguindo a ordem lógica (`<h2>`, `<h3>`, etc.).
- **Elementos Semânticos**: Usar `<main>`, `<article>`, `<section>`, `<footer>` e `<nav>` corretamente.
- **Alt Text**: Todas as imagens (exceto as estritamente decorativas) devem possuir o atributo `alt` descritivo.

### 3. URLs e Indexação
- **Caminhos Canônicos**: Definir `canonical` URLs para evitar problemas de conteúdo duplicado.
- **Sitemap & Robots**: Configurar a geração automática de `sitemap.xml` e um arquivo `robots.txt` bem estruturado usando as funções nativas do Next.js.
- **JSON-LD**: Implementar dados estruturados (Schema.org) em formato JSON-LD para produtos, artigos ou organizações.

### 4. Performance & Core Web Vitals (Fator de Ranking)
- **LCP (Largest Contentful Paint)**: Priorizar o carregamento de imagens principais.
- **CLS (Cumulative Layout Shift)**: Reservar espaço para imagens e anúncios para evitar saltos de layout.
- **Mobile First**: Garantir que a versão mobile seja a prioridade absoluta de design e performance.

## Constraints
- **CRITICAL**: Nunca deixar páginas de produção sem as tags de título e descrição básicas.
- **Links**: Sempre usar o componente `<Link>` do `next/link` para garantir o pre-fetching e a navegação SPA amigável ao Googlebot.
- **Client-Side**: Evitar depender exclusivamente de renderização no cliente (Client-side rendering) para conteúdos críticos que precisam ser indexados.
