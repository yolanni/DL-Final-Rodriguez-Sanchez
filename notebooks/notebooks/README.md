📊 Predicción de Riesgo Crediticio — Caso Lending Club

🧠 Contexto del problema
Lending Club es una plataforma financiera que conecta inversionistas con personas que solicitan préstamos.
Uno de sus principales desafíos es identificar qué clientes tienen alta probabilidad de incumplir sus pagos (default), ya que esto representa pérdidas económicas.


🎯 Objetivo
Desarrollar un modelo de predicción que permita estimar el riesgo crediticio de un cliente, con el fin de apoyar la toma de decisiones al momento de aprobar o rechazar un préstamo.


📁 Dataset
Se utilizó el dataset histórico de préstamos de Lending Club (2007–2018), que contiene información real de clientes.

Se transformó el problema en una clasificación binaria:
0 → Cliente cumple con el pago (Fully Paid)
1 → Cliente incumple (Default / Charged Off)


⚙️ Tecnologías utilizadas

Python
Pandas y NumPy
Scikit-learn
TensorFlow / Keras


🤖 Modelo implementado
🧠 Deep Learning (MLP)

Se desarrolló un modelo de red neuronal tipo Multi-Layer Perceptron (MLP):
Capas densas con activación ReLU
Dropout para evitar sobreajuste
Capa de salida con activación sigmoide
Este modelo permite capturar relaciones no lineales entre las variables del cliente y su comportamiento de pago.


📈 Resultados

El modelo fue evaluado utilizando métricas como:
Accuracy
F1-score
ROC-AUC
Precision y Recall


📌 Resultado clave:
El modelo logra identificar de forma efectiva a los clientes con mayor riesgo de incumplimiento, manteniendo un buen equilibrio entre precisión y recall.

🧪 Proceso del modelo
Limpieza y preparación de datos
Balanceo de clases
Escalado de variables
Entrenamiento del modelo
Evaluación con métricas


💼 Valor para el negocio

Este modelo puede ser utilizado por Lending Club para:
Reducir el riesgo de otorgar préstamos a clientes con alta probabilidad de default
Mejorar la toma de decisiones crediticias
Optimizar la rentabilidad del portafolio de préstamos


🚀 Cómo ejecutar el proyecto

Abrir el notebook en Google Colab
Ejecutar todas las celdas
Revisar resultados


💡 Conclusiones

El Deep Learning permite modelar patrones complejos en datos financieros
El modelo es útil para apoyar decisiones en el sector crediticio
La implementación es reproducible y escalable
