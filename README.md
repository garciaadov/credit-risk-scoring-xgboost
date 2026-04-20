# credit-risk-scoring-xgboost
# 🏦 Sistema de Scoring para Riesgo de Préstamos (Iniciativa Educativa)
## 🎯 Predicción de Impagos con Machine Learning y Auditoría de Decisiones mediante SHAP

Este repositorio ha sido desarrollado con una **finalidad exclusivamente educativa**. 
Se trata de un modelo de **Machine Learning (ML)** diseñado para ayudar a las entidades bancarias a predecir qué personas tienen la capacidad financiera para pagar un crédito y quiénes presentan un alto riesgo de impago. Es una herramienta de apoyo para determinar la viabilidad de un préstamo basada en datos históricos.

---

## 📊 Origen de los Datos
Para este proyecto se ha utilizado un **Dataset Público descargado de Kaggle** (*Credit Risk Dataset*), que contiene información sobre perfiles financieros y el resultado final de sus créditos.

---

## 🤖 Modelos de IA Evaluados
Se han probado tres modelos distintos de Inteligencia Artificial para comparar su eficacia:

1.  **Regresión Logística:** El modelo base por su simplicidad y claridad estadística.
2.  **Random Forest:** Un modelo de árboles que captura relaciones más complejas.
3.  **XGBoost (Modelo Final):** El ganador por su gran capacidad para detectar correctamente a los clientes que no pueden pagar (Recall del 71%).

---

## 🔍 Explicabilidad con SHAP (IA Transparente)
Para que se entienda cómo analiza la IA cada caso, hemos utilizado la lógica de **SHAP**. Con todos los datos reunidos, hemos identificado los factores que determinan si una persona es de confianza para el banco:

* **Salario (`person_income`):** Es fundamental, pero el modelo analiza cómo se relaciona con el préstamo.
* **Peligro Bancario (`loan_grade`):** La columna más importante para entender el nivel de riesgo asignado.
* **Porcentaje de Deuda (`loan_percent_income`):** Si el préstamo es muy grande respecto al sueldo, el peligro de impago sube.
* **Vivienda (`person_home_ownership`):** Tener casa propia es un factor clave que aumenta la confianza en el cliente.

---

## 🛠️ Cómo Utilizar este Proyecto
1. **Instalar dependencias:** `pip install -r requirements.txt`
2. **Explorar el Notebook:** `TFM_Scoring_Prestamos.ipynb` contiene todo el proceso.
3. **Archivos Listos:** Se incluyen los archivos `.pkl` del modelo y el escalador.

---

**Plataforma:** Kaggle (Data Source) / GitHub (Repository)

---
---

# 🏦 Loan Risk Scoring System (Educational Initiative)
## 🎯 Default Prediction with Machine Learning and Decision Auditing via SHAP

This repository has been developed with an **exclusively educational purpose**. It is a **Machine Learning (ML)** model designed to assist banking institutions in predicting which individuals have the financial capacity to repay a loan and which ones present a high risk of default. It serves as a support tool to determine loan viability based on historical data.

---

## 📊 Data Source
A **Public Dataset downloaded from Kaggle** (*Credit Risk Dataset*) was used for this project, containing information on financial profiles and their loan outcomes.

---

## 🤖 AI Models Evaluated
Three different Artificial Intelligence models were tested to compare their effectiveness:

1.  **Logistic Regression:** The baseline model for its simplicity and statistical clarity.
2.  **Random Forest:** A tree-based model that captures more complex relationships.
3.  **XGBoost (Final Model):** The winner due to its high ability to correctly identify customers who cannot pay (71% Recall).

---

## 🔍 Explainability with SHAP (Transparent AI)
To understand how the AI analyzes each case, we used **SHAP** logic. With all the gathered data, we identified the key factors that determine if a person is "trustworthy" for the bank:

* **Salary (`person_income`):** It is fundamental, but the model analyzes its relationship with the loan.
* **Bank Risk Grade (`loan_grade`):** The most important column for understanding the assigned risk level.
* **Debt Percentage (`loan_percent_income`):** If the loan is too large relative to the salary, the danger of default increases.
* **Home Ownership (`person_home_ownership`):** Owning a home is a key factor that increases trust in the client.

---

## 🛠️ How to Use This Project
1. **Install dependencies:** `pip install -r requirements.txt`
2. **Explore the Notebook:** `TFM_Scoring_Prestamos.ipynb` contains the entire process.
3. **Ready Files:** Includes `.pkl` files for the model and the data scaler.

---

**Platform:** Kaggle (Data Source) / GitHub (Repository)
