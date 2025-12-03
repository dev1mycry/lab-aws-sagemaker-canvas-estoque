# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Siga os passos abaixo para completar o desafio!

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira nosso repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).


## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

- Dê um fork neste projeto e reescreva este `README.md`. Sinta-se à vontade para detalhar todo o processo de criação do seu Modelo de ML para uma "Previsão de Estoque Inteligente".
- Para isso, siga o [passo a passo] descrito a seguir e evolua as suas habilidades em ML no-code com o Amazon SageMaker Canvas.
- Ao concluir, envie a URL do seu repositório com a solução na plataforma da DIO.


## 🚀 Passo a Passo da Resolução 

### 1. Selecionar Dataset

-   Naveguei até a pasta `datasets` deste repositório e com ajuda da IA Copilot o enriqueci com novas colunas e dados.
-   Usei como premissa de prompt o uso real dos dados para a IA me oferecer tanto a ideia de enriquecimento como dados técnicos que poderia ser usados no SageMaker Canvas.
-   A IA me orientou a usar o Python para preencher as colunas faltantes; também, o Google Colab, como plataforma de código. Depois de acrescentar colunas e ajustar o dataset fiz o upload no SageMaker Canvas.
  ![image](https://github.com/dev1mycry/lab-aws-sagemaker-canvas-estoque/blob/main/datasets/Captura%20de%20tela%202025-12-02%20224414.png)

### 2. Construir/Treinar

-   No SageMaker Canvas importei o dataset, configurando como *target* a coluna QUANTIDADE_ESTOQUE.
-   Coloquei *configure model* saída temporal baseada em 7 dias.
-   Iniciei o treinamento do modelo no modo *preview* para ver as métricas antecipadamente, e, para poder melhorá-las, perguntei a IA. As opções foram bem técnicas, então optei por um treinamento *standard* que aumentaria a acurância do modelo e tornaria as métricas menores segundo aprendi nas aulas. E foi o que ocorreu! 🙌
- **Métricas do preview mode:**

![image](https://github.com/dev1mycry/lab-aws-sagemaker-canvas-estoque/blob/main/datasets/Captura%20de%20tela%202025-12-02%20235533.png)
![image](https://github.com/dev1mycry/lab-aws-sagemaker-canvas-estoque/blob/main/datasets/Captura%20de%20tela%202025-12-02%20235600.png)
![image](https://github.com/dev1mycry/lab-aws-sagemaker-canvas-estoque/blob/main/datasets/Captura%20de%20tela%202025-12-02%20235623.png)

- **Métricas no modo stardard:**

![image](https://github.com/dev1mycry/lab-aws-sagemaker-canvas-estoque/blob/main/datasets/Captura%20de%20tela%202025-12-03%20013302.png)

### 3. Analisar

-   Após o treinamento, as métricas foram bem baixas, sendo satisfatórias para o que foi proposto na configuração do modelo.
-   Como o modelo foi explorado no range temporal de 7 dias, dificilmente as métricas viriam altas.
  

### 4. Prever

-   As previsões de estoque veio em linha no que foi pedido, que era uma amostra preditiva do estoque em 7 dias.
    ![image](https://github.com/dev1mycry/lab-aws-sagemaker-canvas-estoque/blob/main/datasets/Captura%20de%20tela%202025-12-03%20014353.png)
    ![image](https://github.com/dev1mycry/lab-aws-sagemaker-canvas-estoque/blob/main/datasets/single_prediction_results.png)
-   No gráfico podemos ver as métricas P10, P50 e P90, que indicam como está a demanda no período, e mostrando a variação do estoque nos dias.
    
## 🤙 Conclusões e Agradecimentos 🙌

Enfim, consegui fazer o desafio, aprendendo pela primeira vez sobre Machine Learning. Já tenho noção de algumas coisas e ajuda muito, mas é algo novo que merece mais atenção, não é só por que é no-code que é fácil. Treinar uma IA é divertido e dá trabalho! Vou aprender mais. Que pena que na AWS não tenha algo para praticar *free forever*! 😅 
Agradeço a todos envolvidos no curso! Vamos por mais! DIO está no meu ❤️!
