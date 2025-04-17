# Bribery Reporting Analysis – India

This project explores a real-world dataset of bribery complaints submitted by citizens in India. The goal is to understand corruption patterns across departments, locations, and time, along with analyzing the financial burden of reported bribes. This work sheds light on systemic issues and presents visual insights using Python-based exploratory data analysis (EDA).

---

## 📂 Data

The dataset was obtained from a public bribery reporting platform and contains citizen-submitted complaints. It includes the following fields:

- **Title**: Description of the bribery experience  
- **Date**: When the complaint was posted  
- **Location**: City and State (split into two fields: `City`, `Province`)  
- **Department**: Department where the bribe was taken (e.g., Traffic, Property Registration)  
- **Views**: Number of times the complaint was viewed  
- **Amount(INR)**: Reported bribe amount in Indian Rupees  

Initial cleaning was performed to handle missing values, standardize categories, and treat outliers.

---

## 🔍 Analysis Workflow

Implemented in Python using Jupyter Notebook, the workflow consists of the following steps:

- Data cleaning and preprocessing  
  - Splitting `Location` into `City` and `Province`  
  - Handling missing values in `Department`  
  - Removing outliers from `Amount(INR)` using top 10% trimming  
- Exploratory Data Analysis (EDA)  
  - Aggregations by city, province, and department  
  - Monthly and weekday trends in bribe reporting  
  - Analysis of departments by complaint frequency and bribe totals  
  - Visualization of complaint counts, bribe amounts, and viewership  

---

## 📊 Key Findings

- **Karnataka** and **Maharashtra** emerged as top provinces with the highest number of complaints.
- **Bangalore** was the leading city in terms of bribery reports.
- **Traffic**, **Driving License**, and **Property Registration** were the most commonly reported departments.
- High-value bribes were primarily associated with departments like **Encumbrance Certificate** and **Sale Deed Registration**.
- Bribery reports were consistent across weekdays, with slight dips on Sundays.
- The number of complaints peaked during specific months, possibly due to government actions, media coverage, or seasonal factors.

---

## 📈 Visual Insights

The project includes a wide variety of visualizations:

- Histograms and KDE plots of `Amount(INR)` (before and after outlier removal)  
- Bar plots of top cities, provinces, and departments by complaint count  
- Horizontal bar charts showing departments by total bribe amount  
- Time series plots of complaints by weekday and month  
- Scatter plots of bribe amount vs views  

---

## 🛠️ Libraries Used

- **Data Manipulation**: `pandas`, `numpy`  
- **Visualization**: `matplotlib`, `seaborn`, `plotly`  
- **Date Handling**: `datetime`  
- **Text Processing** (planned): `wordcloud`, `nltk`, `TextBlob`  

---

## 📁 Notebooks & Scripts
  - Future versions may include:
  - Sentiment analysis of complaint titles using NLP  
  - Geographic choropleths using `plotly` or `folium`  
  - Dashboard version in Power BI or Tableau  

---

## ✅ Usage

To reproduce the analysis:

1. Clone the repository  
2. Place the dataset CSV file in the working directory  
3. Run the `bribery-corruption-india.ipynb` notebook  
4. Explore interactive and static visualizations for insights  

---

## 🔄 Potential Improvements

- Add sentiment analysis from complaint titles using NLP  
- Create an interactive dashboard for real-time filtering by location or department  
- Integrate complaint frequency with state population for normalized corruption scores  
- Apply topic modeling or clustering to group types of corruption  

---

## 👤 Author

**Rohit Shivhare**  
[LinkedIn](https://www.linkedin.com/in/rohit-shivhare-a857a4233/)  
*MSc Data Science – Brunel University, London*
