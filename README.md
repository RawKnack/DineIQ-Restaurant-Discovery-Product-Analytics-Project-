# DineIQ — Restaurant Discovery & Product Analytics Case Study

## Overview

DineIQ is a product analytics and discovery case study inspired by restaurant marketplace challenges faced by dining platforms like Swiggy Dineout.

This project combines:

* Exploratory Data Analysis (EDA)
* SQL-based product analytics
* Product Requirement Documentation (PRD)
* Business insight generation

The goal was to identify high-quality but low-visibility restaurants ("Hidden Gems") and design a scalable product feature to improve restaurant discovery and booking conversion.

---

## Problem Statement

Restaurant discovery platforms often over-promote already popular restaurants, causing many high-quality restaurants to remain undiscovered.

Through analysis of the Bangalore restaurant dataset, this project identified hundreds of highly rated restaurants with very low visibility despite strong customer satisfaction.

### Core Insight

200+ restaurants in Bangalore had:

* Rating ≥ 4.0
* Low visibility (<200 votes)
* Table booking enabled

These restaurants represented an opportunity for:

* better user discovery
* increased booking conversion
* improved marketplace liquidity

---

## Project Structure

```text
DineIQ/
│
├── 1_EDA/
│   ├── Zomato_EDA.ipynb
│   ├── Product_Analytics_Using_SQL.ipynb
│   └── outputs/
│       ├── ratings_distribution.png
│       ├── cost_histogram.png
│       ├── cost_pie.png
│       ├── top_15_cuisines.png
│       └── final_5_insights.md
│
├── 2_PRD/
│   └── Hidden_Gems_PRD.md
│
└── README.md
```

---

## Tech Stack

* Python
* Pandas
* SQLite
* Matplotlib
* Jupyter Notebook
* SQL
* Notion-style PRD Documentation

---

## Exploratory Data Analysis (EDA)

The EDA focused on:

* restaurant distribution analysis
* ratings analysis
* booking behavior analysis
* cuisine trend analysis
* pricing segmentation
* hidden gem discovery

### Key Analyses

* Top restaurant locations in Bangalore
* Ratings distribution
* Online ordering behavior
* Table booking vs ratings correlation
* Cuisine popularity analysis
* Cost segmentation analysis

---

## SQL Product Analytics

SQLite was used to perform product-focused analytics queries.

### SQL Queries Implemented

1. Hidden gems by location
2. Table booking vs ratings analysis
3. Price segment distribution
4. Top cuisines among hidden gems
5. Best locations for booking expansion

### Example Product Questions Solved

* Which areas have the highest concentration of hidden gems?
* Do booking-enabled restaurants perform better?
* Which cuisine categories are under-discovered?
* Which regions are ideal for Dineout expansion?

---

## Product Feature Proposal — Hidden Gems

A product proposal was designed for Swiggy Dineout.

### Feature Concept

A curated discovery section highlighting underrated but highly rated restaurants.

### Eligibility Criteria

* Rating ≥ 4.0
* Votes < 200
* Table booking enabled
* Hygiene score ≥ 4.0

### PRD Includes

* Problem statement
* User personas
* User stories
* Success metrics
* Rollout strategy
* Edge cases
* Launch phases

---

## Key Product Insights

### Insight 1

Highly rated restaurants often suffer from visibility imbalance despite strong customer satisfaction.

### Insight 2

Restaurants with table booking enabled showed stronger engagement patterns.

### Insight 3

Specific Bangalore micro-markets contain dense clusters of hidden gems.

### Insight 4

Mid-range pricing dominates the restaurant distribution landscape.

### Insight 5

Several cuisine categories remain under-discovered despite strong ratings.

---

## Business Impact

This project demonstrates how product analytics can help:

* improve restaurant discovery
* increase booking conversion
* balance marketplace exposure
* improve user satisfaction
* support growth strategy decisions

---

## Resume Highlights

* Built SQL-driven product analytics workflows using SQLite and Python
* Identified 200+ high-quality low-visibility restaurants through data analysis
* Designed a product proposal with PRD documentation and rollout strategy
* Connected business insights with product decision-making

---

## Dataset

Dataset used:
Bangalore Zomato Restaurants Dataset (Kaggle)

Note:
Large raw dataset files are excluded from this repository due to GitHub size limitations.

---

## Future Improvements

* Recommendation ranking model
* Personalized discovery engine
* A/B testing simulation for feature rollout
* Restaurant scoring system
* Interactive dashboard

---

## Author

Raunak Suman

Product Analytics | Data Analysis | Product Thinking
