# Análisis de Datos - Online Retail (2010–2011)

## Descripción del Proyecto

Este proyecto analiza datos transaccionales de retail online con el objetivo de identificar patrones de ingresos, comportamiento de clientes, concentración geográfica y oportunidades de modelado predictivo.

El enfoque combina limpieza de datos, análisis exploratorio e ingeniería de variables con orientación a decisiones de negocio.

- **Fuente:** [UCI Machine Learning Repository - Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)

---

## Principales Hallazgos

- ~8.28M en ingresos totales
- 81% de los ingresos concentrados en Reino Unido
- 44% más ingresos en el segundo semestre
- 78% de las transacciones con ticket bajo (<20)
- 2.2% tasa de devoluciones

El negocio presenta un modelo de alto volumen y bajo ticket promedio, con marcada estacionalidad.

---

## Metodología

### 1 Limpieza de Datos
- Eliminación de duplicados
- Filtrado de registros sin CustomerID
- Creación de variable de ingresos (Quantity × UnitPrice)

### 2 Ingeniería de Variables
- Extracción de año, mes y semestre
- Segmentación por ticket de compra
- Agregaciones temporales y geográficas

### 3 Análisis Exploratorio
- Evolución de ingresos
- Distribución por país
- Tasa de devoluciones
- Segmentación por monto de transacción

---

## Tecnologías Utilizadas

- **Python 3.10+**
- **Pandas** 
- **Matplotlib** 
- **NumPy**
- **scikit-learn** (para futuras extensiones de ML)
- **Análisis temporal**
- **Feature engineering**

---

## 📂 Estructura del Proyecto
data/
notebooks/
graphs/
requirements.txt
README.md
conclusions.md

---


---

## 🚀 Próximos Desarrollos

- Segmentación RFM + Clustering
- Modelo de predicción de churn
- Forecasting con estacionalidad
- Estimación de CLV
- Detección de anomalías

---

## Competencias Demostradas

- Pensamiento analítico orientado a negocio
- EDA estructurado
- Transformación de datos transaccionales
- Interpretación estratégica de resultados
- Base sólida para modelado predictivo

---

## 👩‍💻 Autora

Damaris A. Zavala  
Data Scientist / Data Analyst
Enfoque en análisis de datos, modelado predictivo y toma de decisiones basada en evidencia.

---

## Instalación y uso

### Clonar el repositorio:
```bash
git clone https://github.com/tu-usuario/online-retail1.git
cd online-retail1
pip install -r requirements.txt

Crear un venv y:
Después de instalar todo con pip install -r requirements.txt, registra el kernel del entorno con:
python -m ipykernel install --user --name=dataScience --display-name "Python (dataScience)"

... si no se deja: 
Forzar la instalación (solo si sabes lo que haces) en un venv

Puedes decirle a pip que ignore el bloqueo del sistema:
pip install -r requirements.txt --break-system-packages
