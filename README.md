# 📊 Modelo de Previsão de Churn para Plataforma de Streaming

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)

## 📌 Objetivo
Desenvolver um modelo preditivo para identificar usuários com alta probabilidade de cancelamento (churn) em plataforma de streaming, permitindo ações preventivas para retenção de clientes.

## 🔍 Contexto do Projeto
- **Problema**: Alto índice de cancelamento de assinaturas
- **Solução**: Modelo de classificação para prever churn com base no comportamento do usuário
- **Fonte dos Dados**: Adaptação de dataset público do Kaggle sobre churn em e-commerce

## 🛠️ Tecnologias Utilizadas
- **Linguagem**: Python 3
- **Bibliotecas**:
  - Pandas, NumPy (análise de dados)
  - Scikit-learn (modelos de ML)
  - Matplotlib/Seaborn (visualização)
  - Imbalanced-learn (tratamento de dados desbalanceados)

## 📂 Estrutura do Projeto
1. **Análise Exploratória (EDA)**
   - Tratamento de dados faltantes
   - Análise de distribuição das variáveis
2. **Pré-processamento**
   - Codificação de variáveis categóricas
   - Normalização de features
   - Balanceamento de classes (SMOTE)
3. **Modelagem**
   - Regressão Logística
   - Random Forest
   - Balanced Random Forest
4. **Otimização**
   - Grid Search para tuning de hiperparâmetros
   - Validação cruzada
5. **Avaliação**
   - Métricas: Acurácia, Precision, Recall, F1-Score, ROC AUC
   - Matriz de Confusão
   - Curva ROC

## 📊 Resultados Principais
| Modelo | Acurácia | Precision | Recall | F1-Score | ROC AUC |
|--------|----------|-----------|--------|----------|---------|
| Regressão Logística | 0.80 | 0.00 | 0.00 | 0.00 | 0.50 |
| Random Forest | 0.81 | 0.67 | 0.15 | 0.25 | 0.68 |
| Balanced RF + SMOTE | 0.75 | 0.35 | 0.65 | 0.45 | 0.71 |

## 💡 Principais Descobertas
- Dataset altamente desbalanceado (80/20)
- Melhor performance com Balanced Random Forest + SMOTE
- Variáveis mais importantes para prever churn:
  1. Tempo na plataforma
  2. Tipo de assinatura
  3. Dispositivos conectados

## 🤝 Contribuição
Contribuições são bem-vindas! Siga estes passos:

1. Faça um fork do projeto

2. Crie uma branch (git checkout -b feature/improvement)

3. Commit suas mudanças (git commit -m 'Add some feature')

4. Push para a branch (git push origin feature/improvement)

5. Abra um Pull Request
