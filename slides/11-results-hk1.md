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



Gráficos con los 3 clusters



Gráficos con los clusters de los buenos



Gráficos con los clusters de los malos



### Resultados de los modelos



![](img/hk1-cm-lgbm.png)



![](img/hk1-cm-rf.png)



![](img/hk1-cm-et.png)



### Importancia de las variables
![](img/hk1-fe1.png)



### Importancia de las variables de mayor incertidumbre
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
- $\Delta_{p11} < 0 \rightarrow (\hat{y} = 0 \rightarrow \hat{y} = 2)$
- $\Delta_{p13} > 0 \rightarrow (\hat{y} = 2 \rightarrow \hat{y} = 0)$
- $\Delta_{p18} < 0 \rightarrow \hat{y} < 2$
- $\Delta_{p19} < 0 \rightarrow \hat{y} = 2$



### Modelo final
- *Accuracy*: $48.38\%$ ($\Delta = +3.48pp$)
- Exhaustividad: $80.64\%$ ($\Delta = +28.24pp$)
