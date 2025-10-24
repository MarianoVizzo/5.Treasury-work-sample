<div id="header" align="center">
  <img src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExbmJhbGZlM3AxODVmeDJwejN0bXljdzVlNzI2eDFlN2pvbnIwcjdxaCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/AuG7qwUzshT7lXy7FB/giphy.gif" width="200"/>
  <h1 align="center">Treasury Data & Analytics – Work Sample</h1>
</div>

---

## 💼 Descripción general

Este proyecto presenta un caso práctico de **análisis de datos financieros aplicados a Tesorería**, abarcando el proceso completo de **preparación, análisis y visualización de información transaccional bancaria**.  
El objetivo es demostrar la capacidad de generar reportes consolidados y visualizaciones ejecutivas que faciliten la toma de decisiones financieras.

---

## ⚙️ Estructura del proceso

### **1. Limpieza y preparación de datos**

- Renombrado de columnas para asegurar consistencia y formato uniforme.  
- Estandarización de nombres de bancos, eliminando textos redundantes y normalizando variantes.  
- Validación de tipos de datos y eliminación de registros incompletos o inconsistentes.  

> 🧩 Resultado: dataset limpio y normalizado en formato `.parquet`.

---

### **2. Transformaciones de fechas**

- Conversión de las fechas al tipo `datetime`.  
- Creación de columnas adicionales que identifican:
  - Mes de la transacción.  
  - Día de la semana.  
  - Trimestre correspondiente.  

> 🔍 Estas transformaciones permiten agrupar y comparar resultados por períodos financieros homogéneos.

---

### **3. Clasificación de datos**

- Creación de una nueva columna que clasifica las cuentas según su tipo:
  - `Ahorro`  
  - `Corriente`  
  - `Otro` (si no aplica)  

> 📘 Esta clasificación mejora la lectura de reportes y la segmentación de movimientos.

---

### **4. Análisis de datos**

- **Detección de movimientos inusuales (outliers):** identificación de valores atípicos mediante análisis de dispersión.  
- **Generación de reportes trimestrales:**  
  - Saldos netos por trimestre y moneda.  
  - Variaciones porcentuales respecto a períodos anteriores.  
  - Acumulados trimestrales por banco y tipo de cuenta.

> 📊 Script: `src/analytics.py`  
> 📁 Salida: reportes CSV en `reports/`

---

### **5. Visualización de datos**

Creación de gráficos ejecutivos para una lectura rápida de tendencias y anomalías:

- **Evolución mensual de saldos netos por moneda** (líneas comparativas).  
- **Distribución de montos con outliers destacados** (boxplots o violines).  

> 🎨 Script: `src/visuals.py`  
> 📁 Salida: figuras PNG en `figures/`  
> 📈 Librerías utilizadas: `matplotlib`, `plotly`

---

## 🧠 Tecnologías y librerías

| Categoría | Herramientas |
|------------|---------------|
| Lenguaje principal | Python 3.10+ |
| Procesamiento de datos | Pandas, NumPy |
| Visualización | Matplotlib, Plotly |
| Análisis | Scipy, funciones personalizadas |
| Control de versiones | Git / GitHub |

---

## 🚀 Ejecución del flujo

1️⃣ Colocar el archivo `worksample.csv` dentro de la carpeta `data/`.  
2️⃣ Instalar las dependencias:
```bash
pip install -r requirements.txt
