# 📈 Series de Tiempo

Este repositorio tiene como objetivo introducir, desarrollar y aplicar modelos clásicos y modernos de **series de tiempo**, con énfasis tanto en fundamentos estadísticos como en **aplicaciones financieras**.

El contenido está pensado para estudiantes de finanzas, economía, ciencia de datos y perfiles cuantitativos que buscan entender no solo el *cómo*, sino el *por qué* de cada modelo.

---

## 1. Introducción a Series de Tiempo

Una **serie de tiempo** es un conjunto de observaciones ordenadas cronológicamente. A diferencia de datos transversales, el orden temporal es esencial y genera dependencia entre observaciones.

Se abordan conceptos clave como:
- Tendencia
- Estacionalidad
- Ciclos
- Ruido
- Estacionariedad

### 1.1 Ejemplos
- Series macroeconómicas (PIB, inflación)
- Series financieras (precios, rendimientos)
- Series operativas (ventas, demanda)

---

## 2. Modelos ARIMA (p, d, q)

El modelo **ARIMA** combina:
- **AR (p)**: componente autorregresivo  
- **I (d)**: diferenciación para lograr estacionariedad  
- **MA (q)**: promedio móvil  

Se analiza:
- Identificación del modelo
- Estimación de parámetros
- Validación y diagnóstico de residuos

### 2.1 SARIMA (p, d, q)(P, D, Q)<sub>s</sub>

Extensión de ARIMA que incorpora **estacionalidad**, permitiendo modelar patrones repetitivos en el tiempo (mensuales, trimestrales, etc.).

---

### 2.2 Funciones de Autocorrelación

Las funciones de autocorrelación permiten identificar dependencia temporal y son clave para la selección del modelo.

### 2.3 ACF (Autocorrelation Function)

Se utiliza para:
- Detectar correlaciones seriales
- Identificar el orden del componente MA
- Diagnosticar residuos

---

### 2.4 Log-verosimilitud

La **log-verosimilitud** mide qué tan bien el modelo explica los datos observados y es la base para criterios de selección de modelos.

---

### 2.5 Índice de Akaike (AIC)

Criterio de información que penaliza la complejidad del modelo:

- Menor AIC → mejor trade-off entre ajuste y parsimonia

---

### 2.6 Criterio Bayesiano (BIC)

Similar al AIC pero con una penalización más fuerte por el número de parámetros, favoreciendo modelos más simples.

---

## 3. Series de Tiempo Financieras

Las series financieras presentan características particulares:
- Volatilidad cambiante
- Clustering de volatilidad
- Asimetrías
- Colas pesadas

Por ello, se requieren modelos específicos.

---

### 3.1 GARCH

El modelo **GARCH** permite modelar la volatilidad condicional como un proceso dinámico dependiente del pasado.

Aplicaciones:
- Gestión de riesgo
- VaR
- Análisis de mercados financieros

---

### 3.2 EGARCH

Extensión de GARCH que:
- Captura asimetrías
- Modela efectos de apalancamiento
- No requiere restricciones de no-negatividad

---

## 📌 Tecnologías utilizadas
- Python / R  
- NumPy, pandas, statsmodels  
- Visualización de series y diagnósticos  

---

## 🚀 Objetivo del repositorio

Construir una base sólida en series de tiempo y servir como referencia práctica para proyectos académicos y profesionales en finanzas cuantitativas.

---

📬 *Cualquier sugerencia o mejora es bienvenida.*
