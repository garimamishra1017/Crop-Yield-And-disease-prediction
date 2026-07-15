🌱 Crop Yield & Disease Prediction
Overview  
This project integrates machine learning and deep learning techniques to assist farmers in predicting crop yield and detecting plant diseases. It combines synthetic datasets, NDVI satellite imagery preprocessing, CNN‑based disease detection, and a Streamlit dashboard for user interaction.

Key Features

Synthetic dataset generator for weather, soil, and yield data.

NDVI preprocessing using Sentinel‑2 satellite imagery for vegetation health monitoring.

CNN model (ResNet18) for leaf disease classification (Healthy vs Diseased).

Gradient Boosting Regressor for yield forecasting based on rainfall, temperature, humidity, and soil moisture.

Streamlit dashboard with ngrok integration for real‑time predictions.

Installation  
Clone the repository and install dependencies:

bash
git clone https://github.com/your-username/crop-yield-disease-prediction.git
cd crop-yield-disease-prediction
pip install -r requirements.txt
Dependencies include PyTorch, Torchvision, Scikit‑learn, Pandas, Rasterio, Streamlit, Pyngrok, and Joblib.

Usage

Generate synthetic dataset using generate_dataset.py.

Train CNN for disease detection with PlantVillage dataset.

Train yield forecasting model using train_yield.py.

Launch the dashboard with streamlit run dashboard.py and access via ngrok public URL.

Workflow  
The workflow follows five steps:
(i) Synthetic dataset creation,
(ii) NDVI preprocessing,
(iii) CNN training for disease detection,
(iv) Gradient Boosting for yield forecasting,
(v) Streamlit dashboard deployment.

Project Structure

Code
├── generate_dataset.py       # Synthetic dataset generator
├── ndvi_preprocessing.py     # NDVI computation
├── train_cnn.py              # CNN training script
├── train_yield.py            # Yield forecasting model
├── dashboard.py              # Streamlit farmer dashboard
├── crop_yield.csv            # Sample dataset
├── requirements.txt          # Dependencies
└── README.md                 # Documentation
Future Scope  
Planned improvements include expanding disease classification to multiple categories, integrating real‑time weather APIs, and deploying models on cloud platforms for scalability.

Contributing  
Contributions are welcome. Please open an issue before submitting a pull request to discuss proposed changes.

License  
This project is licensed under the MIT License.
