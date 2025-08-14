##FIFA 21 PLAYER STATS ANALYSIS
##FIFA 21 PLAYER STATS ANALYSIS
📌 Overview

This project focuses on analyzing FIFA player statistics and creating new features to better understand player performance.
We perform Exploratory Data Analysis (EDA), Feature Engineering, and Data Preprocessing to prepare the dataset for further insights or machine learning models.

The analysis helps in:

Understanding the relationship between a player’s overall rating and potential

Measuring skill gaps

Identifying players’ fitness levels using BMI

Preparing data for scouting or prediction models

📂 Dataset

Source: players_15.csv (FIFA dataset)

Key Columns:

overall – Current player rating

potential – Predicted peak rating

height_cm – Player height in centimeters

weight_kg – Player weight in kilograms

Other attributes like nationality, club, position, and value


🔍 Steps Performed
1. Exploratory Data Analysis (EDA)

Checked data types, null values, and duplicates

Visualized player distributions for ratings, potential, height, and weight

Studied correlations between numerical attributes

2. Data Cleaning

Handled missing values

Removed irrelevant/unnecessary columns

3. Feature Engineering

Overall to Potential Ratio:
df['overall_to_potential_ratio'] = df['overall'] / df['potential']
Helps compare how close a player is to reaching their potential.

Skill Gap:
df['skill_gap'] = df['potential'] - df['overall']
Measures how much improvement is possible for a player.

Body Mass Index (BMI):
df['bmi'] = df['weight_kg'] / ((df['height_cm'] / 100) ** 2)
Indicates physical fitness level.

BMI Category:
Categorized players as Underweight, Normal, Overweight, or Obese based on BMI values.

📊 Tools & Libraries Used
Python

Pandas – Data manipulation

NumPy – Numerical calculations

Matplotlib & Seaborn – Data visualization

📈 Insights
Players with a higher overall_to_potential_ratio are already close to their peak performance.

Large skill_gap values suggest high growth potential.

Most professional players fall in the Normal BMI range.

🚀 Future Scope
Predict player market value using ratings and physical stats

Build a scouting recommendation system

Track player growth over time

🛠️ How to Run
git clone https://github.com/yourusername/fifa-players-analysis.git
cd fifa-players-analysis
pip install -r requirements.txt
python analysis.py
