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
- Qual ano possuem carrso em melhores condições?
- Qual marca possui maior numero de carros em condições ruins?



# 2. Metodologia
Nesta seção será apresentado todo o processo de preparação, organização e limpeza de dados feito no dataset que possui os seguintes dados:


| Coluna            | Descrição                                                                 | Tipo    |
|-------------------|---------------------------------------------------------------------------|-------- |
| Price             | Valor do veiculo a venda                                                  | Integer |
| Years             | Ano de registro do veiculo                                                            |         |
| Brand             | Marca do carro                                           |         |
| Model             | Modelo do veiculo                                                       |         |
| Color             | Cor do veiculo                                            |         |
| State/City        | Idade do passageiro.                                                      |         |
| Mileage           | Número de irmãos e cônjuges a bordo.                                      |         |
| Vin               | Número de pais e filhos a bordo.                                          |         |
| Title Status      | Número do bilhete                                                         |         |
| Lot               | Preço da tarifa do passageiro.                                            |         |
| Condition         | Cabine.                                                                   |         |


Feature	Type	Description
Price	Integer	The sale price of the vehicle in the ad
Years	Integer	The vehicle registration year
Brand	String	The brand of car
Model	String	model of the vehicle
Color	String	Color of the vehicle
State/City	String	The location in which the car is being available for purchase
Mileage	Float	miles traveled by vehicle
Vin	String	The vehicle identification number is a collection of 17 characters (digits and capital letters)
Title Status	String	This feature included binary classification, which are clean title vehicles and salvage insurance
Lot	Integer	A lot number is an identification number assigned to a particular quantity or lot of material from a single manufacturer.For cars, a lot number is combined with a serial number to form the Vehicle Identification Number.
Condition	String	Time


## OBSERVAÇÕES
classe é uma aproximação do status socioeconômico na época, onde: 1 = Classe Alta1; 2 = Classe Média e 3 = Classe Baixa;
idade está representada em anos, porém, se a idade for menor que Um (1) ou caso tenha sido estimada, ela estará com casas decimais xx.5;
tarifa está em Libras esterlinas (British Pounds - £) anteriores a 1970;
irmaos_conjuges e pais_filhos: as variáveis de relação familiar de algumas relações foram ignoradas; a seguir estão as definições usadas:
Irmão: Irmão, irmã, meio-irmão ou meia-irmã do passageiro a bordo do Titanic;
Cônjuge: Marido ou esposa do passageiro a bordo do Titanic (amantes e noivos ignorados);
Pai: Mãe ou pai do passageiro a bordo do Titanic;
Criança: Filho, Filha, Enteado ou Enteada do Passageiro a bordo do Titanic;
Outros parentes excluídos deste estudo incluem primos, sobrinhos / sobrinhas, tias / tios e parentes;
Algumas crianças viajavam apenas com uma babá, portanto foi atribuído 0 para elas em pais_filhos;
Alguns viajaram com amigos ou vizinhos muito próximos em uma vila, no entanto, as definições não apóiam essas relações.
