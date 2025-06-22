# 🧠 Predicción de Precios de Casas con MLOps

Este proyecto aplica prácticas de MLOps para entrenar, versionar y desplegar un modelo de machine learning que predice el precio estimado de una casa según sus características.

---

## 🚀 Tecnologías usadas

- **Python 3.10**
- **Scikit-Learn** (modelo de regresión)
- **FastAPI** (API para inferencia)
- **Docker** (contenedorización)
- **MLflow** (seguimiento de experimentos)
- **Pydantic** (validación de datos)
- **Git + GitHub** (control de versiones)

---

## 📦 Estructura del proyecto

mlops_casas/
├── Dockerfile
├── main.py # API con FastAPI
├── entrenar_modelo.py # Script para entrenar y registrar el modelo con MLflow
├── datos.csv # Dataset de ejemplo
├── modelo_entrenado.joblib # Modelo serializado (opcional)
├── requirements.txt
└── README.md



---

## ⚙️ Cómo entrenar el modelo

1. Instalar dependencias:

```bash
pip install -r requirements.txt
Ejecutar entrenamiento:


python entrenar_modelo.py
Esto entrena el modelo y registra todo con MLflow.

📈 Visualizar los experimentos con MLflow

mlflow ui
Luego ir a: http://localhost:5000

🌐 Ejecutar la API con Docker
Construir imagen:


docker build -t mlops-fastapi .
Ejecutar contenedor:


docker run -p 8000:8000 mlops-fastapi
Probar la API en:

http://localhost:8000/docs

🧪 Endpoint /predecir_precio/
Método: POST

{
  "metros_cuadrados": 70,
  "habitaciones": 3
}
🔁 Respuesta:


{
  "precio_estimado": 123456.78
}
🧑‍💻 Autor
Valentín Olivero
📍 Río Tercero, Córdoba
🔗 LinkedIn

📝 Licencia
Este proyecto está bajo la Licencia MIT.
