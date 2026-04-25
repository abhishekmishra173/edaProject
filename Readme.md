# Exploratory Data Analysis (EDA): Titanic Survival Dataset

## 📌 Overview
This project performs an Exploratory Data Analysis (EDA) on the classic Titanic dataset. The primary objective is to clean the raw data, uncover underlying patterns, and use statistical visualizations to identify which key factors (such as age, gender, ticket fare, and passenger class) influenced survival rates during the disaster.

## 📂 Project Structure
- `eda_project.py`: The main Python script that handles data loading, cleaning, and visualization.
- `charts/`: A generated directory containing all exported visualizations (.png files).
- `README.md`: This documentation file detailing project setup and analytical findings.

## 🛠️ Prerequisites & Setup
To run this project on your local machine, you will need Python installed along with a few standard data science libraries.

1. **Install required libraries:**
   ```bash
   pip install pandas numpy matplotlib seaborn

   ```
   1. **Run the script:**
   ```bash
   python eda_project.py
   ```
   Note: Running the script will automatically download the dataset, process it, show the charts on your screen, and save the image files into the charts/ folder.

 ## 📊 Key Insights & Visualizations 
 Below are the key visualizations generated during the analysis, along with the insights derived from each.

 1. **Age Distribution**
The histogram below shows the distribution of passenger ages. The majority of passengers aboard the Titanic were young adults between the ages of 20 and 35. There was also a notable spike representing infants and young children.
![Age Distribution Chart](charts/_age_distribution.png)

2. **Overall Survival Count**
Tragically, the count plot confirms that the majority of passengers did not survive the disaster. Out of the total dataset, the number of non-survivors significantly outnumbers the survivors.
![Survival Count Chart](charts/_survival_count.png)

3. **Age vs. Fare (Color-coded by Survival)**
This scatter plot maps out passenger Age against Ticket Fare, using color to indicate survival (Blue = Did not survive, Orange = Survived). It visually demonstrates that passengers who paid higher fares (higher up on the Y-axis) had a much higher likelihood of survival, regardless of their age.
![Age vs Fare Chart](charts/_age_vs_fare.png)

4. **Age Distribution Across Passenger Classes**
The box plot highlights the socio-economic age divide on the ship. 1st-class passengers tended to be significantly older (median age ~37), while 3rd-class passengers were generally younger (median age ~25).
![Class vs Age Chart](charts/_class_vs_age.png)

5. **Correlation Heatmap**
The heatmap displays the statistical correlation between all numerical variables. A key takeaway is the strong negative correlation between pclass (Passenger Class) and fare (-0.55), which confirms that lower-numbered classes (1st class) were associated with much higher ticket prices.
![Correlation Heatmap Chart](charts/_correlation_heatmap.png)

 ## 💡 Conclusion
Through this Exploratory Data Analysis, we successfully identified critical factors influencing Titanic survival rates. The visualizations clearly show that socio-economic status (represented by ticket fare and passenger class) played a major role in survival outcomes.

This cleaned and analyzed dataset is now well-prepared for the next step in the data science pipeline: feature engineering and predictive machine learning modeling.

  ## Author
  Abhishek Mishra