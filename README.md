# Projeto CRISP-DM – Análise de Vendas de uma Loja Virtual

## 1. Apresentação do Projeto

Este projeto tem como objetivo realizar uma análise de dados de vendas de uma loja virtual, utilizando a metodologia CRISP-DM (Cross Industry Standard Process for Data Mining).

A análise foi desenvolvida com Python e a biblioteca Pandas, buscando identificar informações importantes sobre os produtos vendidos, os países com maior quantidade de compras, o faturamento mensal e o comportamento dos clientes.

## 2. Base de Dados

Foi utilizada a base de dados Online Retail, disponibilizada pelo UCI Machine Learning Repository.

A base contém informações sobre transações comerciais realizadas entre dezembro de 2010 e dezembro de 2011.

**Fonte:** Chen, D. (2015). Online Retail. UCI Machine Learning Repository.

https://doi.org/10.24432/C5BW33

## 3. Metodologia CRISP-DM

O projeto foi desenvolvido seguindo as principais etapas da metodologia CRISP-DM:

### 3.1 Entendimento do Negócio
Definição do objetivo de analisar as vendas da loja virtual, buscando identificar padrões e informações que possam auxiliar nas decisões comerciais.

### 3.2 Entendimento dos Dados
Análise inicial da base, que originalmente possuía 541.909 registros e 8 colunas. Foram identificadas informações sobre produtos, clientes, datas, quantidades, preços e países.

### 3.3 Preparação dos Dados
Foram removidos 5.268 registros duplicados e 11.763 registros com quantidade ou preço inválido, considerando a análise após a remoção das duplicatas.

Também foram criadas as colunas TotalPrice e AnoMes para facilitar as análises.

Ao final, a base ficou com 524.878 registros e 10 colunas.

### 3.4 Análise Exploratória
Foram realizadas análises para identificar:
- Produtos com maior faturamento;
- Países com maior faturamento;
- Quantidade de compras por país;
- Faturamento mensal;
- Quantidade de compras por mês;
- Clientes com maiores valores acumulados em compras.

### 3.5 Avaliação
Os resultados foram analisados para identificar padrões de vendas e possíveis limitações da base.

Foi identificado que 25,18% dos registros não possuem identificação de cliente (CustomerID).

## 4. Principais Resultados

- **Faturamento analisado:** aproximadamente £ 10.642.110,80.
- **País com maior faturamento:** Reino Unido, com aproximadamente £ 9 milhões.
- **Maior faturamento mensal:** novembro de 2011, com £ 1.503.866,78.
- **Maior quantidade de compras em um mês:** novembro de 2011, com 2.769 notas fiscais.
- **Cliente com maior valor acumulado:** cliente 14646, com aproximadamente £ 280.206,02.
- **Quantidade de clientes identificados:** 4.338.

## 5. Ferramentas Utilizadas

- Python;
- Google Colab;
- Pandas;
- Matplotlib;
- GitHub.

## 6. Estrutura do Repositório

- `dados/`: base de dados utilizada no projeto.
- `documentos/`: documentação complementar.
- `notebooks/`: notebook com os códigos e análises realizadas.
- `resultados/`: gráficos gerados durante o projeto.

## 7. Conclusão

O desenvolvimento deste projeto permitiu compreender melhor como a análise de dados pode ser utilizada para estudar o desempenho de uma loja virtual.

Por meio das análises realizadas, foi possível identificar os principais produtos, países, períodos e clientes relacionados às vendas.

Também foi possível perceber a importância da preparação dos dados antes de iniciar uma análise, pois registros duplicados, valores inválidos e informações ausentes podem influenciar os resultados.

De modo geral, o trabalho proporcionou uma experiência prática com Python, Pandas, visualização de dados e aplicação da metodologia CRISP-DM.

## 8. Referência Bibliográfica

CHEN, D. **Online Retail**. UCI Machine Learning Repository, 2015. Disponível em: https://doi.org/10.24432/C5BW33. Acesso em: 9 nov. 2026.
