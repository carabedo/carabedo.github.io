---
layout: page
title: Boosting
---

En este articulo voy a explicar boosting, un metodo de aprendizaje por ensambles.


## por que arboles de decision?

Si uno quiere capturar comportamientos no lineales dentro de un sistema, una opcion es el uso de arboles de decision, un modelo no parametrico y no lineal. Ademas de ser no lineal permite una facil interpretacion.

## por que boosting?

El problema de un modelo con un solo arbol de decision es el overfitting, una solucion a esto es usar un ensamble de arboles. Si ajustamos 50 arboles de decision y luego promediamos sus resultados podremos evitar el overfitting. A esto se lo conoce como bagging, otra manera de realizar estos ensambles es boosting.
Boosting consiste en entrenar varios modelos de manera secuencial, entrenando un nuevo modelo sobre los datos que menor permormance tuvo el modelo anterior. 

## adaboost


## gradient boost


### xgboost

### lightbm

### catboost

