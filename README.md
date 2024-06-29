# EmployeeAttrition

This repository contains code for a machine learning model API designed to predict employee attrition based on various factors. The model uses a Random Forest Classifier trained on HR data.

## Table of Contents

- [About the Project](#about-the-project)
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## About the Project

This project provides a RESTful API built with Flask for predicting employee attrition. The machine learning model is trained on an HR dataset to classify whether an employee is likely to leave the company or not.

## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

- Python 3.6+
- Pip (Python package installer)

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/deshakil/EmployeeAttritionModel.git
   cd <Your Project Directory>

2. Install Dependencies
   ```sh
   pip install -r requirements.txt

### Usage 

1. Run the Flask application
   ```sh
   python app.py

2. Navigate to http://localhost:5000 in your web browser or use curl to interact with the API endpoints.

### API Endpoints

- POST /predict: Predict employee attrition based on input features.
- Input: JSON object with employee features.
- Output: Prediction (0 or 1) and probability scores.
- example request
  ```json
  {
  "Age": 35,
  "DailyRate": 500,
  "DistanceFromHome": 10,
  "HourlyRate": 50,
  "MonthlyIncome": 6000,
  "MonthlyRate": 12000,
  "NumCompaniesWorked": 2,
  "TotalWorkingYears": 10,
  "YearsAtCompany": 5
  }
- example response
  ```json
  {
  "prediction": 1,
  "probability": [0.3, 0.7]
  }

### Contributing
- Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

- Fork the Project
- Create your Feature Branch (git checkout -b feature/AmazingFeature)
- Commit your Changes (git commit -m 'Add some AmazingFeature')
- Push to the Branch (git push origin feature/AmazingFeature)
- Open a Pull Request

### License
Distributed under the MIT License. See LICENSE for more information.

  
