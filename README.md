# 🧠 Predictors of Academic Stress: A Parsimonious Approach

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Methodology](https://img.shields.io/badge/Method-Ridge%20Regression-lightgrey)
![Status](https://img.shields.io/badge/Status-Research%20Complete-green)

Un análisis de ciencia de datos "end-to-end" que desafía la complejidad en la psicometría educativa. Este proyecto investiga los factores determinantes del estrés en estudiantes universitarios, comparando la eficacia de modelos saturados frente a modelos reducidos.

---

## 🎯 Objetivo del Proyecto

Determinar si es posible predecir el nivel de estrés académico con alta precisión utilizando un número mínimo de variables, aplicando el principio de parsimonia (Navaja de Ockham) para crear herramientas de detección más eficientes y menos intrusivas.

## 🔍 Hallazgos Clave

A través de un diseño experimental comparativo, se descubrió que:

* **La complejidad tiene rendimientos decrecientes:** Un modelo de Regresión Lineal Múltiple (MLR) con **20 variables** alcanzó un $R^2$ de **0.89**.
* **La simplicidad es robusta:** Un modelo reducido utilizando solo **4 variables clave** alcanzó un $R^2$ de **0.88**.
* **Las 4 Variables Críticas:** 1. Autoestima (Factor protector).
    2. Calidad del Sueño (Factor fisiológico).
    3. Nivel de Ansiedad (Factor emocional).
    4. Preocupación por el Futuro Profesional (Factor contextual).

## 🛠️ Metodología Técnica

El flujo de trabajo incluyó:

1.  **Análisis Exploratorio (EDA):** Detección de multicolinealidad y relaciones lineales.
2.  **Preprocesamiento:** Estandarización (StandardScaler) y limpieza de datos.
3.  **Modelado Comparativo:**
    * *Línea Base:* Regresión Lineal Simple (SLR).
    * *Techo:* Regresión Lineal Múltiple (Full MLR).
    * *Propuesta:* **Ridge Regression (L2)** para manejar la multicolinealidad entre variables psicológicas.
4.  **Validación:**
    * Optimización de hiperparámetros ($\alpha$) mediante **GridSearch**.
    * Validación Cruzada (**K-Fold Cross-Validation**).
    * Diagnóstico de residuos con **QQ-Plots** para verificar supuestos de normalidad.

---

## 📄 Paper de Investigación Generado con IA

Como parte de este experimento, se utilizó **Gemini Deep Research** para sintetizar los hallazgos del código y contrastarlos con literatura científica actual, generando un White Paper académico completo.

📥 **[Leer el Paper (PDF)](paper_estres_academico.pdf)** *(Asegúrate de subir el PDF al repo y ajustar este nombre si cambia)*

---

## 💻 Estructura del Repositorio

```text
├── Stress_Predictive_Models.ipynb   # Notebook principal con todo el código y análisis
├── paper_estres_academico.pdf       # Reporte de investigación generado
├── data/                            # (Opcional) Carpeta con el dataset si la licencia lo permite
└── README.md                        # Documentación del proyecto
