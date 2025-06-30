# Stock Recommendation System

## Overview

**Stock_Recommendation_System** is a scalable, near-real-time analytics pipeline that delivers intelligent stock recommendations by integrating:

- Real-time user feedback via Kafka  
- Historical stock data  
- Sentiment analysis from financial news articles  

This system leverages **K-Means Clustering** to segment both stocks and users based on behavioral, financial, and sentiment-based features, enabling group-specific recommendations. It is built using a big data architecture with **Apache Kafka**, **Spark**, **SQL + HDFS**, and deployed using **Docker** on **Ubuntu**.

---

## Tools & Technologies

### Programming Languages & Libraries

- **Python** – preprocessing, clustering, and end-to-end pipeline  
- **scikit-learn** – implementation of K-Means clustering  
- **Pandas, NumPy** – data manipulation and transformation  
- **Matplotlib, Seaborn** – data visualization  
- **NLTK / VaderSentiment** – sentiment analysis from financial news  

### Infrastructure & Storage

- **Apache Kafka** – real-time ingestion of user feedback (ratings, comments)  
- **Apache Spark** – distributed processing of structured/unstructured data  
- **MySQL / PostgreSQL** – structured data storage (stock metrics, user profiles)  
- **Hadoop HDFS** – unstructured data storage (financial articles, raw feedback)  
- **Docker** – containerization for portability and deployment  
- **Ubuntu (Linux)** – operating environment  

---

## Machine Learning Approach

### K-Means Clustering

- Grouped stocks based on shared patterns in volatility, pricing, and sentiment  
- Grouped users based on investment behaviors and feedback patterns  
- Cluster insights were used to deliver targeted recommendations  
- Helped align recommendations with user group risk profiles and preferences  

---

## Key Features

- **Real-Time Ingestion**: Kafka-based pipeline collects user feedback in real time  
- **Hybrid Storage Architecture**:  
  - SQL for structured data like stock fundamentals and user profiles  
  - HDFS for unstructured data like news articles and raw comments  
- **Distributed ETL**: Apache Spark jobs perform scalable data transformation and clustering  
- **Sentiment-Enhanced Scoring**: Extracted and quantified sentiment from 500+ financial news articles  
- **Unsupervised Learning**: Applied K-Means clustering to uncover market segments and user behavior groups  
- **Containerized Pipeline**: Fully modular system deployed using Docker for consistency and scalability  

---

## Output & Results

- **Stock Clustering**: Stocks segmented based on financial and sentiment metrics  
- **User Feedback Analysis**: Group-level recommendation strategies personalized to user clusters  
- **Visualization Dashboard**: Insights into cluster performance, sentiment trends, and user behavior patterns  
- **Outcome**: Improved relevance and accuracy of stock recommendations using risk-adjusted and sentiment-informed logic  
