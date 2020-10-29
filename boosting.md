---
layout: page
title: Boosting
---

En este articulo voy a dar una introduccion al aprendizaje por ensambles con principal foco en boosting. Partamos de la base de modelos sencillos como regresion lineal o logistica como estandares para la resolucion de problemas de regresion o clasificacion. Algo que nos era dificil con estos modelos era explicar comportamientos no lineales, uno debe hacer una ingeneriera de features para incorporar interacciones no lineales entre las variables. Un metodo de ajuste que funciona muy bien con las no linealidades es el arbol de decision.


## Arboles de decision:

Un arbol de decision es un metodo no parametrico de ajuste, es decir no busca una relacion parametrica entre la variable target y las variables explicativas $ y=f(x)$. Consiste en la particion iterativa del espacio de variables asignando un valor constante a cada region. Su construccion es bastante intuitiva asi como su interpretacion visual. 
Por ejemplo:

Un ejemplo de clasificacion en dos variables y con estos datos:
![]('/assets/img/dt_0.png')

Iterativamente vamos particionando el espacio de variables de manera de elegir las regiones que mejor ajusten a los datos.

![]('/assets/img/dt_1.png')

## por que boosting?

El problema de un modelo con un solo arbol de decision es el overfitting, una solucion a esto es usar un ensamble de arboles. Si ajustamos 50 arboles de decision y luego promediamos sus resultados podremos evitar el overfitting. A esto se lo conoce como bagging, otra manera de realizar estos ensambles es boosting.
Boosting consiste en entrenar varios modelos de manera secuencial, entrenando un nuevo modelo sobre los datos que menor permormance tuvo el modelo anterior. 

## adaboost


## gradient boost


### xgboost

### lightbm

### catboost

