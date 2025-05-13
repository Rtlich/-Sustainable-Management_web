🌱 Sustainable Agrifood AI System - Project Structure
🗂️ Project Structure
projetbi/
├── 🐋 backend/              # Flask backend
│   ├── 🧠 models/          # Trained ML models
│   │   ├── 💧 water_consumption_model.pkl    # LightGBM model
│   │   └── 🔔 notification_model.pkl         # XGBoost model
│   ├── 🚡 app.py          # Main Flask server
│   ├── 🏋️ save_model.py   # Water consumption model training (LightGBM)
│   └️ 🚨 train_notification_model.py  # Notification model training (XGBoost)
└── 🖥️ src/                 # Angular frontend
🚀 Setup Instructions
1. 🐍 Backend Setup

  cd backend  # 📂 Navigate to backend

# 📦 Install dependencies
pip install -r requirements.txt  

# 🤖 Train ML models
# 1. 💧 Water consumption model (LightGBM)
python save_model.py  

# 2. 🔔 Notification priority model (XGBoost)
python train_notification_model.py  

# 🚀 Start Flask server
python app.py  
2. 🅰️ Frontend Setup
cd ..  # 🔙 Return to project root

# 📦 Install dependencies
npm install  

# 🚀 Start Angular dev server
ng serve  
🌐 Frontend available at http://localhost:4200

🤖 Machine Learning Models
💧 Water Consumption Model (LightGBM)
🔮 Predicts water usage based on:

Initial stock 📦

Unit price 💰

🏋️ Training script: save_model.py

🧠 Model type: LightGBM Regressor

🔔 Notification Priority Model (XGBoost)
⚡ Classifies notification priority:

Category 🏷️

Description 📝

Severity scoring ⚠️

🏋️ Training script: train_notification_model.py

🧠 Model type: XGBoost Classifier

🛠️ Development
🔧 Generated with Angular CLI v19.2.9

🔥 Angular Commands
🚀 Dev server: ng serve

🏗️ Build: ng build

🧪 Unit tests: ng test

🔍 E2E tests: ng e2e

📚 For more Angular CLI info, visit the Angular CLI Documentation

🌐 Interfaces Implemented
Login Page 🔑

Secure authentication for users like "Rania"

Main Dashboard 📈

Revenue analytics

Inventory optimization

Regional distribution data

Water Consumption Prediction 💧

Stock and price inputs

ML-powered predictions

Image Classification 🌿

Ecological vs pollutant detection

Notification Center 🔔

Priority-sorted alerts

🤖 AI Features
🧠 Machine Learning decision support

🌍 Environmental impact analysis

📸 Deep learning image classification

📉 Predictive analytics for resource management
