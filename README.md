# ⚽ Fantasy Football Analytics Dashboard

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-App-ff4b4b)
![Data Science](https://img.shields.io/badge/Data%20Science-PCA%20%26%20Clustering-green)

## 📊 Executive Summary

This repository hosts an interactive **Decision Support System (DSS)** designed for Fantasy Football (Serie A) players. Built with **Python** and **Streamlit**, the application transforms raw match data into actionable insights, helping users optimize their roster strategy through statistical analysis and visualization.

Beyond simple descriptive statistics, the project leverages data science techniques (**Dimensionality Reduction**, **Unsupervised Clustering**) to identify undervalued players and analyze performance clusters using the `scikit-learn` library.

---

## 🖼️ Application Preview
![Dashboard Screenshot](https://github.com/user-attachments/assets/2f6fa192-88a5-4167-9666-1b4a48ce4989)

### 🔗 [STREAMLIT WEB APP](https://vincilfanta2526-matteoientile.streamlit.app/) 

---

## 🛠️ Key Features

The application is structured into modular analysis pages:

### 1. Role-Specific Analysis
* **Goalkeepers (`1_Statistiche_PORTIERI`):** Analysis of Goals Conceded vs. Expected Goals (xG) to evaluate true shot-stopping performance.
* **Defenders & Midfielders (`2_DIF`, `3_CEN`):** Advanced filtering by Fantasy Average (FantaMedia), Games Played, and Consistency metrics.
* **Strikers (`4_Statistiche_ATTACCANTI`):** * **Violin Plots & Box Plots** to visualize the variance and consistency of player scores.
    * **Scatter Plots** for cross-metric analysis (e.g., Price vs. Performance).

### 2. Advanced Metrics & Machine Learning
* **Player Similarity Search:** Implementation of **K-Means Clustering** to group players with similar output profiles (e.g., "Playmakers", "Target Men", "Inefficient Volume Shooters").
* **Dimensionality Reduction:** Application of **PCA (Principal Component Analysis)** to synthesize multi-dimensional performance metrics into interpretable indices, reducing noise in player evaluation.

### 3. Roster Management (`5_Listone&Formazioni`)
* Interactive tables to manage the full player database.
* Tools for auction simulation and budget allocation optimization.

---

## 💻 Tech Stack

* **Core:** Python 3.x
* **Web Framework:** [Streamlit](https://streamlit.io/)
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn, Plotly (for interactive charts)
* **Machine Learning:** Scikit-learn (StandardScaler, PCA, KMeans)

---
## 🚀 Getting Started

### Prerequisites
Ensure you have Python installed.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/matteoientile/Fantasy25_26.git](https://github.com/matteoientile/Fantasy25_26.git)
    cd Fantasy25_26
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the App:**
    ```bash
    streamlit run Fanta2526_Homepage.py
    ```

---

## 🔮 Future Developments

* **Predictive Modeling:** Integrating a Time Series model (ARIMA/LSTM) to predict player form for the next 3 matchdays.
* **Optimization Engine:** Adding a Linear Programming solver (PuLP) to suggest the mathematically optimal lineup based on budget constraints.

## 👤 Author

**Matteo Ientile**
* M.Sc. Student in Mathematical Engineering @ Politecnico di Torino
* [LinkedIn](https://www.linkedin.com/in/matteo-ientile/)

## 📂 Project Structure

```text
├── Fanta2526_Homepage.py        # Application Entry Point & Landing Page
├── pages/
│   ├── 1_Statistiche_PORTIERI.py       # GK Analysis Module
│   ├── 2_Statistiche_DIFENSORI.py      # Defenders Analysis Module
│   ├── 3_Statistiche_CENTROCAMPISTI.py # Midfielders Analysis Module
│   ├── 4_Statistiche_ATTACCANTI.py     # Strikers Analysis & ML Module
│   └── 5_Listone&Formazioni.py         # Database & Lineup Tools
├── data/                        # Dataset storage (Excel/CSV)
├── requirements.txt             # Dependencies
└── README.md                    # Documentation




