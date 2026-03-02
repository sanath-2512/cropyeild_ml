# 🌾 Intelligent Crop Yield Prediction & Farm Advisory

> A comprehensive machine learning toolkit for predicting agricultural productivity using historical crop, soil, and weather data. 

## Table of Contents

- [Overview](#overview)
- [Live Demo](#live-demo)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Methodology](#methodology)
- [Limitations](#limitations)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project serves as **Milestone-1** in developing an AI-driven agricultural analytics system. It focuses exclusively on traditional Machine Learning pipelines to predict crop yields and identify key productivity factors without relying on Large Language Models (LLMs) or Agentic AI. 

By analyzing critical inputs like rainfall, soil type, and fertilizer usage, this classical ML approach provides a robust, interpretable baseline. This foundation motivates the transition toward an autonomous, agent-based farm advisory system in future milestones.

## Live Demo

* **Deployed Web Application:** [Crop Yield Predictor on Render](https://cropyield-pahp.onrender.com/)
* **GitHub Repository:** [sanath-2512/cropyeild_ml](https://github.com/sanath-2512/cropyeild_ml)

## Features

### Core Capabilities

- **Data Processing**: Accepts and processes raw agricultural CSV data (Soil, Weather, Crop).
- **Automated Preprocessing**: Handles missing values, performs feature scaling (Standardization/Normalization), and applies categorical encoding (One-Hot/Label Encoding).
- **Yield Prediction**: Generates numerical or categorical crop yield predictions based on environmental inputs.
- **Feature Importance**: Analyzes and extracts the most significant factors driving crop growth (e.g., pH, Rainfall).
- **Evaluation Metrics**: Calculates and displays Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared ($R^2$) scores.

### Interactive Web Interface

Built with Streamlit/Gradio, the interface provides:
- Simple input forms for farmers or agricultural analysts to enter soil and weather parameters.
- Real-time yield predictions based on the trained models.
- Visual breakdowns of which features impacted the prediction the most.
- Clean, intuitive, and accessible UI design.
  
## 🌟 Project Highlights & Model Performance

This repository houses a robust machine learning pipeline designed to predict agricultural output with high precision. By analyzing critical environmental and chemical factors—such as rainfall, soil type, and fertilizer usage—we established a highly accurate predictive baseline. 

Our classical machine learning models demonstrated exceptional reliability on the test dataset:
* **Linear Regression (Top Performer):** Achieved an outstanding **R² score of 0.9140**, explaining over 91% of the variance in crop yields. It maintained low error rates with a Mean Absolute Error (MAE) of **0.3992** and a Root Mean Squared Error (RMSE) of **0.5009**.
* **Decision Tree Regressor:** Successfully captured complex, non-linear environmental interactions, delivering a strong **R² score of 0.8828** alongside an MAE of **0.4656** and RMSE of **0.5847**. The model exhibited only a slight, acceptable margin of overfitting (0.0597 R² difference from training), proving its robustness in real-world data scenarios.

These metrics validate the system's ability to accurately map soil and weather profiles to crop yields, laying a statistically sound foundation before integrating autonomous, agent-based advisory features in the next milestone.


## Tech Stack

### Core Libraries

- **Python 3.8+**: Primary programming language
- **Streamlit / Gradio**: Web application and UI framework
- **scikit-learn**: Machine learning algorithms and preprocessing utilities
- **pandas**: Data manipulation, cleaning, and CSV parsing
- **numpy**: Numerical computations and matrix operations

### Supporting Libraries

- **matplotlib / seaborn**: Plotting and data visualization (Feature importance charts)
- **joblib / pickle**: Model saving and loading

## Installation

### Prerequisites

- Python 3.8 or higher
- pip package manager
- Git

### Setup Steps

1. **Clone the repository**

```bash
git clone [https://github.com/sanath-2512/cropyeild_ml.git](https://github.com/sanath-2512/cropyeild_ml.git)
cd cropyeild_ml
```

2. **Set up a virtual environment (Recommended):**

```python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

3. **Install dependencies:**

```
pip install -r requirements.txt
```

4. **Run the application locally:**

```
streamlit run app.py
```

The application will automatically open in your web browser at http://localhost:8501


## 📂 Project Structure

<img width="185" height="210" alt="Screenshot 2026-03-02 at 3 51 20 PM" src="https://github.com/user-attachments/assets/01d48778-dbab-4523-b420-74588bf60949" />

## ⚠️ Limitations & Next Steps (Milestone 2)

While highly accurate on historical data, this Milestone 1 implementation has classical ML constraints:

Static Nature: It cannot adapt to real-time, unstructured data like sudden weather alerts or agricultural news.

Lack of Reasoning: It provides a prediction number but cannot autonomously generate a structured, strategic farming plan.

Upcoming in Milestone 2: The system will be upgraded into an Agentic AI Retention Assistant using frameworks like LangGraph. It will autonomously reason about yield risks, retrieve farming best practices via RAG, and generate structured, actionable advice for farmers.


## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
Feel free to check the issues page. If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are warmly welcome.

## 📝 License

This project is for academic and research purposes as part of the Intelligent Crop Yield Prediction coursework.



  
