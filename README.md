# GlobalAIHub_VeriAnalizi


project_name: IMDB Movie Reviews Sentiment Analysis
project_description: |
  This project analyzes the **IMDB Dataset of 50K Movie Reviews** using statistical methods and visualizations to explore the differences between positive and negative sentiments. 
  The analysis includes Exploratory Data Analysis (EDA), data preprocessing, and hypothesis testing.

dataset:
  name: IMDB Dataset of 50K Movie Reviews
  source: Kaggle
  size:
    rows: 50000
    columns: 2
  columns:
    - name: review
      description: The text of the review.
    - name: sentiment
      description: Label indicating whether the review is positive or negative.
  data_preview: |
    review: First five rows of reviews
    sentiment: First five sentiment values
    first_5_rows:
      - review: "One of the other reviewers has mentioned that ..."
        sentiment: positive
      - review: "A wonderful little production. <br /><br />The..."
        sentiment: positive
      - review: "I thought this was a wonderful way to spend ti..."
        sentiment: positive
      - review: "Basically there's a family where a little boy ..."
        sentiment: negative
      - review: "Petter Mattei's 'Love in the Time of Money' is..."
        sentiment: positive

steps:
  - step: Dataset Selection and Loading
    description: |
      The dataset was loaded from Kaggle and the first five rows were previewed.
    code: |
      import pandas as pd
      data = pd.read_csv('/kaggle/input/imdb-dataset-of-50k-movie-reviews/IMDB Dataset.csv')
      print(data.head())
      print(data.columns)
      print(data.info())
  - step: Exploratory Data Analysis (EDA)
    description: |
      Analyzed the distribution of sentiments (`positive`, `negative`) using bar and pie charts.
    code: |
      import matplotlib.pyplot as plt
      sentiment_counts = data['sentiment'].value_counts()
      sentiment_counts.plot(kind='bar', color=['blue', 'orange'])
      plt.xlabel('Sentiment')
      plt.ylabel('Count')
      plt.title('Sentiment Distribution')
      plt.show()
  - step: Data Cleaning and Preprocessing
    description: |
      Checked for missing data and handled it by filling missing values in the `review` column with 'No Review'.
    code: |
      print(data.isnull().sum())
      data['review'] = data['review'].fillna('No Review')
      print(data.isnull().sum())
  - step: Statistical Analysis
    description: |
      ANOVA Test was applied to compare the length of positive and negative reviews.
      Chi-Squared Test was applied to see the relationship between sentiment and review length.
    code: |
      from scipy.stats import f_oneway, chi2_contingency
      data['review_length'] = data['review'].apply(len)
      positive_reviews = data[data['sentiment'] == 'positive']['review_length']
      negative_reviews = data[data['sentiment'] == 'negative']['review_length']
      f_statistic, p_value = f_oneway(positive_reviews, negative_reviews)
      print(f"F-statistic: {f_statistic}, P-value: {p_value}")
      
      contingency_table = pd.crosstab(data['sentiment'], data['review_length'] > data['review_length'].mean())
      chi2, p, dof, expected = chi2_contingency(contingency_table)
      print(f"Chi-squared Value: {chi2}, P-value: {p}")
  - step: Visualization
    description: |
      Visualized the sentiment distribution using bar and pie charts, 
      and review lengths using histogram and boxplot.
    code: |
      sentiment_ratio = data['sentiment'].value_counts(normalize=True) * 100
      sentiment_ratio.plot(kind='pie', autopct='%1.1f%%', colors=['blue', 'orange'], startangle=90)
      plt.title('Sentiment Ratio')
      plt.show()
      
      plt.figure(figsize=(10, 6))
      plt.hist(positive_reviews, bins=30, alpha=0.5, label='Positive Reviews', color='blue')
      plt.hist(negative_reviews, bins=30, alpha=0.5, label='Negative Reviews', color='orange')
      plt.xlabel('Review Length')
      plt.ylabel('Frequency')
      plt.title('Distribution of Review Lengths')
      plt.legend()
      plt.show()

results:
  - test: ANOVA Test
    results:
      f_statistic: 12.0557
      p_value: 0.000516
    conclusion: |
      There is a statistically significant difference between the lengths of positive and negative reviews.
  - test: Chi-Squared Test
    results:
      chi_squared_value: 2.4537
      p_value: 0.1172
    conclusion: |
      No statistically significant relationship was found between sentiment and review length.

visualizations:
  - chart_type: Bar Chart
    description: Sentiment distribution (positive vs negative).
  - chart_type: Pie Chart
    description: Sentiment proportions.
  - chart_type: Histogram
    description: Distribution of review lengths for positive and negative reviews.
  - chart_type: Boxplot
    description: Comparison of review lengths based on sentiment.

libraries_used:
  - name: pandas
    description: Data manipulation and analysis.
  - name: numpy
    description: Numerical computations.
  - name: matplotlib
    description: Data visualization.
  - name: seaborn
    description: Advanced data visualization.
  - name: scipy
    description: Statistical hypothesis testing (ANOVA, Chi-Squared).

conclusion_and_recommendations:
  conclusions:
    - Positive reviews tend to be longer, suggesting that users express their satisfaction in more detail.
    - Negative reviews are typically shorter, indicating that users prefer to keep their criticism brief.
  business_applications:
    - Tailor responses to positive and negative feedback accordingly.
    - Understand customer behavior to improve satisfaction and engagement.

project_links:
  kaggle_notebook: "KAGGLE_NOTEBOOK_LINK"
  github_repo: "GITHUB_REPO_LINK"

---

## **How to Run the Project**
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/imdb-sentiment-analysis.git
Navigate to the project folder:
cd imdb-sentiment-analysis
Install dependencies:
pip install -r requirements.txt
Open and run the Jupyter Notebook:
jupyter notebook IMDB_Sentiment_Analysis.ipynb

---

### **Açıklamalar:**
1. **KAGGLE_NOTEBOOK_LINK** ve **GITHUB_REPO_LINK** kısımlarını **projenizin Kaggle ve GitHub bağlantıları** ile değiştirmelisiniz.
2. **YAML** formatı, dosyaları daha organize bir biçimde saklamak için çok kullanışlıdır ancak genellikle konfigürasyon dosyalarında kullanılır. GitHub üzerinde görünüm açısından Markdown (`README.md`) daha yaygın olduğu için, bu dosya genellikle bu formatta kullanılır.
3. Yukarıdaki dosya GitHub'a yüklendikten sonra, projenizin dökümantasyonunu oldukça şeffaf ve detaylı bir şekilde gösterir.

---

### **Sonraki Adımlar:**
1. GitHub repository’nizi oluşturun ve bu dosyayı `.yml` formatında yükleyin.
2. İlgili bağlantıları (KAGGLE_NOTEBOOK_LINK, GITHUB_REPO_LINK) güncellemeyi unutmayın.

Herhangi bir sorunuz olursa, tekrar yardımcı olabilirim! 😊
