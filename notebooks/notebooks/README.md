📊 Predicción de Riesgo Crediticio con Deep Learning


🧠 Problema
Las instituciones financieras necesitan identificar qué clientes tienen alta probabilidad de incumplir un préstamo (default), para reducir riesgos y tomar mejores decisiones de crédito.


🎯 Objetivo
Desarrollar un modelo capaz de predecir si un cliente pagará o no su préstamo, utilizando técnicas de Machine Learning y Deep Learning.


📁 Dataset
Se utilizó el dataset de Lending Club (2007–2018), que contiene información de préstamos reales.

Se transformó el problema en clasificación binaria:
0 → Cliente paga (Fully Paid)
1 → Cliente incumple (Default / Charged Off)


⚙️ Tecnologías utilizadas

Python
Pandas y NumPy
Scikit-learn
TensorFlow / Keras


🤖 Modelos implementados
🔹 Machine Learning
Se utilizaron modelos tradicionales para establecer una línea base.

🔹 Deep Learning (Modelo principal)
Se implementó una red neuronal tipo MLP (Multi-Layer Perceptron):

Capas densas con activación ReLU
Dropout para evitar overfitting
Salida sigmoide para clasificación binaria
Este modelo permite capturar relaciones complejas en los datos.


📈 Resultados

El modelo fue evaluado con las siguientes métricas:
Accuracy
F1-score
ROC-AUC
Precision y Recall


📌 Resultado clave:
El modelo logra un buen equilibrio entre precisión y recall para detectar clientes en riesgo.

🧪 Proceso del modelo
Limpieza y preparación de datos
Balanceo de clases
Escalado de variables
Entrenamiento del modelo MLP
Evaluación con métricas


🚀 Cómo ejecutar el proyecto

Abrir el notebook en Google Colab
Ejecutar todas las celdas
Revisar resultados y métricas


💡 Conclusiones
El modelo permite predecir riesgo crediticio de forma efectiva
Deep Learning captura patrones complejos en los datos
Este tipo de solución puede apoyar la toma de decisiones financieras

