# IMDB Movie Reviews Sentiment Analysis | IMDB Film Yorumları Sentiment Analizi

### **Project Overview**
This project analyzes the **IMDB Dataset of 50K Movie Reviews** using statistical methods and visualizations to explore the differences between positive and negative sentiments. The analysis includes **Exploratory Data Analysis (EDA)**, **Data Preprocessing**, **Hypothesis Testing**, and **Visualization**.

### **Project Details:**
- **Dataset:** IMDB Movie Reviews Dataset from Kaggle
- **Objective:** To perform sentiment analysis on movie reviews and compare positive and negative sentiments based on review length using statistical tests such as ANOVA and Chi-Squared.

### **Key Steps in the Project:**

#### 1. **Dataset Loading and Exploration:**
- Load the IMDB movie reviews dataset from Kaggle.
- Preview the first few rows and inspect the structure.

#### 2. **Exploratory Data Analysis (EDA):**
- Analyze the sentiment distribution of the reviews (positive vs negative).
- Visualize the data using bar and pie charts.

#### 3. **Data Cleaning and Preprocessing:**
- Check for missing data and fill missing reviews with 'No Review'.
- Create a new feature `review_length` to represent the length of each review.

#### 4. **Statistical Analysis:**
- Perform **ANOVA** test to compare the length of positive and negative reviews.
- Perform **Chi-Squared** test to examine the relationship between sentiment and review length.

#### 5. **Visualization:**
- Visualize sentiment distribution, review length distribution, and sentiment-based review length comparison using bar charts, pie charts, histograms, and boxplots.

---

### **Results and Insights:**
- **Positive Reviews** tend to be longer, indicating more detailed expressions of satisfaction.
- **Negative Reviews** are typically shorter, suggesting that criticism is more concise.
- **Business Application:**
  - This analysis can be used to understand user feedback better and tailor responses to positive and negative sentiments accordingly.

### **Libraries Used:**
- **Pandas:** Data manipulation and analysis.
- **NumPy:** Numerical computations.
- **Matplotlib & Seaborn:** Data visualizations.
- **SciPy:** Statistical analysis (ANOVA, Chi-Squared).

### **How to Run the Project:**
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/imdb-sentiment-analysis.git
Navigate to the project folder:
cd imdb-sentiment-analysis
Install dependencies:
pip install -r requirements.txt
Open and run the Jupyter Notebook:
jupyter notebook IMDB_Sentiment_Analysis.ipynb
Kaggle and GitHub Links:
Kaggle Notebook: IMDB Sentiment Analysis on Kaggle
GitHub Repository: GitHub Repo
