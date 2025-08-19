# 📊 Análisis de Evasión de Clientes (Churn) en Telecom X

## 🎯 Propósito del Proyecto
Este proyecto tiene como objetivo principal analizar los factores que influyen en la **evasión de clientes** (Churn) de la empresa de telecomunicaciones Telecom X. A través de un proceso de análisis de datos, se busca identificar patrones y comportamientos de los clientes que cancelan su servicio, con el fin de proporcionar insights estratégicos al equipo de Data Science para que puedan desarrollar modelos predictivos y acciones de retención.

---

## 📁 Estructura del Proyecto
El proyecto está organizado de la siguiente manera:

* `TelecomX_LATAM.ipynb`: El notebook principal que contiene todo el código del proyecto, desde la extracción de datos hasta el análisis y la generación de gráficos.
* `README.md`: Este archivo, que proporciona una visión general del proyecto.

---

## 📈 Gráficos e Insights Clave
El análisis exploratorio de datos (EDA) reveló varios patrones importantes:

### **1. Distribución de Evasión**
La tasa de Churn es de aproximadamente el **26.5%**, lo que indica que más de una cuarta parte de los clientes ha cancelado el servicio.

<img width="549" height="393" alt="image" src="https://github.com/user-attachments/assets/43ee1ff9-0f7b-445b-ac68-3a59084aee6f" />


### **2. Evasión por Tipo de Contrato**
Los clientes con contratos **mes a mes** (`Month-to-month`) muestran una tasa de evasión considerablemente más alta que aquellos con contratos de uno o dos años, lo que sugiere una menor lealtad.

<img width="859" height="548" alt="image" src="https://github.com/user-attachments/assets/2c580df5-9ebc-4288-b47c-525d2f873fba" />


### **3. Evasión por Método de Pago**
El método de pago es un factor clave. Los clientes que utilizan el **cheque electrónico** tienen la mayor tasa de Churn. Esto podría estar relacionado con la experiencia de usuario o la facilidad de cancelación.

<img width="1014" height="671" alt="image" src="https://github.com/user-attachments/assets/2feaaf19-c86e-42aa-b17f-c819ea4efc03" />


### **4. Relación entre `Tenure`, `Monthly Charges` y Evasión**
* **Tiempo de Contrato (`Tenure`)**: Los clientes que evaden tienen un tiempo de contrato significativamente más bajo. La mayoría de las cancelaciones ocurren en los primeros meses.

<img width="686" height="547" alt="image" src="https://github.com/user-attachments/assets/0fa469e0-01ad-4076-a64e-7dd0f208d3d0" />

  
* **Cargos Mensuales (`Charges.Monthly`)**: Los clientes con cargos mensuales más altos son más propensos a evadir, lo que podría indicar que no perciben un valor adecuado por el precio que pagan.
<img width="695" height="548" alt="image" src="https://github.com/user-attachments/assets/cc6646be-cddb-4c9f-a0c3-79de8d5c2a0e" />


---

## 🚀 Cómo Ejecutar el Notebook
Para ejecutar el análisis completo, sigue estos pasos:

1.  Abre el archivo `TelecomX_LATAM.ipynb` en un entorno como **Google Colab**, **Jupyter Notebook** o **JupyterLab**.
2.  Asegúrate de tener las librerías necesarias instaladas:
    ```bash
    pip install pandas requests matplotlib seaborn
    ```
3.  Ejecuta cada celda del notebook secuencialmente. El notebook está diseñado para seguir el flujo de trabajo de ETL:
    * **Extracción**: La primera sección cargará los datos directamente desde la API.
    * **Transformación**: La siguiente sección limpiará y preparará los datos para el análisis.
    * **Análisis y Visualización**: Las últimas secciones generarán los gráficos y el análisis exploratorio.
4.  Al final del notebook, encontrarás el informe final con la recomendación y su justificación.

¡Listo! Con estos pasos, podrás replicar el análisis y obtener los mismos resultados.

---

**Desarrollado por**: TheDanilore

**Tecnologías Utilizadas**:
* Python
* Pandas (para manipulación de datos)
* Matplotlib (para visualización de datos)
* seaborn
* Google Colab
