# IMDB Movie Reviews Sentiment Analysis

This project analyzes the **IMDB Dataset of 50K Movie Reviews** using statistical methods and visualizations to explore the differences between positive and negative sentiments. The analysis includes **Exploratory Data Analysis (EDA)**, **Data Preprocessing**, **Hypothesis Testing**, and **Visualization**.

## Project Details:
- **Dataset:** IMDB Movie Reviews Dataset from Kaggle
- **Objective:** To perform sentiment analysis on movie reviews and compare positive and negative sentiments based on review length using statistical tests such as ANOVA and Chi-Squared.

### Key Steps in the Project:
1. **Dataset Loading and Exploration**
   - Load the IMDB movie reviews dataset from Kaggle.
   - Preview the first few rows and inspect the structure.
   
2. **Exploratory Data Analysis (EDA)**
   - Analyze the sentiment distribution of the reviews (positive vs negative).
   - Visualize the data using bar and pie charts.
   
3. **Data Cleaning and Preprocessing**
   - Check for missing data and fill missing reviews with 'No Review'.
   - Create a new feature `review_length` to represent the length of each review.
   
4. **Statistical Analysis**
   - Perform **ANOVA** test to compare the length of positive and negative reviews.
   - Perform **Chi-Squared** test to examine the relationship between sentiment and review length.
   
5. **Visualization**
   - Visualize sentiment distribution, review length distribution, and sentiment-based review length comparison using **bar charts**, **pie charts**, **histograms**, and **boxplots**.

---

## Results and Insights:
- **Positive Reviews** tend to be longer, indicating more detailed expressions of satisfaction.
- **Negative Reviews** are typically shorter, suggesting that criticism is more concise.
- **Business Application:**
  - This analysis can be used to understand user feedback better and tailor responses to positive and negative sentiments accordingly.

---

## Libraries Used:
- **Pandas:** Data manipulation and analysis.
- **NumPy:** Numerical computations.
- **Matplotlib & Seaborn:** Data visualizations.
- **SciPy:** Statistical analysis (ANOVA, Chi-Squared).

---

## How to Run the Project:
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


---

### 2. **Türkçe README.md**

```markdown
# IMDB Film Yorumları Sentiment Analizi

Bu proje, **IMDB Dataset of 50K Movie Reviews** veri setini kullanarak pozitif ve negatif sentiment analizini gerçekleştirmektedir. Analiz, **Keşifsel Veri Analizi (EDA)**, **Veri Ön İşleme**, **Hipotez Testleri** ve **Görselleştirme** içermektedir.

## Proje Detayları:
- **Veri Seti:** Kaggle'dan alınan IMDB Film Yorumları veri seti
- **Amaç:** Film yorumlarındaki sentiment (duygu) analizi yapılmış, pozitif ve negatif yorumların uzunlukları ANOVA ve Chi-Squared testleri kullanılarak karşılaştırılmıştır.

### Projeye Genel Bakış:
1. **Veri Yükleme ve Keşif**
   - Kaggle'dan IMDB film yorumları veri seti yüklendi.
   - İlk birkaç satır önizlendi ve veri yapısı incelendi.
   
2. **Keşifsel Veri Analizi (EDA)**
   - **Sentiment Dağılımı:** 
     - Pozitif: %50 
     - Negatif: %50
   - Çubuk ve Pasta Grafiği ile görselleştirildi.

3. **Veri Temizleme ve Ön İşleme**
   - Eksik veri kontrolü yapıldı, eksik veri bulunmadı.
   - Veri türleri kontrol edilerek bir sayısal özellik (`review_length`) eklendi.

4. **İstatistiksel Analiz**
   - **ANOVA** testi kullanılarak pozitif ve negatif yorumların uzunlukları karşılaştırıldı.
   - **Chi-Squared** testi ile sentiment ve yorum uzunluğu arasındaki ilişki incelendi.
   
5. **Görselleştirme**
   - Sentiment dağılımı, yorum uzunluğu dağılımı ve sentiment bazında yorum uzunluğu karşılaştırması için **çubuk grafikleri**, **pasta grafikleri**, **histogramlar** ve **boxplotlar** oluşturuldu.

---

## Sonuçlar ve Öneriler:
- **Pozitif Yorumlar** genellikle daha uzun olup, kullanıcılar memnuniyetlerini daha detaylı ifade etmektedir.
- **Negatif Yorumlar** daha kısa olup, kullanıcılar eleştirilerini daha özlü tutmaktadır.
- **İşletme Uygulamaları:**
  - Müşteri geri bildirimlerine özel yanıtlar geliştirilmesi.
  - Müşteri memnuniyetini arttırmaya yönelik stratejiler oluşturulabilir.

---

## Kullanılan Kütüphaneler:
- **Pandas:** Veri manipülasyonu ve analizi.
- **NumPy:** Sayısal hesaplamalar.
- **Matplotlib & Seaborn:** Görselleştirme.
- **SciPy:** İstatistiksel analizler (ANOVA, Chi-Squared).

---

## Projeyi Çalıştırmak İçin:
1. Repository'i klonlayın:
   ```bash
   git clone https://github.com/MKaaNa/GlobalAIHub_VeriAnalizi.git
Proje klasörüne gidin:
cd GlobalAIHub_VeriAnalizi
Gerekli bağımlılıkları yükleyin:
pip install -r requirements.txt
Jupyter Notebook'u açın ve çalıştırın:
jupyter notebook IMDB_Sentiment_Analysis.ipynb

