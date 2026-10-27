# ☀️ Solar Power Output Predictor

An interactive machine learning application that predicts solar power output in watts based on environmental conditions using a pre-trained Linear Regression model.

Built with Python and Streamlit, this project provides a simple interface where users can adjust environmental parameters and estimate solar power output.

## ✨ Features

- **Solar Power Prediction:** Estimates solar power output using a pre-trained Linear Regression model.
- **Interactive Inputs:** Adjust temperature, humidity, solar irradiance, and wind speed using sliders.
- **Model Loading:** Loads the saved model from `solar_power_prediction_model.pkl`.
- **Model Upload:** Allows users to upload a trained `.pkl` model through the sidebar.
- **Instant Results:** Displays the predicted power output when the prediction button is clicked.
- **Simple Interface:** Uses Streamlit to provide an interactive and user-friendly experience.

## 🛠️ Technologies Used

- **Python** – Application development
- **Streamlit** – Interactive web interface
- **Scikit-learn** – Machine learning model
- **NumPy** – Preparing input data for prediction
- **Joblib** – Loading the saved model

## 🌤️ Input Parameters

| Parameter | Unit | Description |
|---|---|---|
| Temperature | °C | Environmental temperature |
| Humidity | % | Relative humidity |
| Solar Irradiance | W/m² | Solar radiation received per unit area |
| Wind Speed | m/s | Environmental wind speed |

The application passes these four values to the model in the same order used during training.

## 📂 Project Structure

```text
solar_energy_predicted/
├── app.py
├── requirements.txt
├── solar_power_prediction_model.pkl
└── .gitignore
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/vidhya-2332/solar_energy_predicted.git
cd solar_energy_predicted
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```powershell
.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Run the application

```bash
streamlit run app.py
```

The terminal will display a local URL, usually `http://localhost:8501`. Open that address in your browser to use the application.

## 🚀 How to Use

1. Start the Streamlit application.
2. Ensure that `solar_power_prediction_model.pkl` is available in the project directory, or upload a compatible model through the sidebar.
3. Adjust the temperature, humidity, solar irradiance, and wind speed sliders.
4. Click **Predict Solar Power Output**.
5. View the estimated solar power output in watts.

## 🧠 Machine Learning Approach

This application uses a pre-trained Linear Regression model to estimate solar power output from four environmental input features.

The model is loaded from a saved `.pkl` file, and the application passes the selected values to the model to generate a prediction.

**Note:** The model training procedure, dataset, evaluation metrics, and prediction accuracy are not documented in the current application code.

## 🎯 Project Objective

The objective is to demonstrate how machine learning can be integrated into an interactive application to estimate solar power output from environmental conditions.

## 🔮 Future Enhancements

- Add model evaluation metrics such as MAE, MSE, and R².
- Include visualizations of environmental inputs and predicted output.
- Provide historical prediction tracking.
- Evaluate the model using additional environmental datasets.
- Deploy the application online for public access.

## 👩‍💻 Author

**Vidhya Sri A J**

- GitHub: [@vidhya-2332](https://github.com/vidhya-2332)

---

*This project is an educational demonstration of machine-learning-based solar power prediction.*
