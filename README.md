# ColorCouture- Smart Outfit Recommendation System

---

## Project Description

This project is a Fashion Color Recommendation System that suggests suitable topwear colors based on the selected bottomwear color. Using a dataset of color combinations and fashion attributes, the system leverages machine learning (K-Nearest Neighbors) to provide recommendations considering color harmony and fashion trends.

---

## Features

Accepts bottomwear color as hex code input.
Converts color input to RGB format for analysis.
Recommends topwear colors with details like season, occasion, and mood.
Uses K-Nearest Neighbors algorithm for similarity matching.
Provides fashion insights such as trend alignment and skin tone compatibility.

---

## Technologies Used

Python
Flask (for REST API)
Pandas and NumPy (for data processing)
Scikit-learn (for machine learning)
Flask-CORS (to enable frontend requests)

---

## Dataset Description

The dataset used contains the following columns:

Topwear_Color_Name, 
Topwear_Hex, 
Bottomwear_Color_Name, 
Bottomwear_Hex, 
Contrast_Score, 
Trend_Alignment, 
Season, 
Occasion, 
Popularity_Score, 
Mood_Conveyed, 
Time_of_Day_Preference, 
Skin_Tone_Compatibility.

---

## How to Run

Clone the repository:

git clone https://github.com/Ananya2125/Final_year_project.git

Navigate to the project folder:

cd your_project

Install required packages:

pip install -r requirements.txt

Ensure the dataset file Final_Topwear_Bottomwear_Color_Combinationss.csv is in the project directory.

Run the Flask application:
python app.py

The API will be available at http://localhost:8000. Use POST requests to /recommend endpoint with JSON body:

{ "color": "#hexcode" }

to get topwear color recommendations.

---

## Example Request

curl -X POST http://localhost:8000/recommend -H "Content-Type: application/json" -d '{"color": "#FF5733"}'

---

## Future Enhancements

Add a frontend interface for easier user interaction.

Expand the dataset with more fashion attributes and more combinations.

Improve recommendation by incorporating user preferences and feedback.

Include personalized style recommendations based on user profile.
