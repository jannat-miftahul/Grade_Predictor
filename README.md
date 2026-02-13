# Grade Predictor

A machine learning web application that predicts student HSC (Higher Secondary Certificate) exam results based on various demographic, academic, and social factors.
<<<<<<< HEAD

## Features

- 🎯 Accurate grade prediction using Random Forest algorithm
- 🖥️ Interactive web interface built with Gradio
- 📊 Real-time predictions based on student data
- 🌐 Shareable web link for easy access

## Dataset

The model is trained on Bangladesh student performance data, considering factors such as:
- Demographic information (gender, age, address)
- Family background (size, parent status, education levels)
- Parental occupation
- Social factors (relationships, smoking habits, time with friends)
- Financial factors (tuition fees)
- Previous academic performance (SSC results)

## Model

- **Algorithm**: Random Forest Regressor
- **Pipeline**: Includes preprocessing and feature engineering
- **Output**: Predicted HSC GPA (0-5 scale)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/grade-predictor.git
cd grade-predictor
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/Scripts/activate  # On Windows
# source venv/bin/activate    # On Linux/Mac
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Train the model (if needed):
```bash
python rf_train.py
```

2. Launch the web application:
```bash
python app.py
```

3. Open the provided URL in your browser and input student information to get grade predictions.

## Input Parameters

- **Gender**: Male (M) or Female (F)
- **Age**: Student's age
- **Address**: Urban or Rural
- **Family Size**: Greater than 3 (GT3) or Less/Equal to 3 (LE3)
- **Parent Status**: Together or Apart
- **Mother's Education**: Scale 0-4
- **Father's Education**: Scale 0-4
- **Mother's Job**: At_home, Health, Other, Services, or Teacher
- **Father's Job**: Teacher, Other, Services, Health, Business, or Farmer
- **Relationship**: Yes or No
- **Smoker**: Yes or No
- **Tuition Fee**: Amount in local currency
- **Time with Friends**: Scale 1-5
- **SSC Result**: Previous GPA score

## Project Structure

```
grade-predictor/
│
├── app.py                              # Gradio web application
├── rf_train.py                         # Model training script
├── bangladesh_student_performance.csv  # Dataset
├── student_rf_pipeline.pkl             # Trained model pipeline
├── requirements.txt                    # Python dependencies
└── README.md                          # Project documentation
```

## Requirements

- Python 3.7+
- gradio
- pandas
- scikit-learn
- numpy
=======
>>>>>>> 21744e57e0c782589cd94a7fceb4de4db69b9d1b
