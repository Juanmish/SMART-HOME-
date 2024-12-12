#README

 #1. Introducción
 
 ● Objetivo principal: Desarrollar un modelo de machine learning para 
optimizar el consumo de energía en una smart home integrada con energías 
renovables.
 ● Alcance: Análisis de series temporales de consumo energético, predicción 
de generación de energía renovable y optimización del uso de dispositivos 
(ej: aire acondicionado).

 #2. Metodología
 
 ● Recopilación de datos:
 Fuente de datos: CSV con información de consumo energético de diversos 
dispositivos y variables ambientales.
 ● Exploratory Data Analysis (EDA):
 Visualizaciones: Gráficos de series temporales, histogramas, mapa de calor, 
matriz de correlación, etc.
 Análisis de correlación: Identificación de relaciones entre variables 
(temperatura, punto de rocío, temperatura aparente).
 ● Preprocesamiento de datos: 
Se elimina una fila que aparece con datos nulos y se convierten los valores 
categóricos en numéricos.
 ● Modelado:
 Algoritmo: Regresión lineal.
 Entrenamiento: Utilización de los datos para entrenar el modelo.
 ● Evaluación: 
Métricas de evaluación hallando R2 para medir la precisión del modelo.

# 3. Resultados

 ● Principales hallazgos:
 ○ Correlación significativa entre temperatura aparente, punto de rocío y 
consumo energético.
○ Desempeño del modelo de regresión lineal 0.989.
 Implicaciones:
 ○ Posibilidad de optimizar el consumo energético mediante la predicción 
de la demanda y la generación.
 ○ Beneficios económicos para el usuario y de tipo ambiental.
 
 #4. Conclusiones
 
 ● Resumen de los resultados:  El modelo de regresión lineal ha demostrado 
un desempeño excepcional con un coeficiente de determinación (R²) de 
0.989. Esto indica que el modelo explica casi el 99% de la variabilidad en el 
consumo energético en función de las variables independientes.
 ● Trabajo futuro:
 ○ Exploración de otros algoritmos de machine learning.
 ○ Incorporación de más variables (precios de la energía, hábitos de 
consumo).
 ○ Desarrollo de una interfaz de usuario más amigable.
 ○ Implementación en fábricas para que en las horas pico se consuma 
menos energía y se reduzcan significativamente los costos operativos.

# 5. Impacto

 ● Beneficios para el usuario:
 ○ Reducción de costos en las facturas de energía.
 ○ Mayor confort en el hogar.
 ○ Contribución a la sostenibilidad ambiental.
 Consideraciones Adicionales
 ● Visualizaciones: Incluye gráficos y visualizaciones para hacer más 
comprensible el análisis de datos.
 ● Datos: Puedes consultar la base de datos utilizada en: 
https://www.kaggle.com/code/koheimuramatsu/change-detection-forecasting-i
 n-smart-home
 Desafíos:
 ● Intermitencia de las fuentes de energía renovable: La generación de 
energía a partir de paneles solares u otras fuentes puede ser impredecible y 
depende de factores como la radiación solar o el viento, lo que complica la 
predicción de la cantidad exacta de energía disponible.
 ● Gestión de la variabilidad del consumo: Los hábitos de consumo de 
energía de los residentes pueden cambiar a lo largo del día o de la semana, 
lo que requiere que el modelo se adapte a esos patrones dinámicos.
● Optimización en tiempo real: El modelo debe ser capaz de tomar 
decisiones rápidas, ya que la demanda de energía y la generación de energía 
renovable pueden cambiar drásticamente en cuestión de minutos, y la 
optimización del consumo debe hacerse de manera eficiente para evitar el 
uso innecesario de energía de la red.
 ● Manejo de datos incompletos o ruidosos: Los datos de consumo y 
generación pueden estar incompletos o ser ruidosos debido a errores de 
medición, lo que puede afectar la precisión de las predicciones del modelo.

 #Guía detallada paso a paso
 
 Para usuarios menos familiarizados con Python y machine learning:
 1. Descarga el modelo: Haz clic en el botón "Descargar" en el repositorio y 
guarda el archivo en tu computadora.
 2. Crea un nuevo cuaderno de Colab: Ve a https://colab.research.google.com 
y crea un nuevo cuaderno de Python.
 3. Sube el modelo: En Colab, ve a "Archivo" > "Cargar" y selecciona el archivo 
del modelo que descargaste.
 4. Carga los datos: Para listar los archivos en la carpeta "Data" y luego carga 
los datos en un DataFrame de Pandas.
 5. Ejecuta el modelo: Carga el modelo guardado y utilízalo para hacer 
predicciones sobre los nuevos datos.
