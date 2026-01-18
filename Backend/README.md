# API de Predicción de Sentimiento
FastApi

# Asegúrarse de tener Python instalado
python --version

# Crear el entorno virtual para aislar las dependencias del proyecto
python -m venv venv

# Activar el entorno virtual
.\venv\Scripts\Activate

# Instalar dependencias:
pip install joblib scikit-learn fastapi uvicorn

# Inicia la aplicación:
uvicorn app:app --reload

# Consumo de API de Sentimiento – Postman

## URL
http://localhost:8000/predict

---

## Método
POST

---

## Headers
| Key | Value |
|---|---|
| Content-Type | application/json |

---

## Body (raw → JSON)
```json
{
  "text": "esta película es fea, la peor que he visto en años"
}
```
## Respuesta
```json
{
    "prevision": "Negativo",
    "probabilidad": 0.9825
}
```

