# Steam_Market_Analysis_BigData

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Databricks](https://img.shields.io/badge/Platform-Databricks-orange?logo=databricks)
![Big Data](https://img.shields.io/badge/Big--Data-PySpark--Ready-red)
![ML](https://img.shields.io/badge/ML-Unsupervised-blueviolet)

## 📌 Project Overview
As part of my Data Science training, I conducted a comprehensive analysis of the Steam platform on behalf of **Ubisoft**. The objective was to decipher the factors influencing game popularity and to identify current trends in the global video game market to support the launch of a new title.

## 🎯 Key Objectives
* **Macro Analysis:** Identify top publishers, release trends (including COVID-19 impact), and price distribution.
* **Genre Insights:** Evaluate the most represented genres vs. those with the highest user satisfaction.
* **Platform Reach:** Compare market share between Windows, Mac, and Linux.
* **Strategic Correlations:** Understand the relationship between pricing tiers and quality scores.

## 🛠️ Technical Challenges & Big Data Solutions
This project involved processing real-world "dirty" data from a semi-structured JSON source (AWS S3):
* **Schema Flattening:** Navigated and extracted data from deeply nested JSON structures using PySpark's `select` and `alias`.
* **Regex Cleaning:** Implemented Regular Expressions to normalize messy age ratings (e.g., converting "MA 15+" or "21+" into standardized PEGI categories).
* **Data Transformation:** Managed currency conversion (cents to euros) and parsed heterogeneous date formats using `try_cast` and `to_date`.
* **Relational Mapping:** Used `explode()` and `split()` to handle many-to-many relationships for games with multiple genres and languages.

## 📊 Strategic Insights
* **Market Dynamics:** Observed a significant surge in game releases during the COVID-19 period, highlighting increased market saturation.
* **Pricing Strategy:** Mapped the "Premium" niche (>60€), revealing high consumer expectations for quality in this segment
