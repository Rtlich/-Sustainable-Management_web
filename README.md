# Sustainable Management Predictions

A web application featuring two machine learning models for predicting water consumption and notification priorities.

## Project Structure

```
projetbi/
├── backend/              # Flask backend
│   ├── models/          # Trained ML models
│   │   ├── water_consumption_model.pkl    # LightGBM model
│   │   └── notification_model.pkl         # XGBoost model
│   ├── app.py          # Main Flask server
│   ├── save_model.py   # Water consumption model training (LightGBM)
│   └── train_notification_model.py  # Notification model training (XGBoost)
└── src/                 # Angular frontend
```

## Setup Instructions

### 1. Backend Setup

First, navigate to the backend directory:
```bash
cd backend
```

Install Python dependencies:
```bash
pip install -r requirements.txt
```

Train both machine learning models:
```bash
# 1. Train water consumption model (LightGBM)
python save_model.py

# 2. Train notification priority model (XGBoost)
python train_notification_model.py
```

Start the Flask server:
```bash
python app.py
```
The backend will be available at http://localhost:5000

### 2. Frontend Setup

In a new terminal, navigate to the project root:
```bash
cd ..  # If you're in the backend directory
```

Install Node.js dependencies:
```bash
npm install
```

Start the Angular development server:
```bash
ng serve
```
The frontend will be available at http://localhost:4200

## Machine Learning Models

1. **Water Consumption Model (LightGBM)**
   - Predicts water consumption based on:
     - Initial stock
     - Unit price
   - Training script: `save_model.py`
   - Model type: LightGBM Regressor

2. **Notification Priority Model (XGBoost)**
   - Predicts notification priority based on:
     - Category
     - Description
   - Includes severity scoring system
   - Training script: `train_notification_model.py`
   - Model type: XGBoost Classifier

## Development

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 19.2.9.

### Angular Development Commands

- **Development server**: `ng serve`
- **Build**: `ng build`
- **Unit tests**: `ng test`
- **End-to-end tests**: `ng e2e`

For more information on using the Angular CLI, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
