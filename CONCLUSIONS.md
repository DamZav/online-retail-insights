# Conclusiones – Análisis de Retail Online (2010–2011)

## Resumen Ejecutivo

El análisis exploró datos transaccionales de retail con el objetivo de comprender la dinámica de ingresos, comportamiento de clientes, desempeño de productos y concentración geográfica. Tras el proceso de limpieza y transformación de datos, se identificaron patrones estructurales clave del negocio.

---

## 1 Alcance del Dataset y Calidad de Datos

- **541,909 registros originales**
- **401,604 transacciones válidas** después de la limpieza
- **4,373 clientes únicos**
- **4,070 productos únicos**
- **38 países**

Se eliminaron:
- 5,268 registros duplicados
- 135,080 transacciones sin CustomerID (~26% del dataset)

Esto permitió garantizar consistencia en análisis a nivel cliente e ingresos.

---

## 2 Ingresos y Crecimiento

- **Ingresos totales (dataset limpio): ~8.28M**
- **Ingresos 2011: 7.7M (93% del total)**
- **Ingresos 2010: 552K (solo diciembre disponible)**

El volumen de ingresos en 2011 confirma que el negocio operó a escala estable durante ese año, mientras que 2010 contiene datos parciales.

---

## 3 Estacionalidad

Distribución de ingresos en 2011:

- **Primer semestre (Ene–Jun): 3.16M**
- **Segundo semestre (Jul–Dic): 4.55M**
- **~44% más ingresos en el segundo semestre**

Se observa una fuerte estacionalidad, probablemente asociada a campañas comerciales y temporada alta de fin de año. Esto sugiere potencial para modelos de forecasting con componente estacional.

---

## 4 Estructura del Ticket de Compra

Segmentación por monto total de transacción:

- **Bajo (<20): 78%**
- **Medio (20–100): 18%**
- **Alto (≥100): 3%**

El negocio opera bajo un modelo de **alto volumen y bajo ticket promedio**, donde la frecuencia y retención de clientes son factores críticos para la rentabilidad.

---

## 5 Devoluciones

- **8,872 transacciones de devolución**
- **~2.2% tasa de devolución**

La tasa es relativamente baja, lo que indica estabilidad operativa. Sin embargo, un análisis más profundo por producto o país podría identificar oportunidades de optimización.

---

## 6 Concentración Geográfica

Principales países por ingresos:

1. Reino Unido – 6.7M (~81% del total)
2. Países Bajos – 284K
3. Irlanda (EIRE) – 250K

El negocio presenta alta dependencia del mercado doméstico, con actividad internacional secundaria pero consistente.

---

# >>v Futuros Pasos

Para evolucionar el proyecto hacia un flujo completo de Data Science, se proponen las siguientes extensiones:

## 1 Segmentación de Clientes (RFM)

- Análisis de Recency, Frequency, Monetary
- Clustering (K-Means)
- Identificación de clientes de alto valor
- Perfilamiento conductual

**Impacto:** Optimización de estrategias de marketing y retención.

---

## 2 Modelo de Predicción de Churn

- Definición operativa de churn
- Ingeniería de variables a nivel cliente
- Modelos supervisados (Logistic Regression, Random Forest)
- Evaluación con ROC-AUC / F1-score

**Impacto:** Retención proactiva y reducción de pérdida de clientes.

---

## 3 Forecasting de Ingresos

- Agregación mensual
- Descomposición estacional
- Modelos SARIMA o Prophet

**Impacto:** Planeación de inventario y optimización de demanda.

---

## 4 Customer Lifetime Value (CLV)

- Estimación de valor futuro por cliente
- Modelos de regresión

**Impacto:** Mejor asignación de presupuesto de marketing.

---

## 5 Detección de Anomalías

- Isolation Forest
- Identificación de outliers en transacciones

**Impacto:** Mejora de calidad de datos y detección de fraudes.

---

# Evaluación Final

El dataset ofrece una base sólida para:

- Análisis descriptivo orientado a negocio
- Modelado de comportamiento de clientes
- Forecasting con estacionalidad
- Desarrollo de pipelines de Machine Learning

La siguiente fase del proyecto estará enfocada en transformar los insights descriptivos en modelos predictivos accionables.
