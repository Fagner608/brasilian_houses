# Análise exploratória e machine learning de dados sobre casas alugadas [kaggle](https://www.kaggle.com/datasets/rubenssjr/brasilian-houses-to-rent)
Projeto autônomo, visando demonstrar conhecimento teórico e prático nos tópicos descritos abaixo.



- Pré-processamento, análise, visualização, geração de insights, machine learning. O projeto visa aplicar os dados à um modelo de regressão linear, para responder às questões de negócio levantadas, e, criar um modelo preditivo.

  
Objetivo: em um primeiro momento, conhecer os dados, e, concluir se estão em ordem para aplicação em um modelo preditivo. Em um segundo momento, será criado o modelo, e realizado o deploy em uma webapp.


Fonte dos dados: 


1 - Dados foram obtidos no [kaggle](https://www.kaggle.com/datasets/rubenssjr/brasilian-houses-to-rent).

## Tecnologias Utilizadas


- Python para:

  * Pré-processamento.
  
  * Análise exploratória, visualização e geração de insights.
  
  * Aplicação de modelos de machine learning (K-Means e regressão linear)
  
  
  * Principais pacotes utilizados:Pandas, Seaborn, Numpy, scikit-learning, statsmodels.
 
 
  * Aplicação de transformação para normalização de distribuição dos dados.
  
  

- Conceitos aplicados:

  * Programação orientada à objetos

  * Pré-processamento de dados

  * Data-wrangling
    
  * Data-Viz com geoprocessamento
  
  * Machine learning (com K-Means e regressão linear)
  
  * Expressões regulares
  
  * Estatística e probabildiade na interpretação da saída dos modelos.
  
  
## Funcionalidades


- A analise foi conduzida para, ao final, proporcionar uma webapp que fará previsões sobre o valor de seguro contra incêndio cobrado, de acordo com a área do imóvel.

## Visualizar


1 - Acesse clicando no arquivo acima com extensão '.ipynb', neste repositório, ou


2 - Faça o clone do repositório para participar deste projeto.

## Resultados


Como resultado da análise, idenfificamos, as correlações entre as variáveis, para iniciar a modelagem da regressão linear:


![image](https://user-images.githubusercontent.com/96034581/218281250-858cc153-fd0b-4946-912b-47768d6bb5a9.png)



Descartamos algumas, e verificamos a existência de relação linear entre as variáveis de interesse:


![image](https://user-images.githubusercontent.com/96034581/218281289-6d9c6ab3-0930-4ee7-b62b-af4c34a0cdae.png)


Vimos que, o algortmo de agrupamento aplicado descartou as impressões iniciais, sobre a existência de dois grupos:

![image](https://user-images.githubusercontent.com/96034581/218281337-41ac7eaf-f309-4786-974b-062ef0ae730b.png)

Ao fina, verificamos que, a assimetria da das variáveis de interesse é tamanha, que interefere na validação das suposições do modelo de regressão linear:

![image](https://user-images.githubusercontent.com/96034581/218281381-1503323d-c428-405d-a941-302274ac5506.png)

Por fim, aplicamos algumas técnicas matemáticas, visando a normalização da distribuição destas variáveis, e, decidmos dar seguimento ao trabalho em uma nova branch, tendo em vista as alterações que se fazem necessárias, no código:

![image](https://user-images.githubusercontent.com/96034581/218281416-d7e20e9e-51c1-447d-9f01-0c8f6c309a89.png)



## Conclusão



Realizando alguns agrupamentos e sumarização dos dados, e analisando as saída do modelo aplicaco, pode-se perceber que, a distribuição dos resíduos não chega nem perto de uma distribuição normal, e, quando relacionados à variável alvo, percebe-se que os coeficientes estão completamente enviezados.

Nosso modelo preditivo está bem modelado (as variáveis parecem atender ao objetivos, e possuem relação linear), mas, teremos que aplicar alguma técnica matemática para normalizar a distruição dos atributos escolhidos, sem perda ou alteração de informação, o que será feito em um segundo momento.


## Referências


Fonte dos dados: 


1 - [kaggle](https://www.kaggle.com/datasets/rubenssjr/brasilian-houses-to-rent)

2 - Repositório do Cientista de Dados Franklin Ferreira: https://franklin390.github.io/Project_03_Netflix_Investor_Quarterly_Earnings/
