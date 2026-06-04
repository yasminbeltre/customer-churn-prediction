# 📊 Predictor de Abandono de Clientes con Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yasminbeltre/Yasminbeltre/blob/main/customer_churn_prediction.ipynb)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-orange?logo=googlecolab)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-green?logo=scikit-learn)
![Estado](https://img.shields.io/badge/Estado-Completado-brightgreen)

Sistema de predicción que identifica qué clientes de una empresa de telecomunicaciones tienen mayor probabilidad de abandonar el servicio (**churn**), utilizando modelos de Machine Learning entrenados con datos reales.

---

## 📌 Tabla de Contenidos

- [Descripción](#descripción)
- [Objetivo](#objetivo)
- [Dataset](#dataset)
- [Tecnologías](#tecnologías)
- [Modelos implementados](#modelos-implementados)
- [Resultados](#resultados)
- [¿Cómo ejecutarlo?](#cómo-ejecutarlo)
- [Aplicación práctica](#aplicación-práctica)
- [Autora](#autora)

---

## 📝 Descripción

Este proyecto forma parte de un portafolio de Inteligencia Artificial aplicada al negocio. A partir de datos históricos de clientes de telecomunicaciones, se construyeron y compararon modelos supervisados para predecir el abandono de clientes antes de que ocurra, permitiendo acciones preventivas de retención.

---

## 🎯 Objetivo

Ayudar a las empresas a tomar decisiones preventivas sobre retención de clientes, identificando patrones de comportamiento que predicen el abandono con anticipación, reduciendo así el costo de adquisición de nuevos clientes.

---

## 📦 Dataset

| Atributo | Detalle |
|---|---|
| **Fuente** | [Telco Customer Churn – IBM/GitHub](https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv) |
| **Registros** | ~7,000 clientes |
| **Variables** | 21 características (demográficas, de servicio y facturación) |
| **Variable objetivo** | `Churn` (Sí / No) |

---

## 🛠️ Tecnologías utilizadas

| Herramienta | Uso |
|---|---|
| Python 3 | Lenguaje principal |
| Google Colab | Entorno de ejecución |
| Pandas | Manipulación y análisis de datos |
| Scikit-learn | Modelos de Machine Learning |
| Matplotlib / Seaborn | Visualización de datos |

---

## 🤖 Modelos implementados

| Modelo | Accuracy | Precisión (weighted) | Recall (weighted) | F1-Score (weighted) |
|---|---|---|---|---|
| Regresión Logística | 78.54% | 77% | 79% | 78% |
| **Random Forest** | **79.25%** | **78%** | **79%** | **78%** |

> ✅ El modelo **Random Forest** fue seleccionado como modelo final por su mejor desempeño general.

---

## 📈 Resultados

### Variable con mayor impacto en el abandono

| Variable | Importancia |
|---|---|
| `TotalCharges` (cargos totales acumulados) | ⭐⭐⭐⭐⭐ Más alta |
| `tenure` (antigüedad del cliente) | ⭐⭐⭐⭐ Alta |
| `Contract` (tipo de contrato) | ⭐⭐⭐⭐ Alta |

### Hallazgos clave

- La variable **`TotalCharges`** fue identificada como el predictor más importante del abandono.
- Los clientes con contratos **mes a mes** presentan una tasa de abandono significativamente mayor.
- El modelo Random Forest identificó correctamente clientes en riesgo con **79.25% de accuracy**.

---

## 📂 Contenido del repositorio

```
├── customer_churn_prediction.ipynb   # Notebook principal con todo el análisis y código
├── requirements.txt                  # Dependencias del proyecto
└── README.md                         # Documentación del proyecto
```

---

## 🚀 ¿Cómo ejecutarlo?

1. Abre el archivo `customer_churn_prediction.ipynb` en Google Colab.
2. Ejecuta las celdas en orden desde el menú **Entorno de ejecución → Ejecutar todo**.
3. El dataset se carga automáticamente desde internet — no necesitas descargar nada.

---

## 💼 Aplicación práctica

Este sistema puede integrarse en estrategias de **Customer Success** para:

- Priorizar llamadas de retención hacia clientes en riesgo.
- Diseñar ofertas personalizadas antes de que el cliente tome la decisión de irse.
- Reducir el **churn rate** y maximizar el **Customer Lifetime Value (CLV)**.

---

## 👤 Autora

**Yasmin Beltre**
Customer Success & Operations Specialist | AI Portfolio – INDOTEL/BID/CYMETRIA 2026
📍 Santo Domingo, República Dominicana
🔗 [LinkedIn](https://linkedin.com/in/yasminbeltre) | [GitHub](https://github.com/yasminbeltre)

---

*Proyecto desarrollado como parte del programa de formación en Inteligencia Artificial INDOTEL/BID/CYMETRIA 2026.*
