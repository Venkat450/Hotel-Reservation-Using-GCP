
# Hotel Reservation No-Show Prediction Pipeline

\

## Overview

This project is a modular machine learning pipeline for predicting hotel reservation no-shows, leveraging **LightGBM**, **MLFlow**, and a robust CI/CD process. Designed for scalability and reliability, it helps hotels proactively manage bookings, reduce revenue loss, and optimize inventory.

---

## Features

- **Data Ingestion & Preprocessing:** Cleans and unifies reservation records from multiple sources.
- **Model Training:** Utilizes LightGBM with `RandomizedSearchCV` for hyperparameter tuning.
- **Experiment Tracking:** Employs MLFlow for tracking model parameters, metrics, and artifacts.
- **Error Handling & Logging:** Built-in robust error logging and handling for pipeline reliability.
- **Model Versioning:** Version control for datasets and models to ensure reproducibility and compliance.
- **CI/CD Integration:** Jenkins automates testing, deployment, and monitoring for production readiness.
- **Performance Reporting:** Tracks and reports key metrics including precision, recall, and F1-score.

---

## Tech Stack

- **Python**: Core programming language
- **LightGBM**: Model training and prediction
- **MLFlow**: Experiment and model tracking
- **Jenkins**: CI/CD automation
- **GCP (Google Cloud Platform)**: Cloud deployment and storage
- **RandomizedSearchCV**: Hyperparameter optimization

---

## Pipeline Architecture

1. **Data Loading:** Retrieve and clean hotel reservation data.
2. **Feature Engineering:** Generate features relevant for no-show prediction.
3. **Model Training:** Train and optimize LightGBM model.
4. **Experiment Tracking:** Log results with MLFlow.
5. **Model Versioning:** Store model artifacts with unique version identifiers.
6. **Automated Deployment:** Jenkins triggers retraining and deployment on updates.
7. **Monitoring:** Automated metric tracking and alerting for performance drops.

---

## Getting Started

### Prerequisites

- Python 3.8+
- [Google Cloud SDK](https://cloud.google.com/sdk)
- [Jenkins](https://jenkins.io)
- MLFlow (`pip install mlflow`)
- LightGBM (`pip install lightgbm`)
- Required Python packages (`pip install -r requirements.txt`)

### Installation

1. **Clone the Repository**
    ```sh
    git clone https://github.com/Venkat450/Hotel-Reservation-Using-GCP
    cd Hotel-Reservation-Using-GCP
    ```

2. **Install Dependencies**
    ```sh
    pip install -r requirements.txt
    ```

3. **Configure GCP & Environment Variables**
    - Set your GCP credentials and environment variables as needed.

4. **Run Pipeline**
    ```sh
    python train_pipeline.py
    ```

---

## CI/CD

- **Jenkins Pipeline:** Jenkins automates testing, retraining, and deployment on commit.
- **MLFlow Tracking:** View experiments at the MLFlow dashboard URL provided in your environment.
- **GCP Deployment:** Models are stored and deployed via GCP services.

---

## Usage

- **Training:** `python train_pipeline.py`
- **Prediction:** `python predict.py --input data/sample_input.csv`
- **Monitor Experiments:** Launch MLFlow UI with `mlflow ui`

---

## Results

- **Precision, Recall, F1:** Tracked and reported after each run.
- **Experiment Logs:** Stored in MLFlow for comparison and reproducibility.

---

## License

This project is licensed under the MIT License.

---

## Contact

For questions or collaboration, reach out via [GitHub Issues](https://github.com/Venkat450/Hotel-Reservation-Using-GCP/issues) or connect with [Sree Venkat Chintakula](mailto:sreevenkat450@gmail.com).

---
