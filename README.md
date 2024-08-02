# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Este é um desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas proposto pelo Lab DIO. O AWS SageMaker Canvas é uma ferramenta poderosa que permite criar modelos de machine learning sem a necessidade de escrever código. Abixo temos a descrição do processo passo a passo para usar o SageMaker Canvas para criar previsões de estoque.

## 📋 Pré-requisito

É necessário ter uma conta na AWS. Instruções de criação de conta são encontradas em [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).


## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

O objetivo do estudo é usar o **SageMaker Canvas** para **criar previsões de estoque baseadas em Machine Learning (ML)**. As etapas para o cumprimento do desafio são as seguintes:


## 🚀 Passo a Passo

### 1. Selecionar Dataset

-   Navegue até a pasta `datasets` deste repositório, que contém datasets que podem ser usados para treinar e testar o modelo de ML. O SageMaker Canvas também oferece acesso a datasets internos, como dados de amostra para treinamento e previsão. Esses datasets podem ser enriquecidos, e outros podem ser usados: quanto mais apurados, mais relevante será o resultado.
-   Escolha o dataset que será usado para treinar o modelo de previsão de estoque (se estiver usando dados próprios, eles podem ser importados de várias fontes, como S3, Snowflake, ou CSVs locais).
-   Faça o upload do dataset no SageMaker Canvas.

### 2. Acessar o Sagemaker Canvas

-   Acesse o AWS Management Console: certifique-se de que a conta tem permissões adequadas para usar o SageMaker.
-   Inicie o SageMaker Canvas. No Console, procure o SageMaker e selecione a opção “Canvas” para abrir a interface do usuário.

### 3. Construir/Treinar

-   No SageMaker Canvas, importe o dataset que foi selecionado.
-   Clique em “Import data” para adicionar seus próprios dados ou escolher datasets de amostra disponíveis.
-   Configure as `variáveis de entrada` e as `variáveis de saída` de acordo com os dados.
-   Visualize seus dados no Canvas para entender a estrutura e a distribuição. Isso é essencial para prever corretamente.
-   Remova dados duplicados ou inconsistentes.
-   Trate valores ausentes usando técnicas apropriadas, como média, mediana, ou modos de imputação.
-   Crie novas features, se necessário, para melhorar a precisão do modelo.
-   Realize a codificação de variáveis categóricas e normalização de dados numéricos.
-   **Seleção de Objetivo**: Especifique a coluna que você deseja prever, como o nível de estoque ou a demanda futura.
-   **Tipo de Modelo**: O SageMaker Canvas seleciona automaticamente o tipo de modelo apropriado, como regressão para previsões de estoque.
-   Clique em “**Build**” para permitir que o Canvas treine o modelo usando algoritmos de ML. O Canvas executa uma análise automática de dados para determinar o melhor modelo baseado nos dados fornecidos.
-   Inicie o treinamento do modelo. Isso pode levar algum tempo, dependendo do tamanho do dataset.

### 4. Analisar

-   Após o treinamento, examine as métricas de performance do modelo. Analise RMSE (Root Mean Square Error), MAE (Mean Absolute Error) ou precisão para avaliar o desempenho do modelo.
-   Utilize gráficos e dashboards para visualizar o desempenho e os padrões identificados pelo modelo.
-   Verifique as principais características que influenciam as previsões.
-   Baseado na avaliação, faça ajustes no modelo ou nos parâmetros de entrada para melhorar a performance se necessário e treine novamente até obter um desempenho satisfatório.

### 5. Prever

-   Use o modelo treinado para fazer previsões de estoque. 
-   Exporte os resultados e analise as previsões geradas para entender as tendências e os padrões nas previsões de estoque.
-   Documente suas conclusões e qualquer insight obtido a partir das previsões.
-   Os resultados das previsões podem ser exportados para CSV ou outros formatos compatíveis para compartilhar ou integrar com outras ferramentas de análise. Considere integrar as previsões com sistemas ERP ou de gerenciamento de inventário para automação.

### 6. Conclusão

Usar o SageMaker Canvas simplifica o processo de criar previsões baseadas em ML, **mesmo para usuários sem experiência em programação**. A chave para o sucesso é a preparação e o entendimento dos dados, o que garante que o modelo seja preciso e útil para prever estoque de forma eficaz.
