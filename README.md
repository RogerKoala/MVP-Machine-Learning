# MVP Sprint 2 - Previsão de Inadimplência em Cartão de Crédito

## Objetivo

Desenvolver e comparar modelos de classificação para prever se um cliente de cartão de crédito irá inadimplir no mês seguinte, com base em seu perfil demográfico e histórico de pagamentos dos últimos 6 meses.

## Dataset

[Default of Credit Card Clients](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)

- 30.000 clientes de um banco de Taiwan (abr/2005 a set/2005)
- Aproximadamente 22% são inadimplentes (dataset desbalanceado)

### Variáveis

- `LIMIT_BAL`: limite de crédito concedido
- `SEX`, `EDUCATION`, `MARRIAGE`, `AGE`: perfil demográfico
- `PAY_0` a `PAY_6`: status de pagamento nos últimos 6 meses
- `BILL_AMT1` a `BILL_AMT6`: valor da fatura nos últimos 6 meses
- `PAY_AMT1` a `PAY_AMT6`: valor pago nos últimos 6 meses
- `default.payment.next.month`: 0 (adimplente), 1 (inadimplente)

## Modelos avaliados

- Baseline (Dummy Classifier)
- Regressão Logística
- Random Forest
- Gradient Boosting
- LightGBM (otimizado via RandomizedSearchCV)
- MLP em PyTorch (apêndice comparativo)

## Autor

Heitor Reyes Sanches
