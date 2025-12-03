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

-   Naveguei até a pasta `datasets` deste repositório e com ajudar de uma IA o enriqueci com novas colunas e dados.
-   Usei como premissa de prompt o uso real dos dados para a IA me oferecer tanto a ideia de enriquecimento como dados técnicos que poderia ser usados no SageMaker Canvas.
-   A IA me orientou a usar o Python para preencher as colunas faltantes; também, o Google Colab, como plataforma de código. Depois de acrescentar colunas e ajustar o dataset fiz o upload no SageMaker Canvas.
-   imagem

### 2. Construir/Treinar

-   No SageMaker Canvas importei o dataset, configurando como *target* a coluna QUANTIDADE_ESTOQUE.
-   Coloquei *confire model* saída temporal baseada em 7 dias.
-   Iniciei o treinamento do modelo no modo preview para ver as métricas antecipadamente e como poderia melhorá-las perguntei a IA. As opções foram bem técnicas, então optei por um treinamento *standard* que aumentaria a acurancia do modelo e tornaria as métricas menores segundo aprendi nas aulas. E foi o que ocorreu! 🙌

### 3. Analisar

-   Após o treinamento, as métricas foram bem baixas, sendo satisfatórias para o que foi proposto na configuração do modelo.
-   Verifique as principais características que influenciam as previsões.
-   Faça ajustes no modelo se necessário e re-treine até obter um desempenho satisfatório.

### 4. Prever

-   As previsões de estoque veio em linha no que foi pedido, que era uma amostra em 7 dias.
-   Exporte os resultados e analise as previsões geradas.
-   Documente suas conclusões e qualquer insight obtido a partir das previsões.

## 🤔 Dúvidas?

Esperamos que esta experiência tenha sido enriquecedora e que você tenha aprendido mais sobre Machine Learning aplicado a problemas reais. Se tiver alguma dúvida, não hesite em abrir uma issue neste repositório ou entrar em contato com a equipe da DIO.
