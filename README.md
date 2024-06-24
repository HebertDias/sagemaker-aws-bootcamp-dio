# Previsão de Estoque inteligente com SageMakers Canvas 🤖

## Bootcamp Nexa - Machine Learning - DIO.

## 📖 Resumo

### O projeto final do bootcamp é utilizar um dataset para criar uma previsão de estoque inteligente baseando-se em Machine Learning No-Code através do SageMakers Canvas, da Amazon Web Service

![SageMaker](https://d2908q01vomqb2.cloudfront.net/da4b9237bacccdf19c0760cab7aec4a8359010b0/2023/11/16/AWS_Juxtaposer_Thumbnail_FINAL.png)

###### 🛎️ Este repositório é um passo a passo seguido por mim até o objetivo do projeto, também como uma forma pessoal de aprendizado enquanto explico. Pode haver erros em termos técnicos, ou abordagens rasas sobre o assunto. Não é um repositório informativo. O resultado está ao final da página.

## 🎯 Passo a Passo

### 📃 DATASET

- #### Meu dataset foi gerado através do generativo Chat-GPT, disponibilizado na pasta 'dataset', com as seguintes intruções:

![dataset-gpt](image.png)

### ☁️ SageMaker

- #### Fiz o upload do arquivo gerado pelo Chat-GPT e selecionei _Predective Analysis_ como meu _Problem type_, sendo ele direcionado a predizer meu estoque com base no histórico do arquivo CSV.

![SageMaker-new-model](image-2.png)

- #### Em _Select a column to predict_, selecionei a coluna ESTOQUE, a qual quero uma predição dos dados.

###### 🛎️ Há um aviso para a coluna PRECO. Segundo ao próprio SageMaker, é porque não há valores reais para os dias futuros onde serão feitas as predições, então decidi que ele trabalhará com a mediana entre os valores prescristos no arquivo CSV para finalização do projeto.

![SageMaker-predict](image-1.png)

- #### Em _Configure Model_, selecionei a coluna ID_PRODUTOS para identificar os itens da coluna ESTOQUE. Enquanto a coluna DIA será o período em que ocorreu as ações do arquivo. Fiz uma previsão de até 3 dias.

![SageMaker-configure-model](image-3.png)

- #### Há possibilidade de criar gráficos através do _Data Visualizer_

![alt text](image-4.png)

## 📊 Final!

#### 🛎️ Não consegui exatamente gerar uma predição geral dos dados do arquivo CSV por conta de limite da plaforma AWS, mas é possível visualizar predições específicas para cada item na aba _Single Prediction_. :)

- Item 12
  ![item-12](image-8.png)
- Item 11
  ![item-11](image-10.png)
- Item 10
  ![item-10t](image-9.png)

- #### Mensagem sobre o limite:
  ![alt text](image-7.png)

### Tecnologias utilizadas (e seu links):

[![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)](https://chat.openai.com/)
[![AWS](https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)](https://aws.amazon.com/pt/free/?)
