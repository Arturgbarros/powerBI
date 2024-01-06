# Análise EggNog (COGs e espécies base)
### Passo a passo da análise
0- fazer o upload das bases de dados "banana_emapper.annotations" e "rosa_emapper.annotations"

1- excluir colunas que não tem interesse

2- separar coluna das espécies base em outra a partir do delimitador "|" e excluir a coluna que não tem interesse (coluna com número)

3- trocar nome das colunas (specie e COGs)

4- remover linhas em branco e linhas com erro de ambas as colunas restantes

5- separar as linhas com mais de uma letra para uma letra em cada linha com o comando "Text.ToList([COGs])" e selecionar a opção "expandir para novas linhas" na coluna personalizada gerada

6- excluir coluna que não tem interesse (coluna que tem mais de uma letra em uma linha)

7- montar o dashboard

	7.1- gráfico de pizza para saber a quantidade de cada tipo de COG em cada espécie, fez um filtro tirando os valores "S" e "-" pois se referem a funções não identificadas
 
	7.2- gráfico de área para analisar de quais espécies foram extraidos os dados de função das proteínas e ver se bate com a espécie analisada
 
	7.3- cartão para exibir a quantidade numérica de cada uma das classificações de COGs das espécies
 
	7.4- gráfico de barras para melhor ilustração da quantidade numérica do cartão e o fundo transparente para sobrepor sobre o número do cartão
 
	7.5- relacionar dados das planilhas na aba "exibição de modelos" para quando selecionar em um gráfico ela for gerada nos outros gráficos também assim ser possível uma comparação mais ligeira entre as espécies
 
	7.6- criar imagem de fundo
 
		7.6.1- imagem criada pela inteligência artifical Leonardo.ia com o prompt "Darkness forest seen from above, all trees black"
  
		7.6.2- após baixar imagem no computador foi inserida no power point para ajustar o tamanho de acordo com o dashboard do powerBI
  
	7.7- ajustar todos os gráfico com plano de fundo transparente, coloração das legendas de forma que fique visível e mudar coloração de certos gráficos
 
### Resultado
#### Dashboard sem nenhuma seleção
![image](https://github.com/Tutugb/powerBI/assets/125391314/e3896a3f-376f-454a-a1cc-793babbc3a60)
#### Dashboard com a seleção
![image](https://github.com/Tutugb/powerBI/assets/125391314/715f9acf-0c5e-4218-adc4-35bd83f25a3b)
