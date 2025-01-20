# Breast Cancer Prediction App

This project is a **Streamlit** [web application](https://cancer-prediction-app.streamlit.app) that predicts whether a breast mass is benign or malignant using a machine learning model. The app provides an interactive interface where users can input cell nucleus measurements and visualize the results with a radar chart.


<img width="1662" alt="Screenshot 2025-01-20 at 2 03 42 PM" src="https://github.com/user-attachments/assets/809b75b3-306f-474b-b9d2-7c4c38f4baa4" />


---

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Files and Directories](#files-and-directories)
- [Dependencies](#dependencies)
- [Credits](#credits)

---

## Features
- Predicts whether a breast mass is **benign** or **malignant** based on user-provided measurements.
- Displays the prediction probabilities for both benign and malignant classes.
- Visualizes the mean, standard error, and worst-case values of measurements using a radar chart.
- Interactive sidebar with sliders to input or modify cell nucleus measurements.
- Assists medical professionals in decision-making but does not substitute professional diagnosis.

---

## Installation

1. **Clone the repository**:
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```

2. **Install required packages**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Prepare the data and model files**:
   - Place the `data.csv` file in the `data/` directory.
   - Add the trained `model.pkl` and `scaler.pkl` files to the `model/` directory.

4. **Run the app**:
   ```bash
   streamlit run app.py
   ```

---

## Usage

1. **Launch the app**:
   After running the above command, the app will open in your default web browser.

2. **Input measurements**:
   Use the sliders in the sidebar to adjust the cell nucleus measurements.

3. **View the prediction**:
   - The app will display the prediction (Benign or Malignant) along with the probability scores.
   - The radar chart will update dynamically based on the input values.

4. **Interpret results**:
   Use the prediction and visualization to analyze the cell cluster characteristics.

---

## Files and Directories

- **`app.py`**: The main Streamlit application file.
- **`data/`**:
  - `data.csv`: Dataset containing cell nucleus measurements.
- **`model/`**:
  - `model.pkl`: Pre-trained machine learning model for prediction.
  - `scaler.pkl`: Scaler used for normalizing input data.
- **`assets/`**:
  - `style.css`: Custom CSS for styling the Streamlit app.
- **`requirements.txt`**: List of required Python libraries.
- **`README.md`**: Documentation for the project.

---

## Dependencies

- **Python 3.7+**
- **Streamlit**
- **Pandas**
- **Plotly**
- **Scikit-learn**
- **Pickle**

Install all dependencies using:
```bash
pip install -r requirements.txt
```

---

## Credits

This app is developed to assist in early detection and analysis of breast cancer using machine learning techniques. Special thanks to the creators of the original dataset and the developers of the libraries used in this project.
