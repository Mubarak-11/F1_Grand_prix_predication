# 🏎️ Formula 1 Race Predictions — Spa Grand Prix 2025

A machine learning project that uses real-world Formula 1 data to predict driver rankings for the **Belgian Grand Prix 2025 at Spa-Francorchamps**.  
Built using **LightGBM Rankers**, evaluated with **NDCG@K** and **Hit@K**, and visualized with podium-style and bar plots.

---

## 📌 Project Overview

This project applies machine learning to simulate and predict real-world F1 outcomes. It involves:

- Processing historical race data (2021–2024)
- Feature engineering for qualifying, race performance, and driver metrics
- Building two specialized ranking models:
  - **Model 1:** Predicts Top 3 podium finishers
  - **Model 2:** Predicts Positions 4–10 (midfield)
- Evaluating models using NDCG@K and Hit@K metrics
- Generating predictions for Spa GP 2025 (including visualization)

---

## 🛠️ Tech Stack

- **Python 3.10**
- **LightGBM Ranker**
- **Scikit-learn**, **Pandas**, **Seaborn**, **Matplotlib**
- Evaluation metrics: `ndcg_score`, custom `Hit@K`

---

## 📊 Key Features

### ✔️ Model Training

- **Model 1 (Podium):**  
  Trained only on positions 1–3 using qualifying, constructor, and historical performance features.

- **Model 2 (Midfield):**  
  Focuses on positions 4–10 with different features to better model midfield variability.

### ✔️ Evaluation

- **Model 1 Results (Test set, 2024):**
  - NDCG@3: `0.3080`
  - Hit@3: `41.7%`

- **Model 2 Results (Test set, 2024):**
  - NDCG@7: `0.6651`
  - Hit@7: `100%`

### ✔️ Visual Outputs

- **Feature Importance Plot** for Model 1
- **Podium-style bar chart** showing predicted Top 10 for Spa 2025
- **Clean HTML + CSS** rendering of final driver rankings

---

## 🧠 Prediction: Spa Grand Prix 2025

| Rank | Driver           | Team         |
|------|------------------|--------------|
| 1    | Oscar Piastri    | McLaren      |
| 2    | Charles Leclerc  | Ferrari      |
| 3    | Lando Norris     | McLaren      |
| 4–10 | [See notebook / HTML] |

Only drivers confirmed for the 2025 season are considered in the final Top 10 list.

---

## 📁 Directory Structure


