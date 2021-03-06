# Projeto Airbnb Rio - Ferramenta de Previsão de Preço de Imóvel para pessoas comuns

<br />
<p align="center">
  <a href="https://upload.wikimedia.org/wikipedia/commons/thumb/6/69/Airbnb_Logo_B%C3%A9lo.svg/2560px-Airbnb_Logo_B%C3%A9lo.svg.png">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/69/Airbnb_Logo_B%C3%A9lo.svg/2560px-Airbnb_Logo_B%C3%A9lo.svg.png"  width="600" height="200">
  </a>
  
## Contexto
No Airbnb, qualquer pessoa que tenha um quarto ou um imóvel de qualquer tipo (apartamento, casa, chalé, pousada, etc.) pode ofertar o seu imóvel para ser alugado por diária.

Você cria o seu perfil de host (pessoa que disponibiliza um imóvel para aluguel por diária) e cria o anúncio do seu imóvel.

Nesse anúncio, o host deve descrever as características do imóvel da forma mais completa possível, de forma a ajudar os locadores/viajantes a escolherem o melhor imóvel para eles (e de forma a tornar o seu anúncio mais atrativo).

Existem dezenas de personalizações possíveis no seu anúncio, desde quantidade mínima de diária, preço, quantidade de quartos, até regras de cancelamento, taxa extra para hóspedes extras, exigência de verificação de identidade do locador, etc.

## Objetivo
Construir um modelo de previsão de preço que permita uma pessoa comum que possui um imóvel possa saber quanto deve cobrar pela diária do seu imóvel.

Ou ainda, para o locador comum, dado o imóvel que ele está buscando, ajudar a saber se aquele imóvel está com preço atrativo (abaixo da média para imóveis com as mesmas características) ou não.

## O que temos disponível, inspirações e créditos
- As bases de dados foram retiradas do site [Kaggle](https://www.kaggle.com/allanbruno/airbnb-rio-de-janeiro)

- Elas estão disponíveis para download no repositório(se você puxar os dados direto do Kaggle pode ser que encontre resultados diferentes dos meus, afinal as bases de dados podem ter sido atualizadas).

- Caso queira uma outra solução, pode olhar como referência a solução do usuário Allan Bruno do kaggle no [Notebook](https://www.kaggle.com/allanbruno/helping-regular-people-price-listings-on-airbnb)

- Há semelhanças entre a solução que vamos desenvolver aqui e a dele, mas também algumas diferenças significativas no processo de construção do projeto.

- As bases de dados são os preços dos imóveis obtidos e suas respectivas características em cada mês.
- Os preços são dados em reais (R$).
- Temos bases de abril de 2018 a maio de 2020, com exceção de junho de 2018 que não possui base de dados.

## Observação
- Os arquivos com Deploy no nome são iguais, pois para executar com o ***streamlit*** é necessário que o arquivo tenha a extensão ***py***.
- Certifique-se de ter instalado o Pandas[^1], Numpy[^2], Joblib[^3], Streamlit[^4], Pathlib[^5], Seaborn[^6], Matplotlib[^7], Plotly[^8] e Sklearn[^9].  

 [^1]: ```pip install pandas```
 [^2]: ```pip install numpy```
 [^3]: ```pip install joblib```
 [^4]: ```pip install streamlit```
 [^5]: ```pip install pathlib``` 
 [^6]: ```pip install seaborn```
 [^7]: ```pip install matplotlib``` 
 [^8]: ```pip install plotly``` 
 [^9]: ```pip install scikit-learn```  
  
## Run
- Execute primeiro ***Solução Final - Airbnb Rio***, assim obteremos o arquivo com a extensão ***.joblib***(não foi incluido nos arquivos disponíveis pois é pesado).
- Certifique-se que o arquivo gerado ***.joblib*** está na mesma pasta do ***DeployProjetoAirbnb.py***.
- Abrir o Anaconda Prompt ou o Terminal.
- Acessar a pasta aonde os arquivos estão.
- Executar um host para o usar o modelo:
``` 
// Selecionar o arquivo com a extensão .py
streamlit run DeployProjetoAirbnb.py
```

