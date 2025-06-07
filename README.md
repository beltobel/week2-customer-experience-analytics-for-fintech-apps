# Ethiopian Banks Mobile Apps Review Analysis

# Overview

This repository contains scripts and documentation for analyzing user reviews of mobile banking apps for Commercial Bank of Ethiopia (CBE), Bank of Abyssinia (BOA), and Dashen Bank. The project includes web scraping, sentiment analysis, thematic analysis, database storage, and visualization of insights.

## Task 1: Data Collection and Preprocessing
**Objective**: Scrape 400+ reviews per bank from Google Play Store and preprocess the data.

**Methodology**:

Used google-play-scraper to collect reviews, ratings, dates, and app names.

Preprocessed data to remove duplicates, handle missing values, and normalize dates.

Saved cleaned data as data/bank_reviews.csv with columns: review_id, review, rating, date, bank, source.