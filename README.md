# Netflix-Content-Strategy-From-Data-to-Decisions
Netflix Data Analysis &amp; Recommendation System
Netflix Data Analysis & Recommendation System
🚀 Project Overview

This repository showcases a complete Data Science workflow on Netflix’s content library, analyzing 8,807 movies and TV shows. The project demonstrates data cleaning, feature engineering, exploratory analysis, clustering, predictive modeling, and a content-based recommendation system.

Objectives:

Understand Netflix content trends over the years

Predict whether a title is a Movie or TV Show

Cluster content based on key features (release year, duration, content age)

Build a recommendation system using content descriptions

📊 Dataset

Source: Kaggle – Netflix Movies and TV Shows

Entries: 8,807

Columns: 12

Column	Description
show_id	Unique ID for each movie/TV show
type	Movie or TV Show
title	Content title
director	Director(s)
cast	Main actors
country	Production country
date_added	Date added on Netflix
release_year	Original release year
rating	Age/TV rating
duration	Minutes (Movies) / Number of seasons (TV Shows)
listed_in	Genres/categories
description	Content synopsis
🛠 Project Workflow
1️⃣ Data Cleaning & Feature Engineering

Convert date_added to datetime and extract year_added and month_added

Handle missing values in director, cast, country, rating, duration

Extract numeric values from duration into duration_int

Compute content_age_when_added = year_added - release_year

Encode type as binary (is_movie) for modeling

Outcome: Clean dataset ready for analysis and machine learning.

2️⃣ Exploratory Data Analysis (EDA)

Content Growth: TV Shows grew faster than Movies after 2016

Content Age: Most added content is recent

Rating Trends: Mature content (TV-MA, TV-14) is increasing over time

Clustering: Identified 4 clusters using KMeans based on release year, duration, and content age

Tools: Plotly for interactive visualizations

3️⃣ Machine Learning

Objective: Predict content type (Movie vs TV Show)

Features: release_year, duration_int, content_age_when_added

Models: Logistic Regression & Random Forest

Results: Random Forest achieved high accuracy; most important features: duration and release_year

4️⃣ Recommendation System

Method: TF-IDF vectorization of description column

Similarity Metric: Cosine similarity

Interactive Widget: Users can input a title and get top 5 similar content recommendations

Outcome: Personalized and interactive content suggestions

🧰 Technologies & Libraries

Python 3.x

Pandas, NumPy

Scikit-learn (ML, preprocessing, clustering)

Plotly (interactive visualizations)

Ipywidgets (recommendation system)

⚡ Usage

Clone the repository:

git clone <repository-url>

Install dependencies:

pip install pandas numpy scikit-learn plotly ipywidgets

Open the Jupyter Notebook to run EDA, ML, clustering, and recommendations

💡 Key Insights

Netflix content library grew significantly after 2016, especially TV Shows

Most added content is recent; older classics are rare

Age ratings indicate increased focus on mature audiences (TV-MA, TV-14)

Clustering shows patterns based on content age and duration

Recommendation system gives relevant content suggestions based on description similarity

✅ Conclusion

This project demonstrates an end-to-end Data Science workflow, including cleaning, visualization, predictive modeling, clustering, and building a recommendation system. It is GitHub-ready and portfolio-ready, ideal for showcasing your data analysis and machine learning skills.
