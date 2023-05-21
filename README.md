# Analise exploratória de carros a venda nos EUA

<div align="left">
<img src="https://github.com/HelderSCordeiro/EDA_CARS/assets/97766575/98da3284-5032-4a74-8ee7-288cbfe2b2e3" width="700px" />
</div>

# 1. Introdução

Automóvel (do grego αὐτός ["autós"], "por si próprio", e do latim mobilis, "mobilidade", como referência a um objeto responsável pela sua própria locomoção ou de outras pessoas em consoante) ou carro (das línguas celtas, através do latim carru)[1] é um veículo motorizado com rodas usado para transporte. Os carros entraram em uso global durante o século XX e as economias desenvolvidas dependem deles. O ano de 1886 é considerado como o ano de nascimento do carro moderno, quando o inventor alemão Karl Benz patenteou seu Benz Patent-Motorwagen.

Neste estudo iremos analisar os carros a venda nos Estados Unidos da América, os dados foram obtidos da AUCTION EXPORT.com, os mesmos contem 28 marcas de veiculos a venda no pais. Ele contem o preço, marca, cor, entre outros.


# 1.1. Objetivos

O objetivo deste estudo é realizar uma Análise Exploratória dos Dados do conjunto de dados US Cars Dataset, disponível em USA_cars_datasets.csv; a fim de caracterizar os carros a leilão nos EUA. Especificiamente serão respondidas as seguintes questões de pesquisa:

- Qual marca teve mais numero de vendas?
- Qual veiculo foi mais comprado?
- Quais modelos possuem maior faturamento?
- Qual ano possuem carros em melhores condições?
- Qual marca possui maior numero de carros em condições ruins?
- Quais caracteristicas tem uma melhor probabilidade de oferecer um carro em melhores condições?



# 2. Metodologia
Nesta seção será apresentado todo o processo de preparação, organização e limpeza de dados feito no dataset que possui os seguintes dados:


| Coluna            | Descrição                                | Tipo    |
|-------------------|------------------------------------------|-------- |
| Price             | Valor do veiculo a venda                 | Integer |
| Years             | Ano de registro do veiculo               | Integer |
| Brand             | Marca do carro                           | String  |
| Model             | Modelo do veiculo                        | String  |
| Color             | Cor do veiculo                           | String  |
| State/City        | Cidade onde o carro está localizado      | String  |
| Mileage           | Milhas percorridas pelo carro            | Float   |
| Vin               | Identificação númerica do veiculo        | integer |
| Title Status      | Classificação do veiculo                 | String  |
| Lot               | Numero de identificação do lote          | Integer |
| Condition         | Tempo                                    | String  |



## OBSERVAÇÕES

Title Status: clean vehicles e salvage insurance
Lot: é um numero atribuido a uma quantidade especifica de carros produzidos
