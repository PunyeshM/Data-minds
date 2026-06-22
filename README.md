# Customer Churn Prediction Web App

This project is a Flask-based web application that predicts customer churn using a pre-trained machine learning model. It also provides data visualization and insights into different customer features and how they correlate with churn.

## Project Structure

- `app.py`: Main Flask application.
- `best_model.pkl`: Pre-trained machine learning model used for predictions.
- `data_set.csv`: Dataset used for generating visualizations and insights.
- `templates/`: Contains HTML templates for the web interface.
- `static/`: Contains static assets like generated graphs.

## Prerequisites

Make sure you have Python 3.8+ installed on your system.

## Setup Instructions

1. **Navigate to the project directory**
   Open your terminal/command prompt and navigate to the `web-app` folder:
   ```bash
   cd path/to/web-app
   ```

2. **Create a virtual environment**
   It's highly recommended to use a virtual environment to manage dependencies.
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**
   - **Windows:**
     ```bash
     venv\Scripts\activate
     ```
   - **macOS / Linux:**
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies**
   Install the required Python packages using pip:
   ```bash
   pip install -r requirements.txt
   ```

## Running the Application

1. Ensure your virtual environment is activated.
2. Run the Flask application:
   ```bash
   python app.py
   ```
3. Open your web browser and go to the local server URL provided in the terminal (usually `http://127.0.0.1:5000/`).

## Features

- **Churn Prediction:** Use the web interface to input customer details and get a prediction on whether they are likely to churn.
- **Visualizations:** Access the `/visualization` route to view automatically generated charts (categorical and numerical features against churn) along with automated insights.

## Notes

- The visualizations are generated on-the-fly and saved to the `static/graphs` directory when accessed.
- Make sure `best_model.pkl` and `data_set.csv` are present in the same directory as `app.py` for the app to function correctly.
