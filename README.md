# Airbnb-London-Weekdays-Analysis.
This project is a **beginner-friendly exploratory data analysis (EDA)** of the **Airbnb London (Weekdays) dataset**.   The dataset contains listings with details such as price, room type, host status, guest ratings, capacity, and location.    The goal is to uncover **business insights** and practice **data visualization** using Python.



---

## 📂 Dataset Columns

- `realSum` → Total price of stay  
- `room_type` → Type of listing (Entire home, Private room, etc.)  
- `room_shared` → Shared room (1 = yes, 0 = no)  
- `room_private` → Private room (1 = yes, 0 = no)  
- `person_capacity` → Number of people a listing can host  
- `host_is_superhost` → 1 = Superhost, 0 = Not superhost  
- `multi` → Host with multiple listings  
- `biz` → Business listing flag  
- `cleanliness_rating` → Cleanliness review rating (1–10)  
- `guest_satisfaction_overall` → Overall guest satisfaction score  
- `bedrooms` → Number of bedrooms  
- `dist` → Distance from city center  
- `metro_dist` → Distance from nearest metro station  
- `attr_index` → Attraction index of location  
- `rest_index` → Restaurant density index  
- `lng`, `lat` → Geographical coordinates  

---

## 🔹 A. Room & Host Analysis

- **Listings by room type**
  - Counted number of listings in each `room_type`.
  - Found % share of each room type (Entire home, Private room, Shared room).
- **Superhosts distribution**
  - Compared proportion of superhosts across different room types.
  - Observed which room type has more superhosts.

---

## 🔹 B. Pricing Insights

- **Basic price statistics**
  - Calculated mean, min, max, and distribution of `realSum` (total price).
  - Found that price data is skewed due to very expensive listings.
- **Room type vs price**
  - Average price calculated for each `room_type`.
  - Entire homes are the most expensive, private/shared rooms are cheaper.
- **Superhosts vs price**
  - Compared average price charged by superhosts vs non-superhosts.
- **Visualizations**
  - Histogram of price distribution.
  - Boxplots of price vs room type.
  - Boxplot of price vs superhost status.

---

## 🔹 C. Guest & Cleanliness Ratings

- **Overall ratings**
  - Summary of `guest_satisfaction_overall` and `cleanliness_rating`.
- **Room type vs satisfaction**
  - Compared average guest satisfaction score across room types.
- **Cleanliness correlation**
  - Measured correlation between cleanliness and guest satisfaction.
  - Found a positive relationship (cleaner = happier guests).
- **Superhosts vs satisfaction**
  - Checked if superhosts consistently receive higher guest ratings.
- **Visualizations**
  - Scatterplot: Cleanliness rating vs Guest satisfaction.
  - Boxplot: Guest satisfaction by room type.

---

## 🔹 D. Capacity & Bedrooms

- **Basic stats**
  - Analyzed `person_capacity` and `bedrooms` distribution.
- **Capacity vs price**
  - Larger capacity listings are more expensive on average.
- **Capacity vs satisfaction**
  - Checked if smaller/larger groups are more satisfied.
- **Bedrooms vs satisfaction**
  - Compared average guest satisfaction by number of bedrooms.
- **Visualizations**
  - Boxplot: Price vs person capacity.
  - Boxplot: Guest satisfaction vs bedrooms.

---

## 🔹 E. Location Analysis

- **Distance from city center**
  - Found relationship between `dist` (distance to center) and `realSum`.
  - Closer to city center → higher price.
- **Metro accessibility**
  - Analyzed `metro_dist` vs price → closer to metro = higher price.
- **Attraction index**
  - Checked `attr_index` vs guest satisfaction → better attraction areas = happier guests.
- **Restaurant index**
  - Explored `rest_index` vs guest satisfaction → more restaurants nearby = better reviews.
- **Visualizations**
  - Scatterplots: Price vs city distance, Price vs metro distance.
  - Scatterplot: Attractions index vs satisfaction.
  - Correlation heatmap for location, price, and satisfaction.

---

## 📊 Tools & Libraries

- **Python**
- **Pandas** → Data cleaning & analysis  
- **Matplotlib & Seaborn** → Data visualization  

---

## 📌 Key Insights

- Most listings are **private rooms**.  
- **Entire homes** are the most expensive category.  
- **Superhosts** generally provide better satisfaction scores.  
- Prices are **skewed** with some very expensive outliers.  
- **Cleanliness rating strongly impacts guest satisfaction**.  
- **Closer to city center or metro → higher prices**.  
- Locations with **higher attraction and restaurant indices** improve guest ratings.  

---

## 🚀 Next Steps

- Extend this project by applying **Machine Learning** to predict:
  - Price category (cheap vs expensive).
  - Guest satisfaction score.
- Add **geospatial maps** to visualize Airbnb distribution across London.  

---
