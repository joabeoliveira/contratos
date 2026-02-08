---
name: Public Administration Rules
description: Diretrizes para projetos que envolvem Administração Pública, leis, jurisprudências e conformidade governamental.
---

# Skill: Especialista em Gov-Tech e Direito Administrativo

## Goal
Garantir que as soluções tecnológicas estejam em total conformidade com a legislação brasileira, normas da AGU/CGU e boas práticas de administração pública, fundamentando cada decisão técnica em bases legais.

## Instructions

### 1. Fontes de Consulta Obrigatórias
Sempre que o projeto envolver o setor público, os seguintes pilares devem ser consultados:
- **Legislação**: Lei de Licitações (14.133/21), Lei de Acesso à Informação (LAI), LGPD e Marco Civil da Internet.
- **Órgãos de Controle**: Recomendações e manuais da **CGU** (Controladoria-Geral da União) e **AGU** (Advocacia-Geral da União).
- **Padronização**: Consultar o [Instrumento de Padronização dos Procedimentos de Contratação da AGU (Fev/2024)](https://www.gov.br/agu/pt-br/composicao/cgu/cgu/guias/instrumento-de-padronizacao-dos-procedimento-de-contratacao-agu-fev-2024.pdf).
- **Jurisprudência**: Entendimentos do **TCU** (Tribunal de Contas da União) relevantes para a regra de negócio.
- **Ecossistema Gov**: APIs do Governo (Gov.br, Compras.gov.br), Manuais de Redação da Presidência e diretrizes de escolas governamentais (ENAP, etc.).

### 2. Documentação e Rastreabilidade no Código
- **Comentários de Origem**: Toda lógica de negócio baseada em lei ou norma deve conter um comentário explicando o "porquê" daquela implementação.
- **Referenciamento**: Citar explicitamente o artigo da lei, o número do acórdão do TCU ou o manual da AGU que originou a regra.
- **Exemplo de Comentário**: 
  `// Regra: Impedimento de licitar conforme Art. 156 da Lei 14.133/2021`
  `// Origem: Manual de Sanções Administrativas da CGU, pág 45.`

### 3. Ética e Segurança
- **Transparência Passiva/Ativa**: Garantir que a lógica de exibição de dados siga os princípios da LAI.
- **Auditabilidade**: Implementar logs de trilha de auditoria para ações críticas que envolvam recursos ou decisões públicas.

## Constraints
- **CRITICAL**: Nunca implementar uma regra de "atalho" que viole princípios do Direito Administrativo (Legalidade, Impessoalidade, Moralidade, Publicidade e Eficiência).
- **Dados Sensíveis**: Tratamento rigoroso de dados conforme a LGPD, especialmente em integrações com bases governamentais.
