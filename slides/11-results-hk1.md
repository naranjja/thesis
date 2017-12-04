# Resultados
***
Admisión



### Correlaciones entre preguntas
![](img/question-corr.png)



### Definición de variable objetivo
![](img/target-def.png)



### Definición de clases relativas
![](img/target-mg.png)



### Frecuencia de observaciones perteneciente a las clases
![](img/class-freq.png)



### Resultados del *clustering*



Gráficos con los 3 clusters



Gráficos con los clusters de los buenos



Gráficos con los clusters de los malos



### Resultados de los modelos



CM del LightGBM



CM del Random Forest



CM del ExtraTrees



### Importancia de las variables



### Importancia de las variables de mayor incertidumbre



### Ranking final



1. El valor de la pregunta 13
2. Si es que el candidato postula al cargo de asesor comercial senior
3. El valor de la pregunta 29
4. Si es que el candidato postula al cargo de asesor comercial junior 2
5. El valor de la pregunta 30
6. El valor de la pregunta 10



7. El valor de la pregunta 27
8. El valor de la pregunta 23
9. El valor de la pregunta 5
10. El valor de la pregunta 1
11. El género del candidato
12. El valor de la pregunta 18



### Recomendaciones
- Eliminar las preguntas 25, 11 y 3
- Revisar correlación entre el nivel de ingresos y postulación al cargo de asesor comercial junior 1



### Análisis de sensibilidad
- $\Delta_{p_5} > 0 \rightarrow \hat{y} > 0$
- $\Delta_{p_{10}} > 0 \rightarrow (\hat{y} = 0 \rightarrow \hat{y} = 2)$
- $\Delta_{p_{11}} < 0 \rightarrow (\hat{y} = 0 \rightarrow \hat{y} = 2)$
- $\Delta_{p_{13}} > 0 \rightarrow (\hat{y} = 2 \rightarrow \hat{y} = 0)$
- $\Delta_{p_{18}} < 0 \rightarrow \hat{y} < 2$
- $\Delta_{p_{19}} < 0 \rightarrow \hat{y} = 2$



### Modelo final
- *Accuracy*: $48.38\%$ ($\Delta = +3.48pp$)
- Exhaustividad: $80.64\%$ ($\Delta = +28.24pp$)
