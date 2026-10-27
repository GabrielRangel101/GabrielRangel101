# Gabriel Rangel

**Analista de Dados | Automação & IA | Power BI · SQL · Python · n8n · Supabase**

Rio de Janeiro, RJ · Business Analytics B2C no Grupo RBS · Analista autônomo de dados e automação

---

## Sobre

Transformo dados brutos em decisão e tiro trabalho manual da operação. No dia a dia, analiso funil de assinaturas, retenção e aquisição paga em produtos digitais B2C. Fora dele, construo dashboards, sistemas web e automações para pequenas e médias empresas.

Hoje meu foco é unir análise de dados com automação: fluxos em **n8n**, back-end em **Supabase** e integrações com a **API do Claude**.

## Stack

| Área | Ferramentas |
|---|---|
| Análise e BI | Power BI (DAX, modelagem, RLS), Looker, Excel |
| Dados | SQL, Python (pandas), ETL |
| Automação e IA | n8n, Power Automate, Claude API |
| Back-end e web | Supabase (PostgreSQL), TypeScript, React, TanStack Start |

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-336791?style=flat&logo=postgresql&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat&logo=n8n&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat&logo=supabase&logoColor=white)

---

## Cases

Os três projetos abaixo usam **dados 100% sintéticos** (nenhuma empresa ou cliente real), gerados em Python com seed fixa. Em todos, o motor de métricas é determinístico e testado, e o "Modo IA" só escolhe a análise e redige: **a IA nunca calcula número**.

### 1. Gazeta Meridiano · Assinaturas B2C

[Painel ao vivo](https://gazetameridiano.app/?view=geral) · [Código](https://github.com/GabrielRangel101/meridiano-subscriber-compass)

- **Problema:** um jornal digital não sabe por que perde assinantes nem quanto vale agir em cada alavanca (churn, falha de pagamento, aquisição).
- **O que construí:** base sintética de ~11 mil assinantes em 24 meses, com histórias plantadas (queda de retenção após a Black Friday, retenção pior em mídia paga, efeito de reajuste de preço). Retenção por Kaplan-Meier, funil de compra visitante → compra com vazamento por canal, ponte de MRR (novos, fim de promoção, reajuste, upgrades, churn), CAC/LTV/payback por canal e um simulador "e se" com três alavancas.
- **Decisão técnica:** correlações calculadas sobre variações mês a mês, para não tratar tendência comum como relação causal. A "Mesa de análise" responde perguntas em português chamando o motor de métricas.
- **Stack:** TanStack Start, Tailwind v4, shadcn, Lovable + GitHub.

### 2. Fluxo Media Compass · Mídia paga e tracking de app

[Painel ao vivo](https://fluxo-subscriber-compass.lovable.app/?view=geral) · [Código](https://github.com/GabrielRangel101/fluxo-media-compass)

- **Problema:** uma fintech fictícia (conta digital + cartão) decide verba de mídia com números que as fontes (plataforma, AppsFlyer, backend) nem sempre confirmam.
- **O que construí:** CPI, CPA, CAC, ROAS D30/D90 e LTV90 por canal, funil do app (clique → instalação → cadastro → KYC → primeiro uso do cartão), testes A/B com checagem de SRM e amostra mínima, simulador de realocação de verba e um tagbook de eventos com dono e saúde.
- **O diferencial:** cinco defeitos de tracking plantados de propósito (perda de atribuição iOS no Meta, cadastro contado em dobro no Google Ads, `form_submit` duplicado no GA4, `kyc_done` sumindo no SDK Android, UTM perdida no LinkedIn). O painel de saúde da coleta encontra todos, com a data de início recuperada dos dados.
- **Rigor:** pacote com 9 consultas SQL e teste automático que exige resultado idêntico ao do motor em TypeScript (20 testes). Coortes imaturas não mostram ROAS, em vez de um número enganoso.
- **Stack:** TypeScript, SQL (SQLite), React, TanStack Start, Lovable + GitHub.

### 3. Mercado Aurora · Margem e ruptura no varejo

[Painel ao vivo](https://aurora-subscriber-atlas.lovable.app/) · [Código](https://github.com/GabrielRangel101/mercado-aurora)

- **Problema:** uma rede fictícia de 4 supermercados perde margem em ruptura de gôndola e em perdas (vencimento, avaria, quebra), sem saber onde nem quanto.
- **O que construí:** simulação de 280 SKUs em 12 categorias, 4 lojas e 365 dias, com estoque de verdade (demanda → venda limitada ao estoque → quebra → pedido com ponto de reposição e lead time). Ruptura e perda **nascem da simulação**, não são sorteadas depois. Sete telas: visão geral com ponte da margem, margem e curva ABC, ruptura, perdas, lojas e caixas, cesta de compras e alertas.
- **Decisões técnicas:** todo texto do painel é calculado dos dados (nenhum número digitado). Fornecedor irregular em itens de alto giro e uma loja que compra demais ficam como padrões plantados, com gabarito documentado.
- **Limites assumidos (no README do projeto):** a taxa de ruptura (~3%) vem da política de reposição simulada e tende a ser maior em operação real; venda perdida assume que 25% dos clientes levam outro item; a aba de alertas é especificação, a automação ainda não está conectada.
- **Stack:** Python (gerador), TypeScript, React, Recharts, Lovable + GitHub.

---

## Em construção

- Sistema de comanda digital com dashboard para restaurante, com back-end em Supabase.
- Automações com n8n + Claude para atendimento e rotinas operacionais.
- Portfólio online com os cases completos de dados, BI, automação e web.

## Trajetória

- **2025 – hoje** · Assistente de Dados, Grupo RBS (Business Analytics): Redação, Audiência, Streaming e produtos digitais B2C.
- **2023 – hoje** · Analista de dados e automação autônomo, com clientes do varejo.
- **Formação** · Análise e Desenvolvimento de Sistemas, IBMR (conclusão prevista em 12/2026).

## Contato

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gabriel-r-lima-a954ba26a/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/gabrielrangel.analytics/)
