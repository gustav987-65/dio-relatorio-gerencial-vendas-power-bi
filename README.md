# Relatório Gerencial de Vendas com Power BI

Projeto prático do desafio **Formação Power BI Analyst (DIO)**: um relatório gerencial de vendas e lucro, com duas páginas, a partir de uma base financeira de 2013 e 2014.

## Objetivo

Transformar uma base de vendas em um painel que responda perguntas de gestão:

- Quanto vendemos e lucramos?
- Quais segmentos, produtos e países mais contribuem?
- Como as vendas e o lucro evoluem ao longo do tempo?

## Base de dados

Tabela `financials`, com as colunas: Segment, Country, Product, Discount Band, Units Sold, Manufacturing Price, Sale Price, Gross Sales, Discounts, Sales, COGS, Profit, Date, Month Number e Month Name.

## Página 1: Vendas

- **Cartões:** Vendas Líquidas, Unidades Vendidas, Descontos Concedidos, Lucro e Custo dos Produtos
- **Evolução das Vendas por Mês e Ano** (gráfico de área, com 2013 e 2014 separados)
- **Vendas por Segmento** (barras e rosca, com botões para alternar)
- **Vendas por Produto** (barras)
- **Vendas por País** (treemap e mapa, com botões para alternar)
- **Filtro de datas** e botão para limpar segmentações

## Página 2: Lucro (Raio-X do Lucro)

- **Árvore de decomposição:** lucro total, por ano e por país
- **Segmentos Mais Lucrativos** (barras, com o prejuízo do Enterprise em destaque)
- **Lucro por Produto** (colunas)
- **Lucro por Trimestre** (cascata)
- **Filtro de ano** (2013 e 2014)
- Botão para voltar à página de vendas

## Principais passos técnicos

1. Importação da base no Power BI Desktop e tratamento no Power Query (tipos de dados e nomes de colunas).
2. Ordenação do nome do mês pelo número do mês (`Month Name` classificado por `Month Number`).
3. Criação das visualizações e do layout (cabeçalho, barra lateral, cartões e gráficos).
4. Botões e marcadores para alternar entre visuais (barras/rosca e blocos/mapa).
5. Segmentação por ano e botão de navegação entre as páginas.
6. Identidade visual própria: azul na página de vendas e verde na página de lucro.

## Insights

- O lucro de **2014 (13,0 Mi)** foi mais de três vezes o de 2013 (3,9 Mi). Vale lembrar que a base de 2013 começa em setembro, então não é um ano completo.
- Em 2014, o segmento **Government** concentra a maior parte do lucro (cerca de 8,5 Mi).
- O segmento **Enterprise** teve **prejuízo** em 2014 (cerca de -420 mil).
- **Paseo** é o produto mais lucrativo em 2014.
- O lucro cresce a cada trimestre de 2014, com o 4º trimestre sendo o maior.
- **França** lidera o lucro por país em 2014.

## Tecnologias

- Power BI Desktop
- Power Query
- DAX (medidas básicas)

## Como abrir o projeto

1. Baixe o arquivo `.pbix` deste repositório.
2. Abra no **Power BI Desktop** (gratuito).
3. Navegue entre as páginas **Vendas** e **Lucro**. No Desktop, use **Ctrl + clique** nos botões.

## Autor

**Gustavo Lima de Sena**

[LinkedIn](https://www.linkedin.com/in/gustavo-lima-3020a3397/) | [GitHub](https://github.com/gustav987-65)

---

Projeto desenvolvido como parte do desafio de projeto da [DIO](https://www.dio.me).
