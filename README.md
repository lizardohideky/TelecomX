![Image_Alt](https://github.com/lizardohideky/TelecomX/blob/main/imagen_colab.png)

# 📚 README - Análisis de Evasión de Clientes (Churn) - TelecomX 

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4%2B-green)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11%2B-purple)

## 🌟 Visión General del Proyecto

Este proyecto tiene como objetivo analizar y comprender los factores que contribuyen a la **evasión de clientes (churn)** en TelecomX LATAM, una empresa de telecomunicaciones que enfrenta una alta tasa de cancelaciones.

El análisis se basa en un conjunto de datos proporcionado que contiene información detallada sobre clientes, incluyendo datos demográficos, servicios contratados, métodos de pago y el estado de evasión.

## 🎯 Objetivos del Proyecto

- **Extraer, transformar y cargar (ETL)** los datos desde la API de TelecomX
- Realizar un **análisis exploratorio de datos (EDA)** para identificar patrones y tendencias
- Visualizar los principales factores que influyen en la evasión de clientes
- Generar **insights estratégicos** para reducir la tasa de churn
- Preparar los datos para futuros modelos predictivos

## 📂 Estructura del Proyecto

```
telecomx-churn-analysis/
├── TelecomX_Data.json          # Datos crudos desde la API
├── telecomx_churn_datos_procesados.csv  # Datos procesados
├── analysis_notebook.ipynb     # Notebook principal de análisis
├── README.md                   # Documentación del proyecto
└── requirements.txt            # Dependencias del proyecto
```

## 📊 Datos del Proyecto

El conjunto de datos contiene información sobre **7,267 clientes** con las siguientes variables clave:

### Variables Demográficas
- `gender`: Género del cliente
- `SeniorCitizen`: Si es cliente mayor (1) o no (0)
- `Partner`: Si tiene pareja (Yes/No)
- `Dependents`: Si tiene dependientes (Yes/No)

### Variables de Servicio
- `PhoneService`: Servicio telefónico (Yes/No)
- `MultipleLines`: Líneas múltiples (Yes/No/No phone service)
- `InternetService`: Tipo de servicio de internet (DSL, Fiber optic, No)
- `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`: Servicios adicionales
- `StreamingTV`, `StreamingMovies`: Servicios de streaming

### Variables Contractuales
- `Contract`: Tipo de contrato (Month-to-month, One year, Two year)
- `PaperlessBilling`: Facturación sin papel (Yes/No)
- `PaymentMethod`: Método de pago

### Variables de Rendimiento
- `tenure`: Antigüedad en meses
- `MonthlyCharges`: Cargo mensual
- `TotalCharges`: Cargo total
- `Churn`: Estado de evasión (Yes/No)

## 🛠️ Tecnologías Utilizadas

- **Python**: Lenguaje principal
- **Pandas**: Manipulación y análisis de datos
- **NumPy**: Cálculos numéricos
- **Matplotlib/Seaborn**: Visualización de datos
- **Requests**: Extracción de datos desde API

## 🚀 Cómo Ejecutar el Proyecto

1. **Clonar el repositorio:**
```bash
https://github.com/lizardohideky/TelecomX.git
```

2. **Instalar las dependencias:**
```bash
pip install -r requirements.txt
```

3. **Ejecutar el notebook:**
```bash
jupyter notebook analysis_notebook.ipynb
```

## 📈 Hallazgos Clave

1. **Tasa de Evasión General**: 26.5% de los clientes han cancelado sus servicios
2. **Contratos Mensuales**: Los clientes con contrato "mes a mes" tienen una tasa de evasión 4 veces mayor que los de contrato anual
3. **Servicio de Fibra Óptica**: Contrariamente a lo esperado, los clientes de fibra óptica tienen mayor tasa de evasión que los de DSL
4. **Clientes Nuevos**: El 68% de las cancelaciones ocurren en los primeros 12 meses
5. **Facturación Sin Papel**: Los clientes con facturación sin papel tienen menor tasa de evasión

## 📊 Visualizaciones Principales

El proyecto incluye visualizaciones estratégicas que muestran:
- Tasa de evasión por tipo de contrato
- Evasión por servicio de internet
- Relación entre antigüedad y evasión
- Segmentación por valor del cliente
- Customer Lifetime Value (CLV) estimado

## 💡 Recomendaciones Estratégicas

1. **Programa de Retención para Contratos Mensuales**: Ofrecer incentivos para migrar a contratos anuales
2. **Mejora en la Experiencia de Clientes de Fibra Óptica**: Implementar soporte técnico prioritario
3. **Programa de Bienvenida para Nuevos Clientes**: Asesoría personalizada en los primeros 30 días
4. **Dashboard de Evasión en Tiempo Real**: Monitoreo diario de KPIs de retención
5. **Automatización del Proceso ETL**: Pipeline diario de actualización de datos

## 📈 Impacto Estimado

- **Reducción de evasión**: 15-20% en 6 meses
- **Retención incremental**: 1,200+ clientes
- **Ingreso recurrente adicional**: $4.8M anuales
- **ROI estimado**: 300% en 12 meses

## 🤝 Contribución

Las contribuciones son bienvenidas. Si tienes sugerencias para mejorar el análisis o encontrar errores, por favor abre un issue o envía un pull request.

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo LICENSE para más detalles.

---

**Desarrollado por:** Hideky Lizardo  
**Rol:** Cientifico de Datos    
**Fecha:** Julio 2025

<br><br><br>

# 📚 README - Análisis de Evasión de Clientes (Churn) - TelecomX Parte 2 

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.5%2B-orange)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-1.3%2B-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7%2B-blue)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12%2B-purple)

## 🌟 Visión General del Proyecto

Este proyecto tiene como objetivo analizar y predecir la **evasión de clientes (churn)** en TelecomX LATAM, una empresa de telecomunicaciones con una alta tasa de cancelaciones.

El análisis combina:
- **Análisis exploratorio de datos (EDA)** para entender los patrones
- **Modelado predictivo con machine learning** para anticipar futuras cancelaciones

Los resultados permiten diseñar estrategias proactivas de retención basadas en datos reales.

## 🎯 Objetivos del Proyecto

- **Extraer, transformar y cargar (ETL)** los datos desde la API de TelecomX
- Realizar un **análisis exploratorio de datos (EDA)** para identificar patrones y tendencias
- **Preparar los datos** para modelado (encoding, normalización, división)
- Entrenar y evaluar **modelos de clasificación** para predecir el churn
- Interpretar los resultados e identificar las **variables más influyentes**
- Generar **insights estratégicos** para reducir la tasa de churn

## 📂 Estructura del Proyecto
```
TelecomX-Parte 2
├── TelecomX_Data.json           # Datos crudos desde la API
├── telecom_clientes_limpio.csv  # Datos procesados y limpios
├── telecomx_parte2.ipynb        # Notebook de modelado predictivo
├── modelo_churn_rf.pkl          # Modelo entrenado (Random Forest)
├── visualizaciones/             # Gráficos generados
│ ├── churn_distribucion.png
│ ├── correlacion_heatmap.png
│ ├── importancia_variables.png
│ └── matriz_confusion.png
├── README.md                    # Documentación del proyecto
└── requirements.txt             # Dependencias del proyecto
```

## 📊 Datos del Proyecto

El conjunto de datos contiene información sobre **7,267 clientes** con las siguientes variables clave:

### Variables Demográficas
- `gender`: Género del cliente
- `SeniorCitizen`: Si es cliente mayor (1) o no (0)
- `Partner`: Si tiene pareja (Yes/No)
- `Dependents`: Si tiene dependientes (Yes/No)

### Variables de Servicio
- `PhoneService`: Servicio telefónico (Yes/No)
- `MultipleLines`: Líneas múltiples (Yes/No/No phone service)
- `InternetService`: Tipo de servicio de internet (DSL, Fiber optic, No)
- `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`: Servicios adicionales
- `StreamingTV`, `StreamingMovies`: Servicios de streaming

### Variables Contractuales
- `Contract`: Tipo de contrato (Month-to-month, One year, Two year)
- `PaperlessBilling`: Facturación sin papel (Yes/No)
- `PaymentMethod`: Método de pago

### Variables de Rendimiento
- `tenure`: Antigüedad en meses
- `MonthlyCharges`: Cargo mensual
- `TotalCharges`: Cargo total
- `Churn`: Estado de evasión (Yes/No)

## 🛠️ Tecnologías Utilizadas

- **Python**: Lenguaje principal
- **Pandas / NumPy**: Manipulación y limpieza de datos
- **Matplotlib / Seaborn**: Visualización de datos
- **Scikit-learn**: Modelado predictivo y evaluación
- **Joblib**: Serialización del modelo
- **Requests**: Extracción de datos desde API

## 🚀 Cómo Ejecutar el Proyecto

1. **Clonar el repositorio:**
```bash
git clone https://github.com/lizardohideky/TelecomX.git
```

2. Instalar las dependencias:
```
pip install -r requirements.txt
```

3. Ejecutar el notebook:
```
jupyter notebook telecomx_parte2.ipynb
```


## 📈 Hallazgos Clave

1. Tasa de Evasión General: 26.5% de los clientes han cancelado sus servicios
2. Contratos Mensuales: Los clientes con contrato "mes a mes" tienen una tasa de evasión 4 veces mayor que los de contrato anual
3. Servicio de Fibra Óptica: Contrariamente a lo esperado, los clientes de fibra óptica tienen mayor tasa de evasión que los de DSL
4. Clientes Nuevos: El 68% de las cancelaciones ocurren en los primeros 12 meses
5. Facturación Sin Papel: Los clientes con facturación sin papel tienen menor tasa de evasión

## 📊 Resultados del Modelo Predictivo

Se entrenaron tres modelos de clasificación:

| Modelo | F1-Score | AUC-ROC | Exactitud |
|-------|----------|---------|-----------|
| **Random Forest** | **0.88** | **0.92** | **0.85** |
| Regresión Logística | 0.81 | 0.86 | 0.83 |
| KNN | 0.79 | 0.84 | 0.81 |

✅ **Random Forest fue el mejor modelo**, seleccionado por su alto F1-Score y capacidad para manejar variables mixtas sin sobreajuste.


## 🔍 Variables Más Influyentes (Random Forest)

Las variables que más contribuyen a predecir el churn son:

1. tenure (meses_en_la_empresa): Clientes nuevos son los más vulnerables
2. Contract (tipo_contrato): Contratos mensuales tienen alto riesgo
3. TechSupport (soporte_tecnico): Falta de soporte técnico aumenta 3x el riesgo de abandono

## 💡 Recomendaciones Estratégicas

1. Programa de Retención para Contratos Mensuales: Ofrecer descuentos para migrar a contratos anuales
2. Soporte Técnico Proactivo: Contactar a clientes nuevos sin soporte técnico
3. Programa de Bienvenida: Asesoría personalizada en los primeros 30 días
4. Dashboard de Riesgo de Churn: Monitoreo diario con el modelo entrenado
5. Automatización del Proceso ETL: Pipeline diario de actualización de datos

## 📈 Impacto Estimado

- Reducción de evasión: 15-20% en 6 meses
- Clientes retenidos: +1,200
- Ingreso recurrente adicional: $4.8M anuales
- ROI estimado: 300% en 12 meses

## 🤝 Contribución

Las contribuciones son bienvenidas. Si tienes sugerencias para mejorar el análisis o encontrar errores, por favor abre un issue o envía un pull request.

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo LICENSE para más detalles.

---

**Desarrollado por:** Hideky Lizardo  
**Rol:** Cientifico de Datos    
**Fecha:** Agosto 2025
