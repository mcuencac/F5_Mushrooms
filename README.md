# ML_Airlines_Grupo3

![](./assets/logo.png)

## 📁 **Estructura del Proyecto**

```bash
.
├── assets/                   # Recursos gráficos
├── data/                     # Datos usados para el análisis y predicciones
├── documentation/            # Documentación del proyecto
├── frontend/                 # Archivos del frontend, interfaz de usuario
├── metrics/                  # Archivos relacionados con métricas y evaluación
├── models_ml/                # Modelos entrenados y relacionados
├── notebooks/                # Jupyter Notebooks para análisis y experimentación
├── tests/                    # Pruebas automatizadas del proyecto
├── .gitignore                # Ignorar archivos y carpetas en git
├── README.md                 # Documentación principal del proyecto
└── requirements.txt          # Dependencias y librerías necesarias para el proyecto
```

## ⚙️ **Predicción de Satisfacción - Machine Learning**

Este proyecto implementa un sistema de predicción de satisfacción de clientes usando Machine Learning. La aplicación tiene dos componentes principales:

- 🖥️ **API construida con FastAPI** para procesar y predecir los datos.
- 🌐 **Interfaz de usuario desarrollada con Streamlit** para recolectar datos del usuario y mostrar predicciones en tiempo real.

### 🚀 Requisitos

Te recomendamos crear y activar un entorno virtual para gestionar las dependencias. Puedes hacerlo con los siguientes comandos:

```bash
python -m venv env  # Crea el entorno virtual con nombre 'env'
source env/bin/activate  # Activa el entorno en Unix/Mac
.\env\Scripts\Activate  # Activa el entorno en Windows
```

Para desactivar el entorno:
```bash
deactivate
```

Instala las dependencias ejecutando:

```bash
pip install -r requirements.txt
```

### 🛠️ **Características del Proyecto**

- **API en FastAPI**: Recibe solicitudes con datos del usuario y devuelve predicciones de satisfacción.
- **Interfaz en Streamlit**: Permite a los usuarios ingresar datos y recibir una predicción de forma visual e interactiva.
- **Modelo de Machine Learning**: Predice la satisfacción del cliente basado en varias características recolectadas.

### ▶️ **Cómo Ejecutar el Proyecto**

1. **API en FastAPI**  
   Para ejecutar la API, navega al directorio donde se encuentra `main.py` y ejecuta el siguiente comando:

   ```bash
   uvicorn app.main:app --reload
   ```

   Esto iniciará un servidor en `http://localhost:8000` donde puedes realizar solicitudes POST para obtener predicciones.

2. **Interfaz de Usuario en Streamlit**  
   Para lanzar la aplicación de Streamlit, navega al directorio donde se encuentra `app.py` y ejecuta:

   ```bash
   streamlit run streamlit_app.py
   ```

   Esto abrirá la aplicación en tu navegador, generalmente en `http://localhost:8501`.

### 🔍 **Cómo Funciona**

- **Entrenamiento del Modelo**: El modelo fue entrenado con un conjunto de datos que incluye variables como edad, ingresos, género, etc., para predecir la satisfacción del cliente.
- **Predicción**: El modelo toma como entrada los datos proporcionados y devuelve una predicción de la satisfacción.
- **Interfaz de Streamlit**: El usuario ingresa datos en la interfaz y ve los resultados de predicción.

### 🔧 **Próximos Pasos**

- Mejorar la precisión del modelo.
- Añadir autenticación a la API para mayor seguridad.
- Implementar validación de datos más robusta en FastAPI.
- Mejorar la interfaz de Streamlit con gráficos adicionales y análisis visual.

### 🤝 **Contribuciones**

Las contribuciones son bienvenidas. Si deseas colaborar, por favor abre un issue o un pull request.
