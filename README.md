⚽ FIFA Player Stats – EDA & Feature Engineering

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

Overall to Potential Ratio
Skill Gap
Body Mass Index (BMI):

pie chart for age group:
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/8a155e8a-2757-48a2-ae22-7b69bd15cede" />

Bar chart for FIFA dataset:

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/3d098895-5548-42fc-9382-bf445f9de1e1" />



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
