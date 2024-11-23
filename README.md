# GlobalAIHub_VeriAnalizi


# IMDB Movie Reviews Sentiment Analysis

## 📘 Project Overview:
This project performs sentiment analysis on the **IMDB Dataset of 50K Movie Reviews** using statistical tests and visualizations to analyze positive and negative sentiments. The analysis includes **Exploratory Data Analysis (EDA)**, **Data Preprocessing**, and **Hypothesis Testing**.

---

## 📊 Dataset Information:
- **Source:** Kaggle
- **Rows:** 50,000
- **Columns:**
  - **review:** Text of the movie review
  - **sentiment:** Label indicating whether the review is positive or negative

### Preview:
The first 5 rows of the dataset:
```plaintext
| review                                    | sentiment |
|-------------------------------------------|-----------|
| One of the other reviewers has mentioned... | positive  |
| A wonderful little production...           | positive  |
| I thought this was a wonderful way to...   | positive  |
| Basically there's a family where...        | negative  |
| Petter Mattei's 'Love in the Time of Money' | positive  |
🔍 Steps and Analysis:

1. Dataset Loading and Exploration:
Loaded the dataset from Kaggle and previewed the first 5 rows.
Columns and data types were checked.
2. Exploratory Data Analysis (EDA):
Sentiment Distribution:
Positive: 50%
Negative: 50%
Visualized sentiment distribution using Bar Chart and Pie Chart.
3. Data Cleaning and Preprocessing:
Checked for missing data, and filled any missing reviews with 'No Review'.
Created a new numeric feature: review_length to represent the length of each review.
📊 Statistical Analysis:

4.1 ANOVA Test:
Hypothesis: Do positive and negative reviews differ significantly in length?
Results:
F-statistic: 12.0557
P-value: 0.000516
Conclusion: There is a statistically significant difference between positive and negative review lengths.
4.2 Chi-Squared Test:
Hypothesis: Is there a relationship between sentiment and review length?
Results:
Chi-squared value: 2.4537
P-value: 0.1172
Conclusion: No significant relationship was found between sentiment and review length.
📈 Visualizations:

Sentiment Distribution (Bar Chart):
A visual comparison of positive and negative reviews.
Sentiment Proportions (Pie Chart):
Displaying the percentage split between positive and negative reviews.
Review Length Distribution (Histogram):
Visualizing the distribution of review lengths for positive and negative sentiments.
Review Length by Sentiment (Boxplot):
Comparing review lengths based on sentiment.
🧑‍💻 Libraries Used:

Pandas: For data analysis and manipulation.
NumPy: For numerical computations.
Matplotlib & Seaborn: For data visualization.
SciPy: For statistical analysis (ANOVA, Chi-Squared).
🔍 Results and Insights:

Positive Reviews: Tend to be longer, suggesting users express satisfaction in more detail.
Negative Reviews: Tend to be shorter, indicating that criticism is more concise.
Business Applications:
Tailor responses to customer feedback.
Use sentiment and length insights to improve customer satisfaction.
💻 How to Run the Project:

Step 1: Clone the Repository
git clone https://github.com/YOUR_USERNAME/imdb-sentiment-analysis.git
Step 2: Navigate to the Project Folder
cd imdb-sentiment-analysis
Step 3: Install Dependencies
pip install -r requirements.txt
Step 4: Open and Run the Jupyter Notebook
jupyter notebook IMDB_Sentiment_Analysis.ipynb
🌐 Project Links:

Kaggle Notebook: IMDB Sentiment Analysis on Kaggle
GitHub Repository: GitHub Repo
Turkish Translation (Türkçe)

📘 Proje Özeti:
Bu proje, IMDB Dataset of 50K Movie Reviews veri seti kullanılarak pozitif ve negatif sentiment analizini gerçekleştirmektedir. Analiz, Keşifsel Veri Analizi (EDA), Veri Ön İşleme ve Hipotez Testleri içermektedir.

📊 Veri Seti Bilgisi:

Kaynak: Kaggle
Satır Sayısı: 50,000
Sütunlar:
review: Yorum metni
sentiment: Yorumun pozitif veya negatif olduğunu belirten etiket
Önizleme:
Veri setinin ilk 5 satırı:

| review                                    | sentiment |
|-------------------------------------------|-----------|
| One of the other reviewers has mentioned... | positive  |
| A wonderful little production...           | positive  |
| I thought this was a wonderful way to...   | positive  |
| Basically there's a family where...        | negative  |
| Petter Mattei's 'Love in the Time of Money' | positive  |
🔍 Adımlar ve Analizler:

1. Veri Yükleme ve Keşif:
Veri seti Kaggle'dan yüklendi ve ilk 5 satır önizlendi.
Sütunlar ve veri türleri kontrol edildi.
2. Keşifsel Veri Analizi (EDA):
Sentiment Dağılımı:
Pozitif: %50
Negatif: %50
Çubuk ve Pasta Grafiği ile görselleştirildi.
3. Veri Temizleme ve Ön İşleme:
Eksik veri kontrolü yapıldı, eksik veri bulunmadı.
Veri türleri kontrol edilerek bir sayısal özellik (review_length) eklendi.
📊 İstatistiksel Analiz:

4.1 ANOVA Testi:
Hipotez: Pozitif ve negatif yorum uzunlukları farklı mı?
Sonuçlar:
F-statistic: 12.0557
P-value: 0.000516
Sonuç: Pozitif ve negatif yorum uzunlukları arasında anlamlı bir fark bulunmaktadır.
4.2 Chi-Squared Testi:
Hipotez: Sentiment ve yorum uzunluğu arasında ilişki var mı?
Sonuçlar:
Chi-squared Değeri: 2.4537
P-value: 0.1172
Sonuç: Anlamlı bir ilişki bulunmamaktadır.
📈 Görselleştirmeler:

Sentiment Dağılımı (Çubuk Grafiği):
Pozitif ve negatif yorumların görsel karşılaştırması.
Sentiment Oranları (Pasta Grafiği):
Pozitif ve negatif yorum oranlarını gösteren pasta grafiği.
Yorum Uzunluğu Dağılımı (Histogram):
Pozitif ve negatif yorumların uzunluk dağılımı.
Sentiment Bazında Yorum Uzunluğu (Boxplot):
Yorum uzunluklarını sentiment bazında karşılaştırma.
🧑‍💻 Kullanılan Kütüphaneler:

Pandas: Veri analizi ve manipülasyonu.
NumPy: Sayısal hesaplamalar.
Matplotlib & Seaborn: Görselleştirme.
SciPy: İstatistiksel analizler (ANOVA, Chi-Squared).
🔍 Sonuçlar ve Öneriler:

Pozitif Yorumlar: Genellikle daha uzun olup, kullanıcılar memnuniyetlerini daha detaylı ifade etmektedir.
Negatif Yorumlar: Daha kısa olup, kullanıcılar eleştirilerini daha özlü tutmaktadır.
İşletme Uygulamaları:
Müşteri geri bildirimlerine özel yanıtlar geliştirilmesi.
Memnuniyet ve katılım stratejilerini geliştirmek için kullanılabilir.
💻 Projeyi Çalıştırmak İçin:

Repository'i klonlayın:
git clone https://github.com/YOUR_USERNAME/imdb-sentiment-analysis.git
Proje klasörüne gidin:
cd imdb-sentiment-analysis
Gerekli bağımlılıkları yükleyin:
pip install -r requirements.txt
Jupyter Notebook'u açın ve çalıştırın:
jupyter notebook IMDB_Sentiment_Analysis.ipynb
🌐 Proje Bağlantıları:

Kaggle Notebook Linki: IMDB Sentiment Analysis on Kaggle
GitHub Repo Linki: GitHub Repo
Açıklamalar:
KAGGLE_NOTEBOOK_LINK ve GITHUB_REPO_LINK kısımlarını doğru bağlantılarla değiştirdiğinizden emin olun.
YAML formatında veri depolama ve proje sunma işlemleri, özellikle konfigürasyon dosyalarında yaygın olsa da, GitHub üzerinde Markdown (README.md) dosyasının daha yaygın kullanıldığını unutmayın.


### **Sonraki Adımlar:**
1. GitHub repository’nizi oluşturun ve bu dosyayı `.yml` formatında yükleyin.
2. İlgili bağlantıları (KAGGLE_NOTEBOOK_LINK, GITHUB_REPO_LINK) güncellemeyi unutmayın.

Herhangi bir sorunuz olursa, tekrar yardımcı olabilirim! 😊
