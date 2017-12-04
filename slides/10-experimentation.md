# Experimentación
***



### Contexto
- Organización microfinanciera en el Perú
- Altos costos de generar flujos de datos nuevos
- La base de la pirámide peruana
- Optimizar calidad de cartera de clientes a través de la calidad de los asesores
- Información lingüística



### Dos modelos predictivos
1. Admisión
2. Seguimiento

Clasificación multiclase con clases relativas
  - Priorización del error tipo 1 (*recall*)



### Integración del proceso propuesto



![](img/fc-process.svg)



### Descripción de los datos
- Muestra de 768 asesores
- Ingresos desde enero a marzo de 2017
  - Octubre como referencia para el seguimiento



### Lista de variables



### Admisión
- 30 preguntas al jurado (*float*)
- Cargo al que postula (*string*)
- Edad (*integer*)
- Estado civil (*string*)
- Género (*string*)
- Nivel de ingresos (*string*)



### Admisión y segumiento
- Antigüedad en la organización (*float*)
- Ratio de crecimiento de deuda (*float*)
- Número de instituciones financieras cercanas (*integer*)
- Zona de trabajo del asesor (*string*)
- Tenencia de créditos heredados (*boolean*)
- Tenencia de amonestaciones y suspensiones (*boolean*)



- Número de operaciones desembolsadas (*integer*)
- Porcentaje de desembolsos en la última semana (*float*)
- Variación porcentual del saldo capital (*float*)
- Porcentaje de créditos con cero cuotas canceladas (*float*)
- Participación en la escuela de formación (*boolean*)
