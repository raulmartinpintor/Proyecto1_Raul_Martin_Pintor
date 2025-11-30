🚗 Proyecto: Análisis Exploratorio, Limpieza y Visualización de un Dataset de Coches


📘 Descripción general

Este proyecto tiene como objetivo realizar un análisis completo sobre un dataset de automóviles. El dataset fue obtenido de Kaggle.

El trabajo se divide en tres fases principales:

- Exploración inicial del dataset
- Limpieza y estandarización de datos
- Visualización y análisis final

Cada fase se desarrolla en un notebook independiente para mantener un flujo de trabajo claro y ordenado.



📂 Estructura del repositorio
data/
 ├── dataset_sucio_para_limpieza.csv
 └── dataset_limpio.csv

notebooks/
 ├── 1_eda_exploracion.ipynb
 ├── 2_eda_limpieza.ipynb
 └── 3_eda_visualizacion.ipynb

README.md
requirements.txt



🔍 1. Exploración inicial

En el notebook 1_eda_exploracion.ipynb se realiza:

• Carga del dataset
• Revisión de dimensiones
• Inspección de columnas y tipos de datos
• Resumen estadístico
• Conteo de valores únicos
• Identificación de valores faltantes
• Búsqueda de duplicados
• Detección de inconsistencias
• Observación de problemas como:
    • Columnas en tipo object con números y texto mezclado
    • Más de 17 tipos diferentes de asientos
    • 37 valores distintos de combustible
    • Potencia y cilindrada con formatos incorrectos
    • Precios con símbolos y rangos
    • Velocidades y aceleraciones sin estandarizar

Conclusión: el dataset requiere una limpieza profunda.



🧹 2. Limpieza y transformación

En el notebook 2_eda_limpieza.ipynb se aplican los siguientes procesos:

• Renombrado de columnas a nombres limpios
• Eliminación de símbolos ($, €, cc, hp, “km/h”, etc.)
• Conversión de columnas numéricas a int o float
• Normalización de categorías (Ej. Petrol, Diesel, Hybrid)
• Estandarización de unidades
• Tratamiento de nulos

Resultado: creación del archivo "dataset_limpio.csv" para poder ver los coches.



📊 3. Visualización y análisis

En el notebook 3_eda_visualizacion.ipynb se generan:

• Histogramas para analizar la distribución de variables numéricas.
• Gráficos de barras para comparar marcas, combustibles y tipos de motor.
• Boxplots para detectar valores extremos y analizar rangos.
• Scatterplots para estudiar relaciones entre variables como potencia, torque y velocidad.
• Lineplots para visualizar tendencias generales.
• Conclusiones basadas en los diagramas.


📌 Conclusiones finales

Todo el análisis, la limpieza de datos y las visualizaciones presentadas se han realizado exclusivamente a partir del dataset seleccionado. 

Con este trabajo se ha completado el proceso de exploración y comprensión del dataset, ofreciendo una visión clara y estructurada de sus características principales.