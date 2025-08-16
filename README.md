# NYC Airbnb EDA

A concise, business-focused **Exploratory Data Analysis** of New York City Airbnb listings to uncover **pricing trends**, **host behavior**, and **guest preferences**. Built for fast insight generation and clean storytelling.

---

## What this project does
- Cleans and validates raw Airbnb data (20,765 rows, 22 columns)
- Explores **prices, room types, neighborhoods, availability, reviews**
- Detects **outliers** and fixes data types (e.g., `last_review` → datetime)
- Visualizes trends with **heatmaps, histograms, boxplots, bar charts, pairplots**
- Produces **actionable recommendations** for both **guests** and **hosts**

---

## Dataset (key fields)
- `id`, `name`, `host_name`
- `neighborhood_group` (borough), `neighborhood`, `latitude`, `longitude`
- `room_type`, `price`, `minimum_nights`
- `number_of_reviews`, `reviews_per_month`, `availability_365`

> Notebook: `airbnb_eda.ipynb` 

---

## Methodology (Pipeline)
1. **Data Cleaning**
   - Handle missing values (e.g., `price`, `beds`, `neighborhood`)
   - Convert data types (`last_review` → datetime)
   - Cap extreme price outliers (> \$1,000) for stable visuals

2. **EDA**
   - **Room Types:** distribution & price differences
   - **Geography:** borough-wise price/availability patterns
   - **Price Analysis:** distribution, outliers, robust stats
   - **Availability & Reviews:** correlation with price and demand
   - **Host Behavior:** multi-listing hosts, variability via boxplots

3. **Visualization**
   - **Heatmap**: correlations among numerical features
   - **Histograms & Boxplots**: price distribution & outliers
   - **Bar Charts**: room types, neighborhood groups
   - **Pairplots**: reviews × price × availability

---

## Key Insights
- **Manhattan** is the most expensive; **Brooklyn** is next and offers strong value.
- **Entire home/apt** dominates supply and is significantly pricier than **private rooms**.
- Listings with **higher availability** tend to be **cheaper** and receive **more reviews**.
- A subset of **professional hosts** (multi-listing) drive a sizeable share of supply.

---


  
