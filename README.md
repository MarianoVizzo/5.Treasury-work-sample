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
  <img width="1545" height="652" alt="image" src="https://github.com/user-attachments/assets/1141a2b6-efb3-4318-b072-6fea0445162b" />

- **Generación de reportes trimestrales:**  
  - Saldos netos por trimestre y moneda.
  <img width="1591" height="657" alt="image" src="https://github.com/user-attachments/assets/8b2fd9a0-c294-47c1-b753-da6ed62ce395" />

  - Variaciones porcentuales respecto a períodos anteriores.
  <img width="1427" height="482" alt="image" src="https://github.com/user-attachments/assets/528db1c5-8a3e-4069-a93b-23bc9f042148" />

  - Acumulados trimestrales por banco y tipo de cuenta.
     - Ejemplo con el **BANCO BBVA ARGENTINA S.A.**
  <img width="1495" height="447" alt="image" src="https://github.com/user-attachments/assets/b0111e28-ff2e-4a62-adfb-972fc09b7c89" />
  <img width="1493" height="446" alt="image" src="https://github.com/user-attachments/assets/8e84d828-e439-4d80-a7a0-2d45cddb76d9" />


---

### **5. Visualización de datos**

Creación de gráficos ejecutivos para una lectura rápida de tendencias y anomalías:

- **Evolución mensual de saldos netos por moneda** (líneas comparativas).
<img width="1465" height="640" alt="image" src="https://github.com/user-attachments/assets/afe5c9dd-2133-461b-8376-5b80be6041bb" />

- **Distribución de montos con outliers destacados** (boxplots o violines).
<img width="1580" height="711" alt="Captura de pantalla 2025-10-24 130259" src="https://github.com/user-attachments/assets/647968a8-7cd6-4972-849c-e68a8a6ab851" />


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
