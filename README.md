<div id="header" align="center">
  <img src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExbmJhbGZlM3AxODVmeDJwejN0bXljdzVlNzI2eDFlN2pvbnIwcjdxaCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/AuG7qwUzshT7lXy7FB/giphy.gif" width="400"/>
  <h1 align="center">Treasury Data & Analytics – Work Sample</h1>
</div>

---

## 💼 Descripción general

Este proyecto presenta un caso práctico de **análisis de datos financieros aplicados a Tesorería**, abarcando el proceso completo de **preparación, análisis y visualización de información transaccional bancaria**.  
El objetivo es demostrar la capacidad de generar reportes consolidados y visualizaciones ejecutivas en **Python** que faciliten la toma de decisiones financieras.

---

## ⚙️ Estructura del proceso

### **1. Limpieza y preparación de datos**

- Renombrado de columnas para asegurar consistencia y formato uniforme.  
- Estandarización de nombres de bancos, eliminando textos redundantes y normalizando variantes.  
- Validación de tipos de datos y eliminación de registros incompletos o inconsistentes.  

---

### **2. Transformaciones de fechas**

- Conversión de las fechas al tipo `datetime`.  
- Creación de columnas adicionales que identifican:
  - Mes de la transacción.  
  - Día de la semana.  
  - Trimestre correspondiente.  

---

### **3. Clasificación de datos**

- Creación de una nueva columna que clasifica las cuentas según su tipo:
  - **Ahorro**
  - **Corriente**  

---

### **4. Análisis de datos**

- **Detección de movimientos inusuales (outliers):** identificación de valores atípicos mediante análisis de dispersión.  
- **Generación de reportes trimestrales:**  
  - Saldos netos por trimestre y moneda.
  <img width="1486" height="552" alt="image" src="https://github.com/user-attachments/assets/ef0cbf79-31f4-47ae-8d05-21faedee0f3c" />
  <img width="1450" height="492" alt="image" src="https://github.com/user-attachments/assets/025bf2e4-0c8f-4115-8263-f8d161b438f2" />


  - Variaciones porcentuales respecto a períodos anteriores.
  <img width="1465" height="640" alt="image" src="https://github.com/user-attachments/assets/afe5c9dd-2133-461b-8376-5b80be6041bb" />
 
  - Acumulados trimestrales por banco y tipo de cuenta.

---

### **5. Visualización de datos**

Creación de gráficos ejecutivos para una lectura rápida de tendencias y anomalías:

- **Evolución mensual de saldos netos por moneda** (líneas comparativas).  
- **Distribución de montos con outliers destacados** (boxplots o violines).  

---

## 🧰 Tecnologías y librerías

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
