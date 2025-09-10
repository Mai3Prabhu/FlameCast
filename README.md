# FlameCast: Fire Weather Index Prediction
## Project Description:
FlameCast is a web application designed to predict the Fire Weather Index (FWI) using machine learning. The application provides a user-friendly interface for inputting meteorological data and instantly receiving a fire risk prediction. The backend is built with Python and Flask, which serves a RESTful API, while the frontend is a dynamic and interactive web page.

## Project Structure

This project is organized into the following directories:

- application.py: The main Flask application file that defines the web routes and handles the core logic.

- models/: Stores the serialized machine learning models (ridge.pkl and scaler.pkl) used for prediction.

- notebooks/: Contains the Jupyter notebooks used for Exploratory Data Analysis (EDA) and training the machine learning model.

- EDA and Feature Engineering.ipynb: Notebook for data cleaning, analysis, and feature engineering.

- Model Training.ipynb: Notebook for training and saving the final machine learning model.

- templates/: Holds the HTML files for the web application's user interface.

- index.html: The interactive landing page.

- home.html: The main prediction form and results page.

- requirements.txt: Lists all the necessary Python libraries for the project.

- venv/: (Ignored by .gitignore) The Python virtual environment for managing dependencies.

## Setup Instructions
Follow these steps to set up and run the project locally.

**1. Clone the repository**
```
git clone [https://github.com/your-username/flamecast-project.git](https://github.com/your-username/flamecast-project.git)
cd flamecast-project
```

**2. Create and activate a virtual environment**

It is highly recommended to use a virtual environment to manage dependencies.

On macOS/Linux:
```
python3 -m venv venv
source venv/bin/activate
```
On Windows:
```
python -m venv venv
.\venv\Scripts\activate
```

**3. Install dependencies**

Install all the required Python libraries using the requirements.txt file.
```
pip install -r requirements.txt
```

**4. Run the Flask application**

Start the development server with the following command:
```
python application.py
```

The application will be running on http://127.0.0.1:5000. Open this URL in your web browser to access FlameCast.

**How to Use**

- Landing Page: The index.html page serves as the entry point, greeting the user with the project name. Click the "Start Prediction" button to proceed.

- Prediction Form: You will be redirected to the home.html page, which contains a form with fields for various meteorological parameters.

- Submit Data: Enter the required values into the form fields and click the "Predict" button.

- View Result: The prediction result for the Fire Weather Index will be displayed prominently in the results panel on the right side of the screen.

## Tech Stack
- Backend: Python, Flask, Scikit-learn, Pandas, Numpy

- Frontend: HTML, CSS, JavaScript (for dynamic quotes), Bootstrap (for styling)

- Version Control: Git, GitHub

