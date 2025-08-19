# Project Analytics: Synthetic Project Data Analysis

## Overview

This repository contains a fully reproducible data‑analysis project built around a synthetic project‑management dataset. The goal is to showcase data exploration, visualization and predictive modelling skills relevant to roles such as **business analyst**, **program manager** and **data analyst**. The project includes an easy‑to‑use dataset, a Jupyter notebook for exploratory data analysis (EDA) and model building, and a clear set of instructions so anyone can get up and running quickly.

The synthetic dataset simulates common project characteristics—such as duration, team size, budget, complexity and risk—and pairs them with a corresponding client‑satisfaction outcome. By analysing this data you can practise deriving insights, drawing conclusions and building models that predict client satisfaction levels.

## Dataset

The dataset is provided in `data/synthetic_project_data.csv`. Each row represents a single project and includes the following columns:

| Column                    | Description                                                                                 |
|---------------------------|---------------------------------------------------------------------------------------------|
| `project_id`              | Unique identifier for each synthetic project                                                |
| `project_length_days`     | Duration of the project in days                                                             |
| `team_size`               | Number of team members assigned to the project                                              |
| `budget`                  | Budget allocated to the project (USD)                                                       |
| `complexity_score`        | A rating (1–10) reflecting the complexity of the project                                    |
| `resources_score`         | A rating (1–10) representing the sufficiency of project resources                           |
| `on_time_delivery`        | Indicator (1 = delivered on time, 0 = not delivered on time)                                |
| `risk_score`              | A rating (1–10) capturing the project’s risk level                                          |
| `client_satisfaction_score` | Continuous score (0–100) measuring client satisfaction                                     |
| `client_satisfaction_label` | Discrete label derived from the satisfaction score (High, Medium, or Low)                  |

## Usage

Follow these steps to reproduce the analysis:

1. **Clone or download** this repository to your local machine.
2. **Install the required Python dependencies** from `requirements.txt`:

   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Jupyter Notebook** and open the analysis notebook:

   ```bash
   jupyter notebook notebooks/analysis.ipynb
   ```

4. **Run the notebook** cell by cell. It will load the dataset, display summary statistics, visualise feature distributions and correlations, and train a RandomForest classifier to predict client satisfaction labels. You’ll see model performance metrics such as accuracy, a classification report, and a confusion matrix. The notebook also plots feature importances to highlight which project attributes most strongly influence client satisfaction.

## Project Structure

- `data/synthetic_project_data.csv` – synthetic dataset used for the analysis.
- `notebooks/analysis.ipynb` – Jupyter notebook containing EDA, visualisations and predictive modelling.
- `requirements.txt` – Python dependencies required to run the notebook.
- `README.md` – documentation outlining the project, dataset and usage instructions.

## Motivation

Building and sharing small but comprehensive projects is an excellent way to demonstrate your analytical capabilities and your ability to communicate insights. This project combines data generation, exploratory analysis and model development in a single repository that you can show to potential employers or collaborators. Use it as a template for your own analyses—modify the dataset, adjust the models or extend the notebook to answer new questions. Good luck!
