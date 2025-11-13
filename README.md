# Análisis Exploratorio de Datos (EDA) - Online Retail

Este proyecto presenta un **análisis exploratorio de datos (EDA)** del dataset *Online Retail*, que contiene información de transacciones reales de una tienda online del Reino Unido entre 2010 y 2011.  
El objetivo es **comprender el comportamiento de ventas, identificar productos clave, analizar estacionalidad y devoluciones**, y preparar el terreno para un análisis predictivo posterior.

---

## 1. Objetivos del proyecto

- Explorar la estructura y calidad del dataset.  
- Limpiar los datos eliminando duplicados y valores faltantes.  
- Analizar el volumen de ventas por año, semestre y mes.  
- Identificar los productos más vendidos.  
- Analizar el comportamiento de devoluciones.  
- Segmentar las transacciones según su monto total.  

---

## 2. Dataset

- **Fuente:** [UCI Machine Learning Repository - Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/online+retail)
- **Registros:** ~540,000  
- **Columnas principales:**
  - `InvoiceNo`: número de factura  
  - `StockCode`: código de producto  
  - `Description`: descripción del producto  
  - `Quantity`: cantidad vendida  
  - `InvoiceDate`: fecha de la transacción  
  - `UnitPrice`: precio unitario  
  - `CustomerID`: identificador del cliente  
  - `Country`: país de origen del cliente  

---

## 3. Estructura del proyecto

| Sección | Descripción |
|----------|--------------|
| **1. Carga y exploración** | Lectura del CSV, inspección general, valores nulos y duplicados. |
| **2. Limpieza** | Eliminación de duplicados y nulos, creación de `TotalAmount`. |
| **3. Análisis temporal** | Agrupación de ventas por año, mes y semestre. |
| **4. Devoluciones** | Identificación de transacciones negativas y su proporción. |
| **5. Segmentación por monto** | Clasificación de ventas en Low, Medium, High. |
| **6. Productos más vendidos** | Ranking de productos según cantidad total vendida. |
| **7. Conclusiones** | Hallazgos clave y propuestas de análisis adicional. |

---

## 4. Resultados principales

- El año 2011 concentra la mayor parte de las ventas.  
- Las devoluciones representan una fracción menor pero relevante para control de calidad.  
- Los productos más vendidos pertenecen a categorías de alto movimiento y bajo costo.  
- Se observa estacionalidad con picos de ventas en el segundo semestre de 2012.  

---

## 5. Tecnologías utilizadas

- **Python 3.10+**
- **Jupyter Notebook**
- **Pandas** (análisis de datos)
- **Matplotlib** (visualización)
- **Seaborn** (visualización avanzada)
- **NumPy**
- **scikit-learn** (para futuras extensiones de ML)

---

## 6. Instalación y uso

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
