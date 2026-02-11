# Previsão Hierárquica e Reconciliação de Séries Temporais

## Objetivo
Desenvolver e avaliar modelos de previsão para séries temporais organizadas em estruturas hierárquicas.
O projeto busca produzir estimativas precisas nos níveis desagregados garantindo, ao mesmo tempo, coerência com os totais agregados.

---

## Problema
Previsões feitas de forma independente em diferentes níveis de agregação normalmente não fecham entre si.
Essa inconsistência gera dificuldades operacionais e reduz a confiabilidade para tomada de decisão.
Este projeto implementa técnicas de reconciliação que impõem coerência com ganho de acurácia.
---

## Dados
- Painel mensal de indicadores  
- Múltiplos níveis hierárquicos (unidade → área → região → total)  
- Amostra longa que permite avaliação fora da amostra  

---

## Metodologia
- Geração de previsões base com modelos de séries temporais  
- Reconciliação hierárquica (bottom-up, top-down e abordagens ótimas)  
- Comparação de desempenho fora da amostra  
- Avaliação via métricas de erro  

---

## Estrutura do Repositório
base_forecast.R    # geração das previsões iniciais
data_processing.R  # ingestão, limpeza e organização dos dados
reconciliation.R   # aplicação dos métodos de reconciliação hierárquica

data_base/         # dados originais
data_treated/      # bases tratadas e prontas para modelagem
