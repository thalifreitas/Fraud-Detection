# 💳 Credit Card Transactions Fraud Detection

>  Este projeto simula um cenário real de detecção de fraude financeira e tem como objetivo desenvolver um modelo de Machine Learning capaz de identificar transações fraudulentas com cartão de crédito, minimizando falsos negativos.

Questionamentos levantados inicialmente:

- [x] Existe alguma relação entre a distância geográfica da transação em relação à localização residencial do titular e a probabilidade de a transação ser fraudulenta?

- [x] Existe relação entre o horário da transação e a probabilidade de ocorrência de fraude?
  
- [x] Existe relação entre o dia da semana que a transação foi realizada e a probabilidade de ocorrência de fraude?

- [x] Existe relação entre o mês que a transação foi realizada e a probabilidade de ocorrência de fraude? Há meses que possuem maior probabilidade de ocorrência de transações fraudulentas?

- [ ] A frequência de transações em janelas curtas de tempo aumenta a probabilidade de uma operação ser fraudulenta? Qual intervalo de tempo seria esse?

- [x] Existe relação entre a idade do titular do cartão e a probabilidade de ocorrência de fraude?

##
Inicialmente foi feita uma análise exploratória dos dados, entendendo a relação de cada variável com a variável alvo, e identificando quais variáveis tinham maior contribuição na detecção de fraudes. 

A base de dados foi dividia em três conjuntos: treino, validação e teste.

Dois modelos de Machine Learning foram testados nessa base de dados, sendo eles **_Regressão Logística_** e **_Random Forest_**.

Como conclusão, o modelo de Random Forest foi o que apresentou melhor performance.
##

Na avaliação final, os seguintes resultados para as métricas de avaliação foram encontrados:
```
Accuracy: 1.00

Classification Report:
               precision    recall  f1-score   support

           0       1.00      1.00      1.00    368526
           1       0.97      0.65      0.78      1953

    accuracy                           1.00    370479
   macro avg       0.98      0.82      0.89    370479
weighted avg       1.00      1.00      1.00    370479



Confusion Matrix:
+--------+--------+
| 368488 |   38   |
+--------+--------+
|  685   |  1268  |
+--------+--------+

F2-Score: 0.6953279227900856

Specificity: 0.9998968865154697

NPV: 0.9981445013584417

```

Fonte: [Credit Card Transactions Fraud Detection Dataset](https://www.kaggle.com/datasets/kartik2112/fraud-detection)
