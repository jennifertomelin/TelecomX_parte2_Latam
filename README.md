# Telecom X – Predicción de Cancelación de Clientes (Churn)

## Descripción del proyecto
Este proyecto tiene como objetivo desarrollar modelos de **Machine Learning** capaces de predecir la cancelación de clientes (churn) en Telecom X. A partir de un conjunto de datos previamente limpiado y preparado, se realizó un proceso de análisis, preprocesamiento y modelado para identificar los factores que influyen en la pérdida de clientes y apoyar la toma de decisiones estratégicas.

## Objetivos
- Preparar los datos para el modelado predictivo.
- Analizar la relación entre variables y la cancelación de clientes.
- Construir y evaluar modelos de clasificación.
- Identificar las variables más relevantes en la predicción del churn.
- Proponer estrategias de retención basadas en los resultados obtenidos.

## Tecnologías utilizadas
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Imbalanced-learn  
- Google Colab / Jupyter Notebook  

## Proceso del proyecto

### 1. Preparación de datos
Se utilizó el dataset limpio generado en la primera parte del desafío.  
Las etapas incluyeron:
- Eliminación de variables irrelevantes (como identificadores).
- Codificación de variables categóricas mediante **One-Hot Encoding**.
- Análisis de correlación entre variables.
- Balanceo de clases para manejar el desbalance en la variable objetivo.

### 2. Análisis exploratorio
Se analizaron relaciones entre variables clave y la cancelación de clientes, como:
- **Tiempo de permanencia (tenure)**
- **Cargos mensuales**
- **Cargos totales**
- **Tipo de contrato**

Se utilizaron visualizaciones como **boxplots, scatter plots y matrices de correlación** para identificar patrones relevantes.

### 3. Modelos predictivos
Se implementaron dos modelos de clasificación:

**Regresión Logística**
- Requiere normalización de datos.
- Permite interpretar la contribución de cada variable mediante coeficientes.

**Random Forest**
- Modelo basado en árboles.
- No requiere normalización.
- Permite calcular la importancia de variables.

### 4. Evaluación de modelos
Los modelos se evaluaron mediante las siguientes métricas:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Matriz de confusión  

El modelo **Random Forest** mostró un mejor desempeño general al capturar relaciones más complejas entre las variables.

## Factores que influyen en la cancelación
El análisis identificó que las variables más relevantes para predecir la cancelación incluyen:

- **Tipo de contrato**
- **Tiempo de permanencia del cliente (tenure)**
- **Cargos mensuales**
- **Cargos totales**
- **Método de pago**
- **Tipo de servicio de internet**

Los clientes con **contratos mensuales, menor antigüedad y cargos mensuales elevados** presentan mayor probabilidad de cancelar el servicio.

## Estrategias de retención propuestas
A partir de los resultados obtenidos se proponen las siguientes acciones:

- Incentivar **contratos de mayor duración** mediante beneficios o descuentos.
- Implementar estrategias de **retención temprana para clientes nuevos**.
- Revisar la **estructura de precios de planes con cargos elevados**.
- Fortalecer programas de **fidelización y soporte al cliente**.

## Conclusión
El uso de modelos de Machine Learning permitió identificar patrones clave asociados a la cancelación de clientes. Estos resultados pueden ayudar a Telecom X a anticipar el churn y diseñar estrategias de retención más efectivas, mejorando la estabilidad y la rentabilidad del negocio.
