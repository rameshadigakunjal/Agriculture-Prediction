# AgroVedan: Rice Yield and Soil Nutrient Prediction

## Overview
AgroVedan is an innovative machine learning-based system designed to empower rice farmers with precise predictions for crop yields and optimal soil nutrient conditions. By leveraging the Random Forest algorithm and a comprehensive dataset spanning 1986 to 2017, AgroVedan addresses critical challenges in rice cultivation, such as climate variability, soil degradation, and food security. The system provides actionable insights on rice yield (kg/ha) and optimal levels of Nitrogen (N), Phosphorus (P), Potassium (K), and soil pH, enabling farmers to optimize resources and enhance productivity.

The project integrates a user-friendly web interface built with HTML, CSS, and JavaScript, a robust backend powered by Python libraries (Scikit-learn, Pandas, NumPy), and a lightweight SQLite3 database. Hosted on Render with Git-based continuous deployment, AgroVedan ensures accessibility and scalability for farmers, particularly smallholders in semi-arid regions of India.

## Features
- **Accurate Yield Prediction**: Forecasts rice yield based on historical data, including production, cultivated area, and environmental factors (temperature, humidity, rainfall). 
- **Soil Nutrient Optimization**: Recommends optimal NPK levels and soil pH for maximum crop health and productivity.
- **User-Friendly Interface**: A responsive web dashboard for easy data input and visualization of predictions.
- **Robust Evaluation**: Employs metrics like Mean Absolute Error (MAE), R-squared (R²), and Precision to ensure reliable predictions.
- **Scalable Design**: Supports future enhancements like real-time data integration, satellite imagery, and mobile app development.

## Dataset
The model is trained on a historical dataset (1986–2017) sourced from agricultural records, including:
- **Input Parameters**: Rice production (tons), cultivated area (hectares), year, temperature (°C), humidity (%), rainfall (mm).
- **Predicted Parameters**: Rice yield (kg/ha), Nitrogen (kg/ha), Phosphorus (kg/ha), Potassium (kg/ha), soil pH.

## Installation
### Prerequisites
- **Operating System**: Windows 10/11, macOS 10.15+, or Linux (Ubuntu 20.04+)
- **Python**: Version 3.8 or higher
- **Web Browser**: Chrome, Firefox, Edge, or Safari (latest versions)
- **Hardware**: Minimum Intel i3 processor, 4 GB RAM, 1 GB free disk space (SSD recommended)

### Setup Instructions
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/rameshadigakunjal/Agriculture-Prediction.git
   cd Agriculture-Prediction
   ```
2. **Create a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. **Install Dependencies**:
  ```bash
  pip install -r requirements.txt
  ```
4. **Run the Application**:
   ```bash
   python app.py
   ```
   Access the web interface at http://localhost:5000 in your browser.

## Usage

1. **Register/Login**: Create an account or log in using demo credentials (email: demo@agrovedan.com, password: demo1). <br>
2. **Input Data**: Navigate to the "Predict" section and enter farming data (e.g., location, year, production, temperature, humidity, rainfall).<br>
3. **Get Predictions**: Submit the form to receive predicted rice yield and recommended NPK levels/soil pH.<br>
4. **Review Results**: View results on the dashboard and use the "Try Another Prediction" option for new inputs.<br>
5. **Logout**: Securely log out to end your session.<br>

### Project Structure

Agriculture-Prediction/ <br>
├── app.py                  # Main Flask application <br>
├── models/                 # Trained ML models (.pkl files) <br>
├── static/                 # CSS and JavaScript files <br>
├── templates/              # HTML templates for web interface <br>
├── data/                   # Dataset files (rice_dataset1.csv, cleaned_rice_data.csv)<br>
├── notebooks/              # Jupyter Notebooks for data analysis and model training <br>
├── requirements.txt        # Python dependencies <br>
└── README.md               # Project documentation<br>

### Model Performance
The Random Forest model achieves high accuracy, as evaluated by the following metrics: <br>

Rice Yield: Accuracy: 1.0000, Precision: 1.0000, MAE: 1.0664, R²: 1.0000 <br>
Nitrogen (N): Accuracy: 0.9986, Precision: 0.9964, MAE: 0.1683, R²: 0.9953 <br>
Phosphorus (P): Accuracy: 0.9957, Precision: 0.9906, MAE: 0.1102, R²: 0.9887 <br>
Potassium (K): Accuracy: 1.0000, Precision: 0.9978, MAE: 0.0318, R²: 0.9959 <br>
Soil pH: Accuracy: 0.9986, Precision: 0.9986, MAE: 0.0188, R²: 0.9960 <br>

### Future Enhancements

1. **Real-Time Data**: Integrate IoT sensors and weather APIs for dynamic inputs. <br>
2. **Mobile App**: Develop a mobile application for offline access and multilingual support.<br>
3. **Satellite Imagery**: Use remote sensing for precise crop health monitoring.<br>
4. **Advanced Models**: Explore hybrid ML models (e.g., LSTM, Vision Transformers) for improved accuracy.<br>
5. **Farmer Training**: Add educational modules and chatbots to support technology adoption.<br>
6. **Scalability**: Extend the system to other crops and regions with localized datasets.<br>

## Contributing
**Contributions are welcome! To contribute:** <br>

Fork the repository. <br>
Create a feature branch (git checkout -b feature-name).<br>
Commit your changes (git commit -m "Add feature-name").<br>
Push to the branch (git push origin feature-name).<br>
Open a pull request on GitHub.<br>

