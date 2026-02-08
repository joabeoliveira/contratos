---
name: Accessibility e-MAG
description: Padrões de acessibilidade para Governo Eletrônico (e-MAG) e diretrizes WCAG.
---

# Skill: Especialista em Acessibilidade Digital (e-MAG/WCAG)

## Goal
Garantir que todas as interfaces do sistema sejam plenamente acessíveis para todos os cidadãos, respeitando as normas legais e técnicas de acessibilidade.

## Instructions

### 1. Padrões Governamentais (e-MAG)
- **Navegação por Teclado**: Garanta que todos os elementos interativos sejam acessíveis via `Tab` e possuam indicadores visuais claros de `focus`.
- **Acessibilidade de Conteúdo**: Fornecer alternativas para conteúdo não textual (imagens, áudios, vídeos).
- **Contraste**: Seguir o padrão WCAG AA para contraste mínimo entre texto e fundo (cores do Shadcn devem ser validadas).

### 2. Semântica para Leitores de Tela (ARIA)
- **Aria Labels**: Usar `aria-label` em botões iconográficos ou elementos sem texto visível.
- **Hierarquia de Cabeçalhos**: Nunca pular níveis de cabeçalho (`h1` -> `h2` -> `h3`) para que a navegação estrutural funcione corretamente.
- **Formulários**: Sempre associar `<label>` aos seus respectivos `<input>` e usar `aria-required` onde necessário.

### 3. Facilidade de Uso
- **Skip Links**: Incluir um "Ir para o conteúdo principal" no topo da página.
- **Mensagens de Erro**: Garantir que as validações de formulário sejam anunciadas por leitores de tela e visualmente intuitivas.

## Constraints
- **CRITICAL**: Nunca desativar o contorno de foco (`outline: none`) sem fornecer uma alternativa visual superior.
- **Imagens**: O uso de `alt=""` é obrigatório para imagens decorativas, mas imagens informativas devem ter descrições úteis.
- **Tamanho**: Manter uma escala de fonte legível (mínimo 16px para texto corrido).
