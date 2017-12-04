# Marco teórico
***



Conjunto de herramientas:
  - Interpretables
  - Flexibles
  - Estables
  - *Kitchen sink**



### *Clustering*
- Las técnicas de *clustering* permiten dividir los datos en grupos (clústeres) que sean similares entre ellos y distintos de los demás.
- Aplicación como herramienta descriptiva:
  - Explorar
  - Resumir
  - Mejorar el poder predictivo de los modelos*



### HDBSCAN
- Algoritmo de *clustering* jerárquico basado en densidades
  - Extensión de DBSCAN
- Busca las zonas densas separadas por las que no son densas
  - No todos los puntos están en un cluster (elimina el ruido )



![](img/distance1.svg)



![](img/distance5.svg)



Mientras más pequeños los círculos, más densa el área. <br> Luego se halla el *minimum spanning tree*.



![](img/how_hdbscan_works_10_1.png)



### Árboles de decisión regresivos
- Modelos de alta interpretabilidad
- Inicialización aleatoria
- Minimización por etapas (en cada decisión)
  - ID3: Entropía o ganancia de información*
  - Otras métricas de desempeño
- Existen muchos árboles de decisión correctos*



![](img/id3.png)



### Métodos de ensamblaje
Agrupar los resultados para generar uno que sea más útil que cada uno independientemente

- ***Bagging*** (multiconjuntos de misma cardinalidad que los datos originales): reduce variancia
- ***Boosting*** (subconjuntos y luego combinación con función de costo): reduce sesgo
- ***Stacking*** (combinar modelos débiles en uno fuerte): aumenta poder predictivo y reduce tiempo*



### Ensamblaje de árboles
- ***Random Forest*** (*bagging*)
  - Multitud de árboles ID3 y luego hallar la moda
- ***Extremely Randomized Trees*** (*stacking*)
  - Multitud de árboles ID3 modificados ($n$ decisiones aleatorias y se escoje la mejor)
- ***Light Gradient Boosting Machine*** (*boosting*)
  - Multitud de árboles anchos* altamente correlacionados con la gradiente negativa de la función de pérdida escogida



### Modelos utilizados
- *Scikit-Learn*:
  - *RandomForestClassifier*
  - *RandomForestRegressor*
  - *ExtraTreesClassifier*
  - *ExtraTreesRegressor*
- *LightGBM*



### Ranking de variables
- Las variables que reducen más la entropía (FI)
- Las variables más correlacionadas con el objetivo (CFI)
- Las variables que generan mayores sinergias (RFE)
- Las variables que añaden menor ruido (PBFE)



### Análisis de sensibilidad
- LIME: explicaciones locales, interpretables y agnósticas a los modelos
  - Identifica un modelo a partir de los resultados
  - Permite probar los cambios rápidamente para encontrar sensibilidades



![](img/lime.png)
