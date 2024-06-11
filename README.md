# Forest Fire Prediction

Welcome to the Forest Fire Prediction project! This repository contains a machine learning model that predicts the likelihood of forest fires based on various environmental factors. The model uses Ridge Regression to make predictions and is deployed using Flask.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model](#model)
- [Installation](#installation)
- [Usage](#usage)
- [Directory Structure](#directory-structure)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
Forest fires are a critical issue that can have devastating effects on the environment, wildlife, and human life. This project aims to predict forest fire occurrences based on various environmental factors such as temperature, relative humidity, wind speed, and more. The goal is to provide an early warning system that can help in taking preventive measures to mitigate the impact of forest fires.

## Dataset
The dataset used for training the model includes various environmental factors:
- **Temperature**: Ambient temperature in Celsius.
- **RH**: Relative Humidity (%).
- **Ws**: Wind speed (km/h).
- **Rain**: Rainfall (mm).
- **FFMC**: Fine Fuel Moisture Code.
- **DMC**: Duff Moisture Code.
- **ISI**: Initial Spread Index.
- **Classes**: Fire occurrence classification.
- **Region**: The region where the data was collected.

## Model
The machine learning model used in this project is Ridge Regression. The model was trained using the dataset mentioned above, and the predictions are scaled using Standard Scaler for better accuracy.

## Installation
To run this project locally, follow these steps:

1. **Clone the repository**:
   ```sh
   git clone https://github.com/Lavishgangwani/ForestFirePrediction.git
   cd ForestFirePrediction
   ```

2. **Create a virtual environment** (optional but recommended):
   ```sh
   python -m venv env
   source env/bin/activate  # On Windows, use `env\Scripts\activate`
   ```

3. **Install the required packages**:
   ```sh
   pip install -r requirements.txt
   ```

4. **Run the Flask application**:
   ```sh
   python app.py
   ```

## Usage
After starting the Flask application, open your web browser and navigate to `http://127.0.0.1:5000/`. You will see a form where you can input the environmental factors. Fill in the values and click the "Predict" button to see the prediction result.

### Example Input
- **Temperature**: 25.0
- **RH**: 45.0
- **Ws**: 5.0
- **Rain**: 0.1
- **FFMC**: 85.0
- **DMC**: 50.0
- **ISI**: 7.0
- **Classes**: 1.0
- **Region**: 2.0

## Directory Structure
```
forestfire/
├── models/
│   ├── ridge.pkl
│   ├── scaler.pkl
├── templates/
│   ├── index.html
│   ├── home.html
├── app.py
├── requirements.txt
├── README.md
```

## Contributing
We welcome contributions to improve the Forest Fire Prediction project. If you have any suggestions or improvements, please submit a pull request or contact me directly at [lavishgangwani22@gmail.com](mailto:lavishgangwani22@gmail.com).

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.