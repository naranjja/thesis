# Resultados
***
Admisión



### Correlaciones entre preguntas
![](img/question-corr.png)



### Definición de variable objetivo
![](img/target-def.png)



### Definición de clases relativas
![](img/target-mg.png)



### Observaciones pertenecientes a las clases
![](img/class-freq.png)



### Resultados del *clustering*
![](img/hk1-clusters.png)



Todos los asesores
![](img/hk1-cluster1.svg)



Los buenos asesores
![](img/hk1-cluster2.svg)



Los malos asesores
![](img/hk1-cluster3.svg)



### Resultados de los modelos



### LightGBM
![](img/hk1-cm-lgbm.png)
$e_1 = 74.19\%$, $e_2 = 46.93\%$



### RandomForestClassifier
![](img/hk1-cm-rf.png)
$e_1 = 83.87\%$, $e_2 = 39.39\%$



### ExtraTreesClassifier
![](img/hk1-cm-et.png)
$e_1 = 80.34\%$, $e_2 = 38.46\%$



### Importancia de las variables
![](img/hk1-fe1.png)



Importancia de las variables de mayor incertidumbre
![](img/hk1-fe2.png)



### Ranking final
Variables más discriminantes



- El valor de la pregunta 13
- Si es que postula al cargo de asesor comercial senior
- El valor de la pregunta 29
- Si es que postula al cargo de asesor comercial junior 2
- El valor de la pregunta 30
- El valor de la pregunta 10
- El valor de la pregunta 27
- El valor de la pregunta 23
- El valor de la pregunta 5
- El valor de la pregunta 1
- El género del candidato
- El valor de la pregunta 18



### Recomendaciones
- Eliminar las preguntas 25, 11 y 3
- Revisar correlación entre el nivel de ingresos y postulación al cargo de asesor comercial junior 1



### Análisis de sensibilidad
- $\Delta_{p5} > 0 \rightarrow \hat{y} > 0$
- $\Delta_{p10} > 0 \rightarrow (\hat{y} = 0 \rightarrow \hat{y} = 2)$
- $\Delta_{p30} < 0 \rightarrow (\hat{y} = 0 \rightarrow \hat{y} = 2)$
- $\Delta_{p13} > 0 \rightarrow (\hat{y} = 2 \rightarrow \hat{y} = 0)$
- $\Delta_{p18} < 0 \rightarrow \hat{y} < 2$
- $\Delta_{p29} < 0 \rightarrow \hat{y} = 2$



### Modelo final
- Accuracy: $48.38\%$ ($\Delta = +3.48pp$)
- Exhaustividad: $80.64\%$ ($\Delta = +28.24pp$)
