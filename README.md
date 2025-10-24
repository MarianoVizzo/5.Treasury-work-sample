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

En el gráfico de barras se visualizan los saldos netos trimestrales por moneda (ARS, EUR y USD) junto con la variación porcentual respecto al trimestre anterior. Como ejemplo se explica el Trimestre 1 al Trimestre 2:

ARS: el saldo pasó de 656k a 810k, lo que representa un crecimiento del +23.4%. Esto indica una mejora significativa en los flujos netos en pesos durante el segundo trimestre.

EUR: el saldo bajó de 789k a 751k, con una variación negativa del -4.8%

USD: el saldo creció de 767k a 797k, con un aumento del +4.0%, mostrando una mejora moderada en dólares.

Como análisis general (Trimestres 1 a 4) se puede visualizar:
ARS (Pesos argentinos):

Muestra una tendencia ascendente sostenida a lo largo del año, pasando de 656k a 851k. Aunque el crecimiento se modera en el tercer y cuarto trimestre, siempre mantiene una variación positiva, lo que refleja una buena performance en saldos netos en pesos.
EUR (Euros):

Presenta una caída moderada en el segundo y tercer trimestre, tocando un piso en 750k.

En el cuarto trimestre se recupera parcialmente, subiendo a 774k (+3.2%), aunque sin superar el valor del primer trimestre.

USD (Dólares estadounidenses):

Experimenta una leve caída en el tercer trimestre (-9.6%), pero se recupera fuertemente en el cuarto, con un salto del +15.1% que lo ubica en 830k, el valor más alto del año para esta moneda.

  - Variaciones porcentuales respecto a períodos anteriores.
  <img width="1465" height="640" alt="image" src="https://github.com/user-attachments/assets/afe5c9dd-2133-461b-8376-5b80be6041bb" />
 
  - Acumulados trimestrales por banco y tipo de cuenta.
  <img width="1486" height="552" alt="image" src="https://github.com/user-attachments/assets/ef0cbf79-31f4-47ae-8d05-21faedee0f3c" />
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
