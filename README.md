# Case - Data Preparation de um dataset para utilizá-lo na classificação de churn dos clientes

## Introdução

Uma empresa fictícia de telecomunicações dos Estados Unidos tem uma base de dados contendo diversas informações a respeito de seus clientes, desde a localização deles até com qual frequência utilizam a internet para assistir filmes. A partir disto, a empresa deseja que, após ser feita toda a limpeza e organização dados disponíveis, seja possível criar uma métrica de classificação chamada "churn", que indica o quanto a empresa perdeu de clientes. Ou seja, clientes classificados como churn são considerados "ex-clientes", não compram ou assinam mais os produtos da compania em questão.

## Objetivo do projeto

Projeto de data cleaning e data wrangling, com o objetivo de preparar uma base de dados que será utilizada para classificação de churn pela empresa.

## Sobre o dataset

O dataset é uma base pública disponibilizada pela IBM, com 7043 linhas e 33 colunas. Segue abaixo a descrição de cada uma das colunas.

* CustomerID: um ID exclusivo que identifica cada cliente.
* Count: um valor usado em relatórios/painel para somar o número de clientes em um conjunto filtrado.
* Country: O país de residência principal do cliente.
* State: O estado da residência principal do cliente.
* City: A cidade da residência principal do cliente.
* Zip Code: O CEP da residência principal do cliente.
* Lat Long: A latitude e longitude combinadas da residência principal do cliente.
* Latitude: A latitude da residência principal do cliente.
* Longitude: A longitude da residência principal do cliente.
* Gender: O gênero do cliente: Masculino, Feminino
* Senior: Indica se o cliente tem 65 anos ou mais: Sim, Não
* Partner: Indique se o cliente possui parceiro: Sim, Não
* Dependents: Indica se o cliente mora com algum dependente: Sim, Não. Os dependentes podem ser filhos, pais, avós, etc.
* Tenure Months: Indica o total de meses que o cliente esteve na empresa até o final do trimestre especificado.
* Phone Service: Indica se o cliente contrata o serviço telefônico residencial da empresa: Sim, Não
* Multiple Lines: Indica se o cliente assina múltiplas linhas telefônicas com a empresa: Sim, Não
* Internet Service: Indica se o cliente assina o serviço de Internet da empresa: Não, DSL, Fibra Óptica, Cabo.
* Online Security: Indica se o cliente assina algum serviço adicional de segurança online fornecido pela empresa: Sim, Não
* Online Backup: Indica se o cliente assina algum serviço adicional de backup online fornecido pela empresa: Sim, Não
* Device Protection: Indica se o cliente assina um plano adicional de proteção de dispositivos para seus equipamentos de Internet fornecido pela empresa: Sim, Não
* Tech Support: Indica se o cliente assina algum plano adicional de suporte técnico da empresa com tempos de espera reduzidos: Sim, Não
* Streaming TV: Indica se o cliente utiliza seu serviço de Internet para transmitir programação de televisão de um provedor terceirizado: Sim, Não. A empresa não cobra taxa adicional por este serviço.
* Streaming Movies: Indica se o cliente utiliza seu serviço de Internet para transmitir filmes de um provedor terceirizado: Sim, Não. A empresa não cobra taxa adicional por este serviço.
* Contract: Indica o tipo de contrato atual do cliente: Mês a Mês, Um Ano, Dois Anos.
* Paperless Billing: Indica se o cliente optou pelo faturamento sem papel: Sim, Não
* Payment Method: Indica como o cliente paga sua fatura: Saque Bancário, Cartão de Crédito, Cheque Enviado
* Monthly Charge: Indica a cobrança mensal total atual do cliente por todos os serviços da empresa.
* Total Charges: Indica os encargos totais do cliente, calculados até o final do trimestre especificado acima.
* Churn Label: Sim = o cliente saiu da empresa neste trimestre. Não = o cliente permaneceu na empresa. Diretamente relacionado ao valor de churn.
* Churn Value: 1 = o cliente saiu da empresa neste trimestre. 0 = o cliente permaneceu na empresa. Diretamente relacionado ao rótulo Churn.
* Churn Score: um valor de 0 a 100 que é calculado usando a ferramenta preditiva IBM SPSS Modeler. O modelo incorpora vários fatores conhecidos por causar rotatividade. Quanto maior a pontuação, maior a probabilidade de o cliente se desligar.
* CLTV: Valor de vida do cliente. Um CLTV previsto é calculado usando fórmulas corporativas e dados existentes. Quanto maior o valor, mais valioso é o cliente. Clientes de alto valor devem ser monitorados quanto à rotatividade.
* Churn Reason: o motivo específico de um cliente para deixar a empresa. Diretamente relacionado à categoria Churn.