# Medicine Recommendation System

A web application that uses machine learning to predict diseases based on symptoms and recommend medications, precautions, workouts, and dietary suggestions.

## Overview

The Medicine Recommendation System is a Flask-based web application that leverages a trained Support Vector Classifier (SVC) model to predict diseases based on user-input symptoms. The system then provides comprehensive recommendations including medications, precautions, dietary advice, and workout suggestions for the predicted condition.

## Features

- Disease prediction based on symptoms input
- Speech recognition for voice input of symptoms
- Detailed disease information including:
  - Disease description
  - Recommended precautions
  - Medication suggestions
  - Workout recommendations
  - Dietary advice
- Responsive design for desktop and mobile devices

## Project Structure

```
Medicine-Recommendation-System/
├── datasets/                  # Contains all data files
│   ├── description.csv        # Disease descriptions
│   ├── diets.csv              # Diet recommendations
│   ├── medications.csv        # Medication suggestions
│   ├── precautions_df.csv     # Precautions for diseases
│   ├── symtoms_df.csv         # Symptoms data
│   └── workout_df.csv         # Workout recommendations
├── models/                    # Contains trained ML models
│   └── svc.pkl                # Support Vector Classifier model
├── static/                    # Static files (CSS, JS, images)
│   ├── img.png                # Logo image
│   └── images/                # Additional images if any
├── templates/                 # HTML templates
│   ├── about.html             # About page
│   ├── base.html              # Base template with common elements
│   ├── blog.html              # Blog page
│   ├── contact.html           # Contact page
│   ├── developer.html         # Developer info page
│   └── index.html             # Main application page
├── main.py                    # Flask application
├── requirements.txt           # Python dependencies
├── run.bat                    # Windows startup script
└── run.sh                     # Unix/Linux/Mac startup script
```

## Installation

### Prerequisites
- Python 3.8 or higher
- pip (Python package installer)

### Setup

1. Clone this repository
   ```
   git clone https://github.com/yourusername/Medicine-Recommendation-System.git
   cd Medicine-Recommendation-System
   ```

2. Setup using scripts:

   **For Windows:**
   ```
   run.bat
   ```

   **For macOS/Linux:**
   ```
   chmod +x run.sh
   ./run.sh
   ```

   The scripts will:
   - Create a virtual environment
   - Activate the virtual environment
   - Install required dependencies
   - Start the application

3. Manual setup:
   ```
   # Create virtual environment
   python -m venv venv
   
   # Activate virtual environment
   # On Windows:
   venv\Scripts\activate
   # On macOS/Linux:
   source venv/bin/activate
   
   # Install dependencies
   pip install -r requirements.txt
   
   # Run the application
   python main.py
   ```

## Usage

1. Open your web browser and navigate to `http://127.0.0.1:5000`
2. Enter symptoms in the input field (separated by commas) or use the speech recognition feature
3. Click "Predict" to get disease prediction and recommendations

## Model Information

The system uses a Support Vector Classifier (SVC) trained on symptoms data to predict diseases. The model achieves high accuracy in identifying common diseases based on symptom patterns.

## Technologies Used

- Python 3.x
- Flask
- Pandas
- NumPy
- scikit-learn
- Bootstrap 5
- HTML/CSS/JavaScript
- Web Speech API

## Demo

You can try out the system by following these steps:
1. Input symptoms like "fever, cough, fatigue"
2. The system will predict the most likely disease
3. View comprehensive recommendations for managing the condition

## Future Improvements

- Add user authentication
- Implement disease history tracking
- Enhance mobile responsiveness
- Add more diseases and symptoms to the database
- Integrate with medical APIs for additional information

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Developer

Adarsh Singh - Software Developer

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Disclaimer

This application is for educational purposes only and should not replace professional medical advice. Always consult with a healthcare professional for medical concerns.
