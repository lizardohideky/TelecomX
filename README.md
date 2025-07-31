![Image_Alt](https://github.com/lizardohideky/TelecomX/blob/main/imagen_colab.png)

# 📚 README - Análisis de Evasión de Clientes (Churn) - TelecomX LATAM

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
git clone https://github.com/tu-usuario/telecomx-churn-analysis.git
cd telecomx-churn-analysis
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
**Rol:** Analista de Datos  
**Empresa:** TelecomX LATAM  
**Fecha:** Julio 2025
