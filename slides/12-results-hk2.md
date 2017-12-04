# Resultados
***
Admisión



### Correlaciones entre variables numéricas



### Resultados del *clustering*



Gráficos con los 2 clusters



Gráficos con los clusters de los buenos



Gráficos con los clusters de los malos



### Resultados de los modelos



CM del LightGBM



CM del Random Forest



CM del ExtraTrees



### Importancia de las variables



### Importancia de las variables de mayor incertidumbre



### Ranking final



1. El número de operaciones
2. El porcentaje de créditos heredados
3. Si es que el asesor es comercial senior
4. Si es que el asesor es comercial junior 1
5. Si es que el asesor trabaja en una zona rural
6. Los meses de antigüedad del asesor en la organización



7. La variación en el saldo capital
8. El porcentaje de créditos con cero cuotas canceladas
9. Si es que el asesor se encuentra casado
10. El valor de la pregunta 3
11. El valor de la pregunta 13
12. Si es que el asesor es comercial junior 2



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
- *Accuracy*: $53.84\%$ ($\Delta = +0.24pp$)
- Exhaustividad: $83.96\%$ ($\Delta = +23.96pp$)
