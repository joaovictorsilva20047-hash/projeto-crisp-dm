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
