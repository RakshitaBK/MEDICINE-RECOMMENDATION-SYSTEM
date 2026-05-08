# MEDICINE-RECOMMENDATION-SYSTEM
# MediScan — AI-Powered Medical Recommendation System

A redesigned, fully functional Flask web app that predicts diseases from symptoms using a trained SVM model and provides personalized health guidance.

## Setup

```bash
pip install -r requirements.txt
python main.py
```

Then open http://localhost:5000 in your browser.

## Project Structure

```
health_project/
├── main.py                  # Flask app (fixed & complete)
├── requirements.txt
├── models/
│   └── svc.pkl              # Pre-trained SVM classifier
├── datasets/
│   ├── Training.csv
│   ├── symtoms_df.csv
│   ├── precautions_df.csv
│   ├── medications.csv
│   ├── diets.csv
│   ├── workout_df.csv
│   ├── description.csv
│   └── Symptom-severity.csv
├── static/
│   └── img.png              # Logo
└── templates/
    ├── base.html            # Shared layout, nav, footer
    ├── index.html           # Home + symptom predictor
    ├── about.html
    ├── blog.html
    ├── developer.html
    └── contact.html
```

## How to Use

1. Go to the home page
2. Type symptoms separated by commas (e.g. `itching, fatigue, headache`)
3. Click **Analyze Symptoms**
4. View disease prediction + click cards for medications, diet, workouts, and more

## Notes

- This tool is for informational purposes only — not a substitute for professional medical advice.
- The SVM model covers 41 diseases and 132 symptoms.
