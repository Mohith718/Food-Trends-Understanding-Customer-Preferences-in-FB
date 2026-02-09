# 🍔 Food Brand Customer Trends Analysis

## 📊 Project Overview

This project analyzes customer feedback from multiple sources to uncover insights on customer satisfaction, product preferences, and emerging trends in the food & beverage industry. By integrating structured survey data and unstructured feedback from reviews and social media, this Power BI solution provides actionable insights for product development, R&D, and marketing teams.

### 🎯 Problem Statement

Customer feedback is a goldmine for innovation in the food industry. However, feedback data is scattered across surveys, social media platforms, and product reviews. This project centralizes and analyzes this data to generate meaningful insights that drive business decisions.

### ✨ Key Outcomes

- **Centralized Sentiment Analysis**: Unified view of customer sentiment across products and regions
- **Feature-Level Insights**: Visualization of most-liked and most-criticized product features
- **Trend Detection**: AI-powered keyword and theme detection from unstructured feedback
- **Customer Segmentation**: Behavioral clustering by satisfaction, frequency, and preferences
- **Regional Patterns**: Geographic analysis of preferences and complaints
- **Strategic Recommendations**: Data-driven insights for product innovation and marketing campaigns

---

## 📁 Dataset Information

This project utilizes two complementary datasets:

### 1. Structured Dataset (Surveys)
- **Source**: Customer satisfaction surveys
- **Format**: CSV/Structured tables
- **Key Fields**: 
  - User demographics (age, region, purchase channel)
  - Product ratings (taste, price, packaging, quality)
  - Satisfaction scores
  - Purchase frequency

### 2. Unstructured Dataset (Reviews & Social Media)
- **Source**: Product reviews, social media comments, customer feedback forms
- **Format**: Text data (CSV/JSON)
- **Key Fields**:
  - Review text/comments
  - Product mentions
  - Timestamp
  - User metadata
  - Platform source

Both datasets are available in the `/data` folder of this repository.

---

## 🏗️ Project Architecture

### Technology Stack

- **Data Visualization**: Microsoft Power BI
- **Data Transformation**: Power Query (M Language)
- **NLP & Sentiment Analysis**: Python (TextBlob/VADER/Transformers)
- **Data Modeling**: Star Schema with dimension and fact tables
- **Version Control**: Git/GitHub

### Data Pipeline

```
Data Sources (Surveys, Reviews, Social Media)
           ↓
Power Query Transformation & Cleaning
           ↓
Python NLP Processing (Sentiment Analysis)
           ↓
Semantic Data Model (Star Schema)
           ↓
Power BI Dashboards & Visualizations
```

### Data Model

- **Dimension Tables**: Customer, Product, Time, Location
- **Fact Tables**: Feedback, Sentiment Scores, Ratings
- **Unified Keys**: user_id, product_id, feedback_id, timestamp

---

## 📅 Implementation Timeline

### Week-wise Module Plan

| Week | Module | Deliverables | Status |
|------|--------|--------------|--------|
| 1-2  | Data Collection & Cleaning | Cleaned, standardized datasets with unified schema | 🔄 In Progress |
| 3-4  | Sentiment Analysis | NLP-based classification, sentiment visualizations | ⏳ Upcoming |
| 5-6  | Product Insights | Performance dashboards by feature/category | ⏳ Upcoming |
| 7-8  | Customer Segmentation | Behavioral personas and demographic analysis | ⏳ Upcoming |
| 9-10 | Strategy & Innovation Dashboard | Trend keywords, campaign impact analysis | ⏳ Upcoming |

### Milestones

- ✅ **Milestone 1 (Week 2)**: Data cleaning and validation complete
- ⏳ **Milestone 2 (Week 4)**: Sentiment analysis implementation
- ⏳ **Milestone 3 (Week 6)**: Product performance dashboards
- ⏳ **Milestone 4 (Week 8)**: Customer segmentation logic
- ⏳ **Milestone 5 (Week 10)**: Final strategy dashboard and documentation

---

## 🔧 Setup & Installation

### Prerequisites

- **Power BI Desktop** (Latest version)
- **Python 3.8+** (for sentiment analysis)
- **Required Python Libraries**:
  ```bash
  pip install pandas numpy nltk textblob vaderSentiment scikit-learn
  ```

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/food-trends-analysis.git
   cd food-trends-analysis
   ```

2. **Install Python dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Open Power BI file**
   - Navigate to `/power-bi` folder
   - Open `FoodTrends_Analysis.pbix`

4. **Configure data sources**
   - Update data source paths in Power Query
   - Refresh all data connections

---

## 📂 Repository Structure

```
food-trends-analysis/
│
├── data/
│   ├── structured/          # Survey data (CSV files)
│   ├── unstructured/        # Reviews and social media data
│   └── processed/           # Cleaned and transformed data
│
├── scripts/
│   ├── data_cleaning.py     # Data preprocessing scripts
│   ├── sentiment_analysis.py # NLP and sentiment scoring
│   └── customer_segmentation.py # Clustering algorithms
│
├── power-bi/
│   ├── FoodTrends_Analysis.pbix  # Main Power BI file
│   └── custom_visuals/      # Custom visual imports
│
├── documentation/
│   ├── data_dictionary.md   # Field descriptions
│   ├── architecture.png     # System architecture diagram
│   └── project_plan.pdf     # Detailed project documentation
│
├── results/
│   └── dashboard_screenshots/  # Output visualizations
│
├── README.md
└── requirements.txt         # Python dependencies
```

---

## 📈 Key Modules

### 1. Data Collection & Cleaning
- Import and merge multiple data sources
- Text normalization, tokenization, and deduplication
- Handle missing values and outliers
- Create unified schema with consistent keys

### 2. Sentiment Analysis
- AI/NLP classification (Positive, Neutral, Negative)
- Sentiment scoring per product, feature, and region
- DAX measures for sentiment trends over time
- Keyword extraction and theme detection

### 3. Product Insights
- Category-level performance comparison
- Feature analysis (taste, price, packaging, quality)
- Correlation between sentiment and sales
- Identify top-performing and underperforming products

### 4. Customer Segmentation
- Behavioral personas: "Loyal Fans", "Critics", "Silent Users"
- Clustering by rating frequency, sentiment, and preferences
- Demographic filters (region, age, purchase channel)
- RFM (Recency, Frequency, Monetary) analysis

### 5. Strategy & Innovation Dashboard
- Emerging trend identification
- Pre/post campaign sentiment tracking
- Opportunity areas for marketing and R&D
- Data-driven recommendations for product innovation

---

## 📊 Dashboard Preview

_Dashboard screenshots will be added upon completion of each milestone_

---

## 🔍 Key Insights (To be updated)

- Most liked product features
- Common customer complaints
- Regional preference patterns
- Emerging food trends
- Customer segment characteristics

---

## 🚀 Future Enhancements

- [ ] Real-time social media data integration via API
- [ ] Advanced NLP using transformer models (BERT, RoBERTa)
- [ ] Predictive analytics for trend forecasting
- [ ] Integration with CRM systems
- [ ] Automated report generation and distribution
- [ ] Multi-language sentiment analysis
- [ ] Image analysis from social media posts

---

## 📧 Contact

**Your Name**  
- LinkedIn: (https://www.linkedin.com/in/mohith-srinivas/)
- Email: smohith200@gmail.com

---

## 🙏 Acknowledgments

- Dataset sources: [Facebook, Food Survey]
- Inspiration: Customer-centric innovation in F&B industry
- Tools: Microsoft Power BI, Python, NLP

---

**Last Updated**: February 2026  
**Project Status**: 🔄 In Progress
