# 📊 Formação Power BI Analyst - Desafio de Projeto DIO

Este repositório contém o desenvolvimento do **Sales Report (Relatório de Vendas)**, um painel interativo construído no Power BI Desktop como parte dos desafios práticos da plataforma Digital Innovation One (DIO).

O objetivo principal foi transformar dados brutos de vendas (`financials`) em insights visuais claros que facilitem a tomada de decisões estratégicas de negócios.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

*   **Power BI Desktop**: Construção dos gráficos, modelagem e layout.
*   **DAX (Data Analysis Expressions)**: Criação de medidas e colunas calculadas para análise de indicadores.
*   **Power Query**: Limpeza, tratamento e transformação dos dados estruturados.

---

## 📈 Indicadores Chave (KPIs) Analisados

O dashboard apresenta as principais métricas de desempenho em cartões de destaque no topo da página:

*   **Total de Vendas**: Soma do faturamento bruto gerado (`118,73 Mi`).
*   **Unidades Vendidas**: Volume total de produtos comercializados (`1,13 Mi`).
*   **Soma de Descontos**: Total de reduções aplicadas nas vendas (`9,21 Mi`).
*   **Soma de Gross Sales**: Faturamento total antes das deduções (`127,93 Mi`).
*   **Soma de COGS**: Custo total das mercadorias vendidas (`101,83 Mi`).

---

## 🗺️ Estrutura das Visualizações

O relatório foi desenhado utilizando um layout limpo, moderno e segmentado para responder às seguintes perguntas de negócio:

1.  **Filtro Temporal**: Um segmentador de dados por período para analisar intervalos específicos de datas.
2.  **Evolução das Vendas**: Um gráfico de área que demonstra a flutuação e tendências do faturamento ao longo dos meses.
3.  **Vendas por Segmento**: Gráfico de barras horizontais detalhando a performance por canais de mercado.
4.  **Vendas por Produto**: Gráfico de barras horizontais elencando os produtos mais vendidos.
5.  **Distribuição Geográfica**: Um mapa interativo que exibe o volume de vendas mapeado por países/regiões.

---

## 🗄️ Modelo de Dados

O painel utiliza como base a tabela nativa **`financials`**, contendo os seguintes campos principais em sua hierarquia:
*   `Sales` (Vendas)
*   `COGS` (Custo das mercadorias)
*   `Discounts` (Descontos)
*   `Product` (Produtos)
*   `Segment` (Segmentos de mercado)
*   `Date` (Dimensão de tempo estruturada em Ano, Trimestre, Mês e Dia)



💡 *Projeto desenvolvido por Pedro de Souza durante a Formação Power BI Analyst da DIO.*
