 # K-Nearest Neighbor (KNN)
 

 ## Descrição
 

 Este repositório contém um exemplo simplificado do algoritmo K-Nearest Neighbor (KNN) para classificação, aplicado a um dataset de doenças cardíacas. O KNN é um algoritmo de aprendizado de máquina supervisionado que pode ser usado para tarefas de classificação e regressão. Ele classifica novos pontos de dados com base na classe majoritária de seus K vizinhos mais próximos no espaço de características.
 

 ## Dataset
 

 O dataset utilizado é o "heart.csv", que contém informações sobre pacientes e a presença ou ausência de doença cardíaca. As colunas incluem dados como idade, sexo, tipo de dor no peito, pressão sanguínea em repouso, colesterol, entre outros.
 

 ## Código
 

 O script `knn_simples.py` implementa as seguintes etapas:
 

 1.  **Carregamento dos dados:** Carrega o dataset "heart.csv" utilizando a biblioteca pandas.
 2.  **Pré-processamento:**
  *   Remove a linha onde a pressão sanguínea em repouso (RestingBP) é igual a 0.
  *   Substitui os valores de colesterol iguais a 0 pela mediana dos valores não nulos.
  *   Codifica as variáveis categóricas (como sexo e tipo de dor no peito) em valores numéricos utilizando `LabelEncoder`.
 3.  **Divisão em treino e teste:** Divide o dataset em conjuntos de treino (70%) e teste (30%).
 4.  **Treinamento do modelo KNN:** Inicializa e treina o modelo KNN com os dados de treino. O número de vizinhos (k) é definido como 7.
 5.  **Teste do modelo:** Utiliza o modelo treinado para fazer previsões nos dados de teste.
 6.  **Avaliação do modelo:** Calcula a acurácia, gera a matriz de confusão e o relatório de classificação para avaliar o desempenho do modelo.
 

 ## Como Rodar o Código
 

 1.  **Clone o repositório:**
  ```bash
  git clone [URL do seu repositório]
  cd Aprendizagem-de-Mark/K-Nearest-Neighbor
