---
layout: page
title: Boosting
---

En este articulo voy a dar una introduccion al aprendizaje por ensambles con principal foco en boosting. Partamos de la base de modelos sencillos como regresion lineal o logistica como estandares para la resolucion de problemas de regresion o clasificacion. Algo que nos era dificil con estos modelos era explicar comportamientos no lineales, uno debe hacer una ingeneriera de features para incorporar interacciones no lineales entre las variables. Un metodo de ajuste que funciona muy bien con las no linealidades es el arbol de decision.


## Arboles de decision:

Un arbol de decision es un metodo no parametrico de ajuste, es decir no busca una relacion parametrica entre la variable target y las variables explicativas $ y=f(x)$. Consiste en la particion iterativa del espacio de fases asignando un valor constante a cada region. Su construccion es bastante intuitiva asi como su interpretacion visual. 
Por ejemplo:

Un ejemplo de clasificacion en dos variables y con estos datos:

![](https://github.com/carabedo/carabedo.github.io/raw/main/assets/img/dt_0.png)


Iterativamente vamos particionando el espacio de fases de manera de elegir las regiones que mejor ajusten a los datos.

![](https://github.com/carabedo/carabedo.github.io/raw/main/assets/img/dt_1.png)

#### Como elegimos y armamos las regiones?

Este es un proceso iterativo, se utiliza alguna metricas para decidir en cada paso una particion binaria en alguna variable. Ademas es jerarquico, en cada iteraccion se hace una eleccion de variable y de threshold que maximice el error cuadratico medio.

#### Por que usar arboles de decision?

Los árboles son muy fáciles de explicar a las personas.
Parecen más cercanos a la forma en la que las personas toman decisiones 
Pueden ser representados gráficamente, pueden ser interpretados por no expertos fácilmente (especialmente si son pequeños)
Pueden manejar fácilmente predictores cualitativos sin necesidad de crear variables dummy.

#### Por que no usar arboles de decision?

En general no tienen el mismo nivel de precisión en la predicción comparados con otros enfoques para regresión y clasificación vistos previamente. 
Además pueden ser poco robustos. Un pequeño cambio en los datos puede generar un gran cambio el árbol final estimado. Sin embargo al agregar muchos árboles de decisión usando métodos como bagging, random forests, y  boosting la performance predictiva de los árboles puede mejorarse sustancialmente. 





## Por que Esambles?

El problema de un modelo con un solo arbol de decision es el overfitting, una solucion a esto es usar un ensamble de arboles. Si ajustamos 50 arboles de decision y luego promediamos sus resultados podremos evitar el overfitting. A esto se lo conoce como bagging, otra manera de realizar estos ensambles es boosting.
Boosting consiste en entrenar varios modelos de manera secuencial, entrenando un nuevo modelo sobre los datos que menor permormance tuvo el modelo anterior. 

## adaboost


## gradient boost


### xgboost

### lightbm

### catboost

