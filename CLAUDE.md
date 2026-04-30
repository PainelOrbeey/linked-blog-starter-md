# ORBEEY BRAIN — Contexto do Projeto

## O que é este projeto
Este repositório é o **Orbeey Brain**: um segundo cérebro organizacional da Orbeey, construído em Obsidian e publicado via `linked-blog-starter` (Next.js + Vercel). Cada pasta representa uma região do cérebro com função específica.

## Estrutura do Cérebro (`publish/`)

```
publish/
├── HOME.md                          ← Página central (entry point)
├── 00_IDENTIDADE_ORBEEY/            ← DNA da empresa
│   ├── Visao_Missao_Valores.md
│   ├── Cultura_Orbeey.md
│   ├── Posicionamento.md
│   ├── Proposta_de_Valor.md
│   └── Regras_Gerais.md
├── 01_CORTEX_PRE_FRONTAL/           ← Estratégia e decisões
│   ├── Decisoes.md
│   ├── Estrategias.md
│   ├── Planejamento.md
│   ├── Oportunidades.md
│   └── Riscos.md
├── 02_HIPOCAMPO_MEMORIA/            ← Memória e histórico
│   ├── Clientes/
│   │   └── TEMPLATE_Cliente.md     ← Copiar para cada cliente novo
│   ├── Aprendizados.md
│   ├── Historico_Tarefas.md
│   ├── Reunioes.md
│   └── Relatorios.md
├── 03_CORTEX_TEMPORAL_COMUNICACAO/  ← Comunicação e scripts
│   ├── Tom_de_Voz.md
│   ├── Scripts_Clientes.md
│   ├── Scripts_Equipe.md
│   ├── Respostas_Padrao.md
│   └── Relatorios_Automaticos.md
├── 04_CORTEX_PARIETAL_DADOS/        ← Dados e métricas
│   ├── KPIs.md
│   ├── Metricas.md
│   ├── Dashboards.md
│   ├── Analises.md
│   └── Diagnosticos.md
├── 05_CORTEX_MOTOR_EXECUCAO/        ← Execução e automações
│   ├── Tarefas.md
│   ├── Checklists.md
│   ├── Automacoes.md
│   ├── Fluxos.md
│   └── Comandos.md
├── 06_SISTEMA_LIMBICO_RELACIONAMENTO/ ← CS e satisfação
│   ├── Churn.md
│   ├── Satisfacao_Cliente.md
│   ├── Feedbacks.md
│   └── CS_Processos.md
├── 07_CEREBELO_ROTINAS/             ← Rotinas e processos
│   ├── Rotina_Agencia.md
│   ├── Rotina_Clientes.md
│   ├── Rotina_Financeiro.md
│   └── Rotina_Relatorios.md
├── 08_CORPO_CALOSO_INTEGRACOES/     ← Integração dos polos
│   ├── Agency.md
│   ├── Technology.md
│   ├── Influencers.md
│   ├── Law.md
│   ├── Contability.md
│   └── Trip.md
├── 09_FINANCEIRO/                   ← Finanças
│   ├── Receita.md
│   ├── Custos.md
│   ├── Margens.md
│   ├── Projecoes.md
│   └── Split.md
├── 10_COMERCIAL/                    ← Vendas e funil
│   ├── Funil.md
│   ├── Leads.md
│   ├── Scripts_Vendas.md
│   ├── Objecoes.md
│   └── Fechamentos.md
├── 11_MARKETING/                    ← Marketing e performance
│   ├── Campanhas.md
│   ├── Performance.md
│   ├── Copies.md
│   ├── Criativos.md
│   └── Influenciadores.md
├── 12_PROTOCOLOS/                   ← Regras e protocolos da IA
│   ├── Protocolo_Memoria.md
│   ├── Protocolo_Anti_Alucinacao.md
│   ├── Protocolo_Atendimento.md
│   ├── Protocolo_Decisao.md
│   ├── Protocolo_Emergencia.md
│   ├── Protocolo_Relatorio.md
│   ├── Protocolo_Privacidade.md
│   ├── Protocolo_Treinamento.md
│   └── Protocolo_Cobranca_Equipe.md
└── 13_META/                         ← Arquitetura e evolução da IA
    ├── Arquitetura_IA.md
    ├── Roadmap_IA.md
    └── Evolucao_Orbeey.md
```

## Padrão dos Arquivos
Todo arquivo `.md` usa frontmatter YAML:
```yaml
---
title: "Título legível"
excerpt: "Descrição curta do conteúdo."
tags:
  - orbeey-brain
---
```

Links internos usam formato Obsidian: `[[pasta/arquivo|Texto do link]]`

## Como adicionar novos clientes
1. Copie `02_HIPOCAMPO_MEMORIA/Clientes/TEMPLATE_Cliente.md`
2. Renomeie para o nome do cliente: `02_HIPOCAMPO_MEMORIA/Clientes/NOME_CLIENTE.md`
3. Preencha todos os campos
4. Adicione frontmatter com `title` e `excerpt`
5. Commite e faça push

## Pipeline de publicação
- Branch `main` → GitHub Actions → `obsidian-export` → Vercel (linked-blog-starter)
- O `obsidian-export` converte wiki-links `[[...]]` para markdown padrão
- PUBLISH_DIR: `publish/`

## Princípio de funcionamento
**Entrada de dado → Registro no módulo correto → Linkagem → Ação → Aprendizado**

## Protocolos obrigatórios ao interagir
1. **Nunca inventar dados** → ver `12_PROTOCOLOS/Protocolo_Anti_Alucinacao.md`
2. **Sempre registrar decisões** → ver `01_CORTEX_PRE_FRONTAL/Decisoes.md`
3. **Clientes têm ficha** → ver `02_HIPOCAMPO_MEMORIA/Clientes/`
4. **Relatórios seguem padrão** → ver `12_PROTOCOLOS/Protocolo_Relatorio.md`
