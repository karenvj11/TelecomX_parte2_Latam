# 📊 TelecomX – Análisis y Predicción de la Rotación de Clientes

## 📌 Acerca del Proyecto

Este proyecto busca analizar el comportamiento de los clientes de TelecomX y desarrollar modelos de aprendizaje automático capaces de predecir la rotación de clientes.

La rotación de clientes representa a los clientes que han cancelado sus servicios, lo que impacta directamente en los ingresos de la compañía. Mediante análisis exploratorio y modelos predictivos, buscamos identificar los principales factores que influyen en la rotación y proponer soluciones estratégicas.

---

##  Objetivos

- Realizar análisis exploratorio de datos
- Comprender los patrones de abandono
- Preparar los datos para el modelado
- Entrenar y comparar diferentes modelos de clasificación
- Evaluar el rendimiento e identificar el sobreajuste/subajuste
- Analizar la importancia de las variables
- Generar información estratégica para la retención de clientes

---

##  Estructura del proyecto

El cuaderno se organiza en los siguientes pasos:

### 1. Importación de bibliotecas
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-Learn

---

### 2. Recopilación y comprensión de datos

- Cargar el conjunto de datos (`data_procesada.csv`)

- Análisis de:

- Estructura (`.info()`)

- Dimensiones (`.shape`)

- Columnas disponibles

- Variable Tipos

---

### 3. Preprocesamiento de datos

#### Eliminación de columnas irrelevantes
- Exclusión de `CustomerID`, ya que no aporta valor predictivo.

#### Agrupación por categorías
- Estandarización de categorías como `"No"` y `"Sin servicio"`.

#### Comprobación de valores nulos
- Verificación de la integridad del conjunto de datos.

--

## Análisis exploratorio de datos (EDA)

Se realizaron análisis para comprender:

- Correlación entre variables numéricas
- Tasa de abandono por categoría
- Distribución de la variable objetivo (Churn)
- Relación entre el tipo de contrato y el abandono
- Impacto de los servicios adicionales en la retención

### Conclusiones clave observadas:

- Los clientes con contratos mensuales tienen una mayor tasa de abandono.

- Los clientes con contratos más cortos tienden a cancelar con más frecuencia.

- Los métodos de pago automáticos reducen la pérdida de clientes.

- Los servicios adicionales (como la seguridad en línea y el soporte técnico) influyen en la retención.

---

##  Preparación para el Modelado

### Separación de Variables

- Variables Explicativas (X)
- Variable Objetivo (y → Perdida de Clientes)

### Codificación

- Transformación de variables categóricas
- Conversión a formato numérico

### División de Datos

- Entrenamiento
- Pruebas

### Normalización

- Aplicada a modelos sensibles a la escala (p. ej., KNN y Regresión Logística)

---

# Modelos Implementados

Se probaron diferentes algoritmos de clasificación:

## Modelo Base (Dummy)
Utilizado como punto de referencia inicial.

---

## Árbol de decisión

**Ventajas:**

- Fácil interpretación
- Identificación clara de reglas

**Limitaciones:**
- Tendencia al sobreajuste

---

## Bosque aleatorio

**Ventajas:**

- Mejor generalización
- Reducción del sobreajuste
- Mejor rendimiento general

---

## K-vecinos más cercanos (KNN)

**Ventajas:**

- Implementación sencilla

**Limitaciones:**

- Sensibilidad a la escala
- Puede presentar alta dimensionalidad

---

## Regresión logística

**Ventajas:**

- Interpretable
- Buen rendimiento en problemas lineales
- Permite analizar la importancia de las variables

---

#  Evaluación del modelo

Métricas como:

- Exactitud
- Precisión
- Recordatorio
- Puntuación F1

- Comparación entre entrenamiento y pruebas
- Identificación de sobreajuste o infraajuste

---

#  Mejor Modelo

El modelo **Random Forest** mostró el mejor equilibrio entre:

- Rendimiento
- Generalización
- Robustez

Demostró un menor sobreajuste y una mejor capacidad predictiva en comparación con los otros modelos.

---

# Análisis de la Importancia de las Variables

El análisis mostró que las variables más relevantes para predecir la pérdida de clientes están relacionadas con:

- Tipo de contrato
- Duración de la estancia
- Importe mensual
- Método de pago
- Servicios adicionales contratados

Esto proporciona una dirección estratégica para las acciones de retención.

---

# Perspectivas estratégicas para el negocio

Basado en el análisis:

1. Fomentar contratos anuales o bienales
2. Crear estrategias de retención en los primeros meses
3. Ofrecer beneficios a los clientes con pagos automáticos
4. Ofrecer paquetes con servicios adicionales
5. Monitorear a los clientes con periodos de retención cortos

---

# Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-Learn

---
