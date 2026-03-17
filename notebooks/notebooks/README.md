Predicción de Riesgo Crediticio — Lending Club

🧠 Problema

El sistema financiero enfrenta el desafío de identificar préstamos con alta probabilidad de incumplimiento (**default**), lo que impacta directamente en la rentabilidad y riesgo de las instituciones.

Este proyecto aborda la predicción de riesgo crediticio utilizando datos reales de préstamos de Lending Club.



🎯 Objetivo

Desarrollar un sistema integral que permita:

* Predecir la probabilidad de incumplimiento de un cliente
* Optimizar decisiones de crédito
* Explicar las decisiones del modelo (interpretabilidad)
* Integrar modelos de Machine Learning, Deep Learning y LLMs


📁 Dataset

* Fuente: Lending Club (2007–2018)
* Más de 2 millones de registros
* Variables financieras, crediticias y de comportamiento

Se filtraron estados relevantes:

* ✅ Fully Paid → 0
* ❌ Charged Off / Default → 1



⚙️ Tecnologías utilizadas

* Python
* Pandas / NumPy
* Scikit-learn
* TensorFlow / Keras
* LightGBM
* Optuna
* InterpretML (EBM)


🔬 Modelos implementados

📌 Machine Learning

* **EBM (Explainable Boosting Machine)** → modelo interpretable
* **HistGradientBoosting**
* **LightGBM**

✔ Se optimizaron hiperparámetros con Optuna
✔ Se utilizó SMOTETomek para balancear clases

---

🧠 Deep Learning

Se implementó una red neuronal tipo **MLP (Multi-Layer Perceptron)**:

* Capas densas con activación ReLU
* Dropout para evitar overfitting
* Salida sigmoide para clasificación binaria

El modelo permite capturar relaciones no lineales complejas en los datos.



🤖 LLM (Large Language Model)

Se integró un pipeline que genera un **payload estructurado** para un modelo de lenguaje (LLM).

¿Qué hace el LLM?

* Recibe la predicción del modelo
* Usa factores de riesgo explicados por EBM
* Genera una **carta de decisión crediticia profesional**

✔ Evita alucinaciones (datos estructurados)
✔ Explica decisiones de forma clara para usuarios



📈 Resultados

🔹 Modelos de Machine Learning

* ROC-AUC ≈ 0.70
* F1 (Default) ≈ 0.69
* Buen balance entre precisión y recall

🔹 Deep Learning (MLP)

* Captura relaciones complejas
* Comparable con modelos tradicionales
* Útil para escalabilidad y patrones no lineales

📌 Conclusión:
Los modelos de Machine Learning fueron más interpretables, mientras que Deep Learning aporta flexibilidad y capacidad de generalización.



🧩 Pipeline de decisión

El sistema final combina:

1. Reglas de negocio (políticas)
2. Lógica difusa
3. Predicción del modelo ML
4. Explicaciones del modelo (EBM)
5. Generación de texto con LLM

Resultado: decisión final = APPROVE / REVIEW / DECLINE

---

🧪 Casos de prueba

Se evaluaron tres escenarios:

* 🟢 Bajo riesgo → REVIEW
* 🟡 Riesgo medio → DECLINE
* 🔴 Alto riesgo → DECLINE (con violaciones de política)


📂 Estructura del proyecto

```id="code1"
notebooks/
 └── proyecto_final.ipynb
```


