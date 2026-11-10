# Dados do Projeto

Esta pasta contém a base de dados utilizada
na análise de vendas da loja virtual.

Os arquivos serão utilizados nas etapas de
entendimento e preparação dos dados.

## Referência bibliográfica

Chen, D. (2015). Online Retail.
UCI Machine Learning Repository.
https://doi.org/10.24432/C5BW33

### 2. Entendimento dos Dados

Nesta etapa, foi realizada uma análise inicial da base de dados Online Retail, disponibilizada pelo UCI Machine Learning Repository. O arquivo contém 541.909 registros e 8 colunas com informações relacionadas às vendas de uma loja virtual.

Entre os dados disponíveis estão o número da fatura, código e descrição dos produtos, quantidade vendida, data da compra, preço unitário, identificação dos clientes e país de origem.

Durante a análise, foi possível identificar que algumas informações estão incompletas. A coluna Description apresenta 1.454 registros sem preenchimento, enquanto a coluna CustomerID possui 135.080 registros sem identificação do cliente.

Essas informações são importantes porque ajudam a compreender a qualidade da base antes de iniciar a preparação dos dados e a construção das análises. Por esse motivo, os dados ausentes serão avaliados com mais cuidado na próxima etapa do projeto.

### 3. Preparação dos Dados

Na etapa de preparação dos dados, foram realizadas verificações para identificar registros duplicados, quantidades negativas e preços inválidos.

Inicialmente, foram encontrados 5.268 registros duplicados, que foram removidos. Também foram retirados 11.763 registros com quantidade ou preço inválido, considerando a análise após a remoção das duplicatas.

Os registros com quantidade negativa foram tratados como possíveis devoluções ou cancelamentos e não foram considerados na análise de vendas positivas.

Após os procedimentos, a base passou de 541.909 para 524.878 registros.

Também foi criada uma nova coluna chamada TotalPrice, calculada pela multiplicação da quantidade vendida pelo preço unitário. Essa coluna permite analisar o faturamento dos produtos.

O faturamento total calculado para os registros mantidos foi de aproximadamente £ 10.642.110,80.

### 4. Análise Exploratória dos Dados

Após a preparação da base, foram realizadas análises para identificar os produtos com maior faturamento e os países com maior participação nas vendas.

Na análise dos produtos, o item DOTCOM POSTAGE apresentou o maior faturamento, com aproximadamente £ 206.248,77, seguido pelo REGENCY CAKESTAND 3 TIER, com £ 174.156,54.

Em relação aos países, o Reino Unido apresentou o maior faturamento, com aproximadamente £ 9.001.744,09. Esse resultado representa cerca de 84,6% do faturamento total da base analisada.

Os resultados mostram uma concentração significativa das vendas no mercado britânico. Também foi possível identificar que alguns registros representam serviços ou cobranças, como postagem, e não necessariamente produtos físicos.

Para facilitar a interpretação dos resultados, foram desenvolvidos gráficos que apresentam os produtos e países com maior faturamento.

### 5. Análise do Faturamento Mensal

Foi realizada uma análise do faturamento mensal da loja, utilizando a coluna InvoiceDate para agrupar as vendas por mês e ano.

Os resultados mostraram que novembro de 2011 foi o período de maior faturamento, alcançando aproximadamente £ 1.503.866,78. Outubro e setembro também apresentaram resultados expressivos, com faturamentos de £ 1.151.263,73 e £ 1.056.435,19, respectivamente.

Por outro lado, fevereiro de 2011 apresentou o menor faturamento entre os meses analisados, com aproximadamente £ 522.545,56.

Os resultados indicam um crescimento do faturamento nos meses que antecederam novembro de 2011, seguido de uma redução em dezembro. Esse comportamento pode estar relacionado à sazonalidade das compras, embora sejam necessárias outras análises para confirmar essa hipótese.

### 6. Análise da Quantidade de Compras por País e por Mês

Também foi realizada uma análise da quantidade de compras, considerando o número de notas fiscais registradas na base de dados.

Na análise por país, o Reino Unido apresentou a maior quantidade de compras, com 18.019 notas fiscais. Em seguida, aparecem Alemanha, com 457, e França, com 392. Esse resultado reforça a concentração das transações no mercado britânico.

Na análise mensal, novembro de 2011 apresentou a maior quantidade de compras, totalizando 2.769 notas fiscais. Outubro ficou em segundo lugar, com 2.040, enquanto dezembro apresentou a menor quantidade, com 819 compras.

Esses resultados ajudam a identificar os principais mercados da loja e os períodos de maior movimentação. As informações também podem contribuir para o planejamento de estoque e para futuras estratégias comerciais.
