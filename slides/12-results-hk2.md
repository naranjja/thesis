# Resultados
***
Seguimiento



### Correlaciones entre variables numéricas
![](img/num-corr.png)



### Resultados del *clustering*
![](img/hk2-clusters.png)



Todos los asesores
![](img/hk2-cluster1.svg)



Los buenos asesores
![](img/hk2-cluster2.svg)



Los malos asesores
![](img/hk2-cluster3.svg)



### Resultados de los modelos



### LightGBM
![](img/hk1-cm-lgbm.png)
$e_1 = 77.41\%$, $e_2 = 57.14\%$



### RandomForestClassifier
![](img/hk1-cm-rf.png)
$e_1 = 70\%$, $e_2 = 56.75\%$



### ExtraTreesClassifier
![](img/hk1-cm-et.png)
$e_1 = 80.64\%$, $e_2 = 54.34\%$



### Importancia de las variables
![](img/hk1-fe1.png)



Importancia de las variables de mayor incertidumbre
![](img/hk1-fe2.png)



### Ranking final
Variables más discriminantes



- El número de operaciones
- El porcentaje de créditos heredados
- Si es que el asesor es comercial senior
- Si es que el asesor es comercial junior 1
- Si es que el asesor trabaja en una zona rural
- Los meses de antigüedad del asesor en la organización
- La variación en el saldo capital
- El porcentaje de créditos con cero cuotas canceladas
- Si es que se encuentra casado
- El valor de la pregunta 3
- El valor de la pregunta 13
- Si es que postula al cargo de asesor comercial junior 2



### Recomendaciones
- Eliminar las preguntas 2, 28, 8, 25, 23 y 29
- Revisar correlación entre:
  - Las variables correspondientes a las cuotas canceladas
  - El número de operaciones y el nivel de productividad
  - La edad y la antigüedad en la empresa



### Análisis de sensibilidad
- $x_1$: número de operaciones
- $x_2$: porcentaje de créditos heredados
- $x_3$: meses de antigüedad en la organización
- $x_4$: número de desembolsos en la última semana
- $x_5$: variación del saldo capital



- $\Delta_{x_1} < 0 \rightarrow (\hat{y} = 2 \rightarrow \hat{y} = 0)$
- $\Delta_{x_2} > 0 \rightarrow (\hat{y} = 2 \rightarrow \hat{y} = 0)$
- $\Delta_{x_3} > 0 \rightarrow \hat{y} = 2$
- $\Delta_{x_4} < 0 \rightarrow (\hat{y} = 2 \rightarrow \hat{y} = 0)$
- $\Delta_{x_5} < 0 \rightarrow (\hat{y} = 0 \rightarrow \hat{y} = 2)$



### Modelo final
- Accuracy: $53.84\%$ ($\Delta = +0.24pp$)
- Exhaustividad: $83.96\%$ ($\Delta = +23.96pp$)
