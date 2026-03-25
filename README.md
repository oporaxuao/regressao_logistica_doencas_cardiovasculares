Predição de Doenças Cardiovasculares com Regressão Logística 🏥
Este projeto foi desenvolvido como parte do Módulo 27 do curso de Ciência de Dados, focado na implementação e análise de um modelo de Regressão Logística para identificar a propensão a doenças cardiovasculares com base em dados clínicos e hábitos de vida.

📋 Visão Geral
O objetivo principal foi construir um classificador binário capaz de prever se um paciente possui ou não doença cardiovascular (cardio_disease), utilizando variáveis como idade, peso, altura, níveis de glicose, consumo de álcool e atividade física.

🛠️ Tecnologias e Ferramentas
Linguagem: Python

Ambiente: PyCHarm / Jupyter Notebook

Bibliotecas Principais: * Pandas e NumPy (Manipulação de dados)

Seaborn e Matplotlib (Visualização de dados)

Scikit-Learn (Machine Learning e Métricas)

Imbalanced-learn (SMOTE para balanceamento de classes)

🚀 Etapas do Projeto
1. Pré-processamento e Limpeza
Tratamento de separadores decimais e conversão de tipos de dados.

Análise de outliers em variáveis físicas (altura e peso).

Padronização de escala com StandardScaler para garantir a convergência do modelo linear.

2. Análise Exploratória (EDA)
Uso de Boxplots e Violin Plots para identificar que a idade e o peso são fatores de risco visualmente distintos entre os grupos.

Matriz de correlação para identificar relações entre hábitos (como fumo e álcool) e a variável alvo.

3. Balanceamento de Dados (SMOTE)
Devido à leve disparidade entre as classes no dataset original, utilizei a técnica SMOTE (Synthetic Minority Over-sampling Technique) para equilibrar a base de treino em 50/50, evitando vieses no treinamento.

4. Modelo de Machine Learning
Algoritmo: Regressão Logística.

Performance: O modelo atingiu uma AUC-ROC de 0.70, demonstrando um poder de discriminação aceitável para um baseline clínico.

Insights dos Coeficientes: A análise dos pesos revelou que a Idade e o nível de Glicose foram os preditores mais impactantes para o diagnóstico positivo.

📊 Resultados Técnicos
Acurácia: 64%

AUC-ROC: 0.70

Equilíbrio: O modelo apresentou métricas de Precisão e Recall balanceadas, indicando uma boa capacidade de generalização sem overfitting.

✍️ Autor
João - Graduado em Análise e Desenvolvimento de Sistemas e Estudante de Ciência de Dados.
