# 🏙️ Segmenting and Clustering Neighborhoods in Toronto

![Toronto Neighborhoods](https://via.placeholder.com/1200x400?text=Toronto+Neighborhoods+Clustering)  

## 📌 Project Overview
This project analyzes and clusters neighborhoods in Toronto using **geospatial data** and **machine learning** to identify patterns in venue distribution. Originally developed for the IBM Data Science Professional Certificate, it demonstrates practical applications of k-means clustering for urban planning and business location analysis.

**Key Question:**  
*"How can we group Toronto neighborhoods based on their venue characteristics to identify similar areas for targeted services?"*

## 🛠️ Tools & Technologies
- **Data Sources:** 
  - Toronto neighborhood data (Wikipedia scraping)
  - Foursquare API (venue data)
- **Languages:** Python
- **Libraries:** 
  - Pandas, NumPy (data manipulation)
  - Scikit-learn (K-Means clustering)
  - Folium (geospatial visualization)
  - BeautifulSoup (web scraping)
- **Environment:** Jupyter Notebook

## 📂 Project Structure
**Segmenting-and-Clustering-Neighborhoods-in-Toronto/**
├── data/ # Raw and processed datasets
│ ├── toronto_neighborhoods.csv
│ └── foursquare_results.json
├── notebooks/ # Analysis workflow
│ ├── 1_Data_Collection.ipynb
│ ├── 2_Data_Preprocessing.ipynb
│ └── 3_Clustering_Visualization.ipynb
├── outputs/ # Generated maps/charts
├── README.md # This file
└── requirements.txt # Dependencies


## 🚀 Methodology
1. **Data Collection**:
   - Scraped neighborhood postal codes from Wikipedia
   - Enriched with latitude/longitude using Geocoder API
   - Collected top venues via Foursquare API

2. **Feature Engineering**:
   - One-hot encoded venue categories
   - Calculated mean venue frequency per neighborhood
   - Normalized features for clustering

3. **Clustering**:
   - Applied K-Means (optimized k using elbow method)
   - Validated with silhouette score

4. **Visualization**:
   - Interactive Folium maps with cluster layers
   - Bar charts of top venue categories per cluster

## 💡 Key Insights
- Identified **X distinct neighborhood types** (e.g., "Downtown Entertainment", "Suburban Family") 
- Discovered underserved areas for specific services (e.g., coffee shops in Cluster 3)
- High-density zones vs. residential clusters clearly visualized

## 🏆 Applications
This analysis can help:
- **Businesses** identify expansion opportunities
- **City planners** optimize service distribution
- **Real estate agents** characterize neighborhood profiles

## 🔧 How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/yawdap/Segmenting-and-Clustering-Neighborhoods-in-Toronto.git

## 🤝 Contributing
Contributions welcome! Please:

Open an issue to discuss changes
Fork the repository
Submit a pull request
