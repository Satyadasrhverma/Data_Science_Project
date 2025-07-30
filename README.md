# Zomato Restaurants Dataset

**Source**: Zomato Restaurants Data by ShrutiMehta on Kaggle  
https://www.kaggle.com/datasets/shrutimehta/zomato-restaurants-data

---

## 🚩 Dataset Overview

- Collected from Zomato’s public API as JSON files; converted into a CSV (zomato.csv) :contentReference[oaicite:1]{index=1}  
- Contains over 10,000 restaurants across 15 countries: India, United States, UK, UAE, Canada, Australia, Singapore, Philippines, Brazil, Indonesia, New Zealand, Qatar, South Africa, Sri Lanka, Turkey :contentReference[oaicite:2]{index=2}

---

## 🧾 Columns Description

| Column                | Description |
|-----------------------|-------------|
| Restaurant ID         | Unique identifier |
| Restaurant Name       | Name of restaurant |
| Country Code          | Numeric country code |
| City                  | City name |
| Address               | Full address |
| Locality              | Neighborhood/area |
| Locality Verbose      | Detailed locality description |
| Longitude / Latitude  | Geo‑coordinates |
| Cuisines              | Cuisine types offered |
| Average Cost for Two  | Estimated cost for two people |
| Currency              | Currency symbol (varies by country) |
| Has Table Booking     | ‘Yes’/’No’ |
| Has Online Delivery   | ‘Yes’/’No’ |
| Is Delivering         | ‘Yes’/’No’ (whether currently delivering) |
| Switch to Order Menu  | ‘Yes’/’No’ |
| Price Range           | 1–4 scale (affordability) |
| Aggregate Rating      | Average review rating (out of 5) |
| Rating Color          | Color code mapping to rating |
| Rating Text           | Text label (Poor, Average, etc.) |
| Votes                 | Number of reviews/votes :contentReference[oaicite:3]{index=3}

---

## 📦 How to Use

1. Download `zomato.csv` from the Kaggle link.
2. Load into your preferred environment (e.g. Pandas, SQL).
3. Inspect & clean (e.g. handle missing cuisines, unify country codes).
4. Use columns to filter, visualize, and analyze:
   - Cuisine trends by city
   - Cost vs rating relationships
   - Delivery/table‑booking availability
   - Geospatial mapping of restaurants using lat/long

---

## 📊 Common Analysis Ideas

- Country and city distribution of restaurants
- Rating categorization:  
  - 0 → White (“Not rated”)  
  - 1.8–2.4 → Red (“Poor”)  
  - 2.5–3.4 → Orange (“Average”)  
  - 3.5–3.9 → Yellow (“Good”)  
  - 4.0–4.4 → Green (“Very Good”)  
  - 4.5–4.9 → Dark Green (“Excellent”) :contentReference[oaicite:4]{index=4}
- Share of restaurants with online delivery or table booking
- Correlation between cost, votes, and ratings
- Identify top cuisines or most reviewed restaurants in major cities

---

## 🛠 Example Workflows

- **Data cleaning**: fill missing values in cuisines, standardize country/currency.
- **Aggregation**: group restaurants by city or cuisine to rank by cost, rating, or votes.
- **Visualization**: bar charts, treemaps, scatter plots (e.g. cost vs rating), and maps using latitude/longitude.
- **Modeling**: e.g., predict whether a restaurant’s rating > 4 based on features like cuisine, cost, online delivery, etc.

---

## ⚠️ Limitations & Considerations

- Dataset is skewed heavily toward Indian cities (especially Delhi/New Delhi, Gurgaon, Noida) :contentReference[oaicite:5]{index=5}
- Many restaurants lack ratings (`Aggregate Rating = 0`)
- No time component—ratings/votes are aggregate to the snapshot time
- Currency and cost values are not normalized across countries

---

## ✅ Repository Structure (suggested)

├── data/
│ └── zomato.csv
├── notebooks/
│ └── EDA_and_visualization.ipynb
├── src/
│ └── data_cleaning.py
└── README.md

yaml
Copy
Edit

---

## 🔗 Link to Dataset

Zomato Restaurants Data by ShrutiMehta on Kaggle:  
https://www.kaggle.com/datasets/shrutimehta/zomato-restaurants-data
# Data_Science_Project
