# 📊 Play Store Analytics Dashboard

An interactive data analytics project built using Python to analyze Google Play Store applications, ratings, reviews, installs, pricing, sentiment, revenue, and app performance.

The project contains **16 interactive visualizations**, including advanced analytical charts such as Hexbin, Sunburst, Calendar Heatmap, Streamgraph, Clustered Heatmap, and Radar charts.

---

## 🚀 Project Overview

The objective of this project is to analyze Google Play Store data and extract meaningful insights related to:

- 📱 App categories and types
- ⭐ App ratings
- 📥 App installs
- 💬 User reviews and sentiment
- 💰 App pricing and estimated revenue
- 📏 App size
- 🔄 App update activity
- 📈 Category performance
- 🧩 Free vs Paid applications
- 📊 Engagement and performance metrics

The final output is an interactive dashboard containing multiple Plotly visualizations.

---

## 🎯 Objectives

- Perform data cleaning and preprocessing using Python.
- Analyze application categories and app types.
- Study relationships between ratings, installs, reviews, and app size.
- Analyze user sentiment from reviews.
- Calculate estimated revenue and engagement metrics.
- Identify category-level trends and outliers.
- Apply statistical techniques such as:
  - IQR Outlier Detection
  - Z-Score Normalization
  - Percentile Normalization
  - Hierarchical Clustering
  - Rolling Averages
  - Rolling Z-Scores
- Build interactive visualizations using Plotly.
- Combine the visualizations into a web-based analytics dashboard.

---

## 📂 Dataset

The project uses two datasets:

### 1. Play Store Data

Contains information about applications available on the Google Play Store.

Important columns include:

- App
- Category
- Rating
- Reviews
- Size
- Installs
- Type
- Price
- Content Rating
- Genres
- Last Updated
- Android Version

### 2. User Reviews

Contains user review information used for sentiment analysis.

Important columns include:

- App
- Translated_Review
- Sentiment
- Sentiment_Polarity
- Sentiment_Subjectivity

---

## 🛠️ Technologies Used

### Programming & Analysis

- Python
- Pandas
- NumPy
- SciPy
- NLTK
- TextBlob

### Visualization

- Plotly
- HTML
- JavaScript
- CSS

### Development Environment

- Jupyter Notebook
- Anaconda
- VS Code

### Deployment

- Netlify
- GitHub

---

# 📊 Visualizations

The dashboard contains **16 interactive charts**.

## 1. Category Graph

Analyzes the distribution of applications across different Play Store categories.

## 2. Type Graph

Compares the distribution of Free and Paid applications.

## 3. Rating Graph

Shows the distribution of application ratings.

## 4. Sentiment Graph

Analyzes user review sentiment across positive, neutral, and negative reviews.

## 5. Category Rating Graph

Compares application ratings across different categories.

## 6. Updates Graph

Analyzes application update activity over time.

## 7. Revenue Graph

Analyzes estimated application revenue using price and install information.

## 8. Genre Graph

Examines the distribution of application genres.

## 9. Update Graph

Analyzes the relationship between application ratings and update activity.

## 10. Paid vs Free Graph

Compares rating and performance characteristics of Free and Paid applications.

---

# 🔬 Advanced Visualizations

## 11. Hexbin Size vs Rating

An interactive hexbin density visualization analyzing the relationship between:

- App Size
- Rating
- Average Installs

The visualization includes:

- Category filtering
- Rating and install thresholds
- Review filtering
- Sentiment subjectivity filtering
- IQR-based category outlier detection
- Marginal distributions
- Game apps highlighted in pink
- Translated category labels

### Availability

**5 PM – 7 PM IST**

---

## 12. Sunburst Installs & Rating

A hierarchical visualization using:

**Country → Category → App Type → Rating Band**

The visualization uses:

- Total installs for segment size
- Weighted average rating for colour
- Rating bands
- Drill-down interaction
- Parent contribution percentages
- High-install segment highlighting
- Custom hover information

### Availability

**6 PM – 8 PM IST**

---

## 13. Calendar Installs Heatmap

An interactive calendar-style visualization showing monthly installs for eligible app categories.

Features include:

- Category selector
- Monthly installs
- Month-over-month growth
- Three-month moving average
- Forecast values
- Growth >20% highlighting
- Actual vs forecast distinction
- Interactive hover information

### Availability

**6 PM – 9 PM IST**

---

## 14. Streamgraph

An interactive streamgraph analyzing category growth over time.

It includes:

- Monthly installs
- Cumulative installs
- Growth percentage
- Complete monthly timeline
- Missing-month handling
- 25% growth threshold
- Rolling Z-score anomaly detection
- Anomaly annotations
- Interactive metric selector

### Availability

**4 PM – 6 PM IST**

---

## 15. Clustered Heatmap

A performance comparison of the top 10 app categories across:

- Weighted Rating
- Total Reviews
- Total Installs
- Average Size
- Engagement Rate
- Update Frequency

The visualization uses:

- Z-score normalization
- Weighted composite scoring
- Hierarchical clustering
- Category ranking
- Top 3 / Bottom 3 annotations
- Raw vs normalized value selector

### Availability

**3 PM – 5 PM IST**

---

## 16. Free vs Paid Radar Chart

An interactive radar chart comparing Free and Paid applications across:

- Average Installs
- Weighted Rating
- Total Reviews
- Average Size
- Revenue
- Engagement Rate

The visualization includes:

- Percentile-based normalization
- Top 5 categories by installs
- Free vs Paid comparison
- Category selector
- Overall comparison
- Composite performance score
- Better-performing app type identification

### Availability

**1 PM – 2 PM IST**

---

# 🧹 Data Preprocessing

The project performs several preprocessing steps before analysis.

### Cleaning

- Missing ratings are removed.
- Missing values are handled.
- Duplicate applications are removed.
- Ratings above 5 are excluded.
- Installs are converted from strings to numeric values.
- Price values are converted to numeric values.
- Reviews are converted to numeric values.
- App sizes are converted into a consistent unit.
- Android version values are cleaned.
- Review text is cleaned before sentiment analysis.

### Feature Engineering

Additional analytical metrics are created, including:

- Revenue
- Engagement Rate
- Weighted Rating
- Sentiment Score
- Month-over-Month Growth
- Rolling Average
- Rolling Z-Score
- Composite Performance Score

---

# 📐 Statistical Techniques

The project applies several statistical methods.

### IQR Outlier Detection

Used to identify category-level outliers based on the Interquartile Range method.

### Z-Score Normalization

Used in the clustered heatmap to make different metrics comparable.

### Percentile Normalization

Used in the radar chart to normalize metrics across different scales.

### Hierarchical Clustering

Used to group categories according to similarity in their performance metrics.

### Rolling Statistics

Used to identify unusual changes in category growth over time.

---

# 🕐 Time-Based Dashboard Controls

The six advanced visualizations are intentionally displayed only during their specified IST windows.

| Visualization | Availability |
|---|---|
| Radar | 1 PM – 2 PM IST |
| Clustered Heatmap | 3 PM – 5 PM IST |
| Streamgraph | 4 PM – 6 PM IST |
| Hexbin | 5 PM – 7 PM IST |
| Sunburst | 6 PM – 8 PM IST |
| Calendar Heatmap | 6 PM – 9 PM IST |

The dashboard uses the **Asia/Kolkata timezone** so the restrictions are based on Indian Standard Time rather than the visitor's local timezone.

---

# 🌐 Interactive Dashboard

The final dashboard provides:

- Interactive Plotly charts
- Search functionality
- Category/topic filters
- Grid and list views
- Chart sorting
- Individual chart access
- Insights for each visualization
- Responsive design
- Dark/light mode
- Time-based visualization availability

---

# 📁 Project Structure

```text
PlayStore-Analytics/
│
├── index.html
│
├── Category_Graph_1.html
├── Type_Graph_2.html
├── Rating_Graph_3.html
├── Sentiment_Graph_4.html
├── Category_Graph_5.html
├── Updates_Graph_6.html
├── Revenue_Graph_7.html
├── Genre_Graph_8.html
├── Update_Graph_9.html
├── Paid Free Graph 10.html
│
├── Hexbin_Size_Rating_Graph_11.html

GitHub Repository:
https://github.com/indraneelbhattacharya19-hub/Google-Play-Store-_Analysis
├── Sunburst_Installs_Rating_Graph_12.html
├── Calendar_Installs_Heatmap_Graph_13.html
├── Streamgraph_Installs_Graph_14.html
├── Clustered_Heatmap_Graph_15.html
└── Radar_Free_Paid_Graph_16.html

Website link:
https://googleplaystoreproject.netlify.app
