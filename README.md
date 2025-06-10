# Ethiopian Banks Mobile Apps Review Analysis

# Overview

This repository contains scripts and documentation for analyzing user reviews of mobile banking apps for Commercial Bank of Ethiopia (CBE), Bank of Abyssinia (BOA), and Dashen Bank. The project includes web scraping, sentiment analysis, thematic analysis, database storage, and visualization of insights.

## Task 1: Data Collection and Preprocessing
**Objective**: Scrape 400+ reviews per bank from Google Play Store and preprocess the data.

**Methodology**:

Used google-play-scraper to collect reviews, ratings, dates, and app names.

Preprocessed data to remove duplicates, handle missing values, and normalize dates.

Saved cleaned data as data/bank_reviews.csv with columns: review_id, review, rating, date, bank, source.

## Task 2: Sentiment and Thematic Analysis 

Task 2 aimed to quantify the sentiment of user reviews and identify key themes to 
highlight satisfaction drivers and pain points for each bank’s mobile application. 

## Sentiment Analysis:
Use distilbert-base-uncased-finetuned-sst-2-english to compute sentiment scores (positive, negative, neutral). 
Aggregate by bank and rating (e.g., mean sentiment for 1-star reviews).

## Thematic Analysis:
A theme refers to a recurring concept or topic within user reviews. For this challenge, themes will help summarize user feedback into actionable categories for the banks.
##	Data Storage
The processed data was inserted into an Oracle database with two tables: Banks and Reviews. 

## Visualization
Visualizations were generated  with pandas, matplotlib, and seaborn. Key outputs included:
•	Sentiment Distribution by Bank: 
•	Rating Distribution by Bank:  
•	Keyword Clouds: 


## Conclusions
CBE leads in user satisfaction with a 4.4-star rating, driven by a user-friendly interface, but faces challenges with glitches and slow transfers. BOAs 2.8-star rating reflects urgent needs for stability and faster updates. Dashens 4.0-star rating benefits from Sharia- compliant features but requires improved transaction reliability. The analysis successfully identified key themes and provided actionable recommendations to enhance user retention, feature sets, and complaint management. Future work should resolve sentiment analysis pipeline issues, install the wordcloud module for visualizations, and explore advanced visualization techniques to improve stakeholder communication.




