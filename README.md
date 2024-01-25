# Análise EggNog (COGs e espécies base)
### Passo a passo da análise
```
0- fazer o upload das bases de dados "banana_emapper.annotations.xlsx" e "rosa_emapper.annotations.xlsx"

1- excluir colunas que não tem interesse

2- separar coluna das espécies base em outra a partir do delimitador "|" e excluir a coluna que não tem interesse (coluna com número)

3- trocar nome das colunas (specie e COGs)

4- remover linhas em branco e linhas com erro de ambas as colunas restantes

5- separar as linhas com mais de uma letra para uma letra em cada linha com o comando "Text.ToList([COGs])" e selecionar a opção "expandir para novas linhas" na coluna personalizada gerada

6- excluir coluna que não tem interesse (coluna que tem mais de uma letra em uma linha)

7- montagem do dashboard

	7.1- gráfico de pizza para saber a quantidade de cada tipo de COG em cada espécie, fez um filtro tirando os valores "S" e "-" pois se referem a funções não identificadas
 
	7.2- gráfico de área para analisar de quais espécies foram extraidos os dados de função das proteínas e ver se bate com a espécie analisada, fez um filtro tirando os valores "-" pois se referem a organismo não identificado ou a função não foi identificada com nenhum organismo do banco de dados
 
	7.3- cartão para exibir a quantidade numérica de cada uma das classificações de COGs das espécies e quantificar quantas proteínas são codificadas por cada espécie por isso foi considerado os valores "S" e "-"
 
	7.4- gráfico de barras para melhor ilustração da quantidade numérica do cartão e o fundo transparente para sobrepor sobre o número do cartão, fez um filtro tirando os valores "S" e "-" pois se referem a funções não identificadas
 
	7.5- relacionar dados das planilhas na aba "exibição de modelos" para quando selecionar em um gráfico ela for gerada nos outros gráficos também assim ser possível uma comparação mais ligeira entre as espécies
 
	7.6- criar imagem de fundo
 
		7.6.1- imagem criada pela inteligência artifical Leonardo.ia com o prompt "Darkness forest seen from above, all trees black"
  
		7.6.2- após baixar imagem no computador foi inserida no power point para ajustar o tamanho de acordo com o dashboard do powerBI
  
	7.7- ajustar todos os gráfico com plano de fundo transparente, coloração das legendas de forma que fique visível e mudar coloração de certos gráficos
 ```
### Resultado
#### Dashboard sem nenhuma seleção
![image](https://github.com/Tutugb/powerBI/assets/125391314/3cf9ba11-7eca-4eb5-b9bf-74e8f241ffc3)
#### Dashboard com a seleção
![image](https://github.com/Tutugb/powerBI/assets/125391314/b8853639-1365-473b-9cb7-9aeccf057cd3)

# Análise de Venda e lucro 
```
0. fazer o upload da base de dados "Online Retail.xlsx"
1. Tratamento dos dados

	2. excluir colunas que não tem interesse

	3. renomear as colunas

	4. multiplicar "quantidade vendida" e "preço" criando "vendido"

	5. dividir coluna de preço por delimitador "-" para retirara valores negativos os quais estão errados já que não existe preço negativo

	6. substituir valore "null" por 0

7. Montagem do dashboard

	8. Primeiro gráfico de barras com linha onde o eixo x em comum é a data apenas com mês e ano, mas os valores de y para as barras é a quantidade vendida e os valores da linha é o valor acumulado (coluna "vendido")

	9. Segundo gráfico de barras de barras com linha onde o eixo x em comum é a data apenas com mês e ano, mas os valores de y para as barras é a quantidade vendida e os valores da linha é o preço dos produtos

	10. Primeiro gráfico de pizza com as cidades que fizeram vendas assim analisando qual vendeu mais

	11. Segundo gráfico dos produtos vendidos analisando qual produto foi mais vendido

	12. Primeiro cartão com o valor da soma do valor acumulado com as vendas (coluna "vendido")

	13. Segundo cartão com o valor da soma da quantidade vendida dos produtos em geral

 	14. Primeiro filtro, seleciona o ano que quer analisar

 	15. Segundo filtro, seleciona o mês que quer analisar

 	16. Terceiro filtro, seleciona a cidade que quer analisar

 	17. Quarto filtro, seleciona o produto que quer analisar

	18. Realizado do plano de fundo no powerpoint
```
### Resultado 
#### Dashboard sem nenhuma seleção
![image](https://github.com/Tutugb/powerBI/assets/125391314/a7db8521-6786-4ddb-a5f8-ff83929c6e44)
#### Dashboard com a seleção
![image](https://github.com/Tutugb/powerBI/assets/125391314/350056c7-024c-4f04-9be3-d15a31e7bedd)
