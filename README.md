# SpotifyDataAnalysisForecasting

## Authors  
Matheus Nogueira  
Anna Carolina Fonseca  
Guilherme Bizzo  
Roberto Mario L T L  

📧 Contact: matnogueira@gmail.com

## About this Project

This project was developed as part of the final assignment for the course **INF1032 – Introduction to Data Science** at PUC-Rio. It explores the characteristics of popular songs using Spotify data and applies predictive modeling to estimate a track's likelihood of entering the Top 200 charts and the number of streams it may receive.

The dataset was constructed using Spotify’s Web API and Spotify Charts (Top 200) across multiple countries. The project includes both **descriptive analytics** and **predictive modeling**.

## Key Insights and Objectives

### Descriptive Analysis
- Compared audio features of top-charting songs across different regions (Global, Brazil, USA, India, Mexico, Germany).
- Tracked the evolution of musical characteristics over time.
- Assessed the prevalence of native-language songs in national Top 200 rankings.
- Identified potentially anomalous songs using an ensemble of outlier detection models.
- Investigated which song attributes most influence popularity.

### Predictive Modeling

1. **Classification**
   - Predict whether a song will enter the Global Top 200 based on its features and metadata.
   - Models used: Logistic Regression and Random Forest.
   - Variants explored:
     - With/without artist-related features
     - PCA with 5 components
     - Filtering out anomalies
   - Best result (Random Forest with anomaly filtering):
     - Accuracy: 0.90  
     - Precision: 0.91  
     - Recall: 0.92  

2. **Regression**
   - Predict the number of streams a song will receive based on its characteristics.
   - Models: Linear Regression and Random Forest Regression.
   - Tested using raw features and PCA-transformed data.

### Anomaly Detection Ensemble
- Combined results from ABOD, Autoencoders, Isolation Forest, and Local Outlier Factor.
- Final anomaly labels obtained via weighted averaging of model outputs.
- Helped interpret outliers and refine datasets for predictive models.

## Notes

- Code was developed using Google Colab, with file paths linked to shared Google Drive directories. Execution outside that environment may require adjustments.
- Data collection and model tuning steps (e.g., Spotify API queries, grid search) may require significant runtime.
- This repository includes only work related to the second half of the course (G2).

## Academic Integrity Notice

This repository is shared strictly for academic transparency and educational purposes.  
**Reusing, copying, or submitting any part of this work for academic credit is strictly prohibited.**  
All work was completed independently and published after the course was finalized.
