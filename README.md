# Airbnb Bordeaux Market Analysis

## 1. Background and Overview
Bordeaux, France, a UNESCO World Heritage site, is renowned for its rich cultural heritage, world-class wine, and relaxed pace of life. The city has become a magnet for middle-class retired couples from high-income countries seeking immersive travel experiences and extended stays. This project investigates the Airbnb rental market in Bordeaux to uncover opportunities for a new entrant to establish a foothold by addressing gaps in the current offerings.

Leveraging data from "Inside Airbnb" and public sentiment on Reddit, this analysis delves into pricing trends, customer preferences, and sentiment dynamics. Through advanced data analytics and a customer-centric lens, this report provides actionable strategies to capture an underserved market segment.

---

## 2. Executive Summary

### Objectives
- Identify gaps in the Bordeaux Airbnb market.
- Understand preferences and pain points of middle-class retired couples.
- Develop targeted recommendations for a new entrant to compete effectively.

---

## 3. Data Manipulation and Analysis

### Data Collection
- The "Inside Airbnb" dataset provided granular data on listings, including pricing, location, room types, and guest reviews.
- Public sentiment was extracted from Reddit discussions using the `RedditExtractoR` package, focusing on travel-related subreddits mentioning Bordeaux.

### Data Cleaning
- **Airbnb Data**:
  - Missing and inconsistent entries (e.g., listings without reviews) were removed.
  - Text reviews were tokenized and processed for sentiment analysis using the `tidytext` library in R.
  - Prices were converted into uniform units (USD) for comparative analysis.

- **Reddit Data**:
  - Irrelevant posts were filtered out by using keywords (e.g., "Bordeaux" and "travel").
  - Comments were cleaned by removing URLs, special characters, and stopwords.

### Exploratory Data Analysis (EDA)
- **Neighborhood Pricing**:
  - A geospatial analysis highlighted disparities in pricing across neighborhoods.
  - Central areas like Saint-Pierre exhibited the highest average nightly rates, while suburban neighborhoods offered lower costs but lacked proximity to attractions.

- **Guest Review Analysis**:
  - Sentiment scores were calculated for text reviews using the Bing sentiment lexicon.
  - Reviews with high scores highlighted exceptional communication and location, while low scores emphasized cleanliness and perceived value gaps.

- **Occupancy Trends**:
  - Listings with higher review counts were consistently booked more frequently.
  - Price elasticity was evident, with moderately priced listings showing better occupancy than premium offerings.

### Sentiment Analysis
- **Reddit Sentiment**:
  - Positive sentiments focused on Bordeaux’s cultural appeal, gastronomy, and walkable cityscape.
  - Negative sentiments revolved around limited accommodation availability during peak seasons and lack of tailored services for retirees.

- **Review Trends**:
  - Strengths: Guests appreciated seamless check-in processes and host communication.
  - Weaknesses: Cleanliness and hidden fees emerged as consistent pain points.

### Visualizations
- **Price by Neighborhood**: A bar chart visualized the stark contrasts in pricing across central and suburban areas, aiding in identifying profitable locations.
  ![Price by Neighborhood](reports/figures/price_by_neighborhood.png)

- **Review Sentiment Over Time**: A time-series chart depicted sentiment trends, showing spikes in positive reviews during holiday seasons.
  ![Review Sentiment Over Time](reports/figures/sentiment_trend.png)

- **Word Cloud**: A word cloud of frequent terms in Reddit discussions provided insights into traveler priorities.
  ![Word Cloud](reports/figures/word_cloud.png)

---

## 4. Recommendations

### Accommodation Strategies
1. **Targeted Property Features**:
   - Design properties with retirees in mind: accessible layouts, quiet environments, and home-like amenities such as kitchens and laundry facilities.
   - Include local cultural decor to enhance the immersive travel experience.

2. **Location Optimization**:
   - Focus investments on neighborhoods with moderate pricing and cultural proximity (e.g., Saint-Michel).
   - Ensure properties are close to healthcare facilities and public transport for convenience.

### Pricing and Booking Optimization
1. **Dynamic Pricing Models**:
   - Implement algorithms to adjust pricing based on seasonality and demand.
   - Offer tiered discounts for longer stays to appeal to slow-travel enthusiasts.

2. **Transparent Policies**:
   - Clearly communicate cancellation and cleaning policies to avoid guest dissatisfaction.
   - Provide bundled packages, including guided cultural tours, to increase booking value.

### Enhanced Marketing
1. **Data-Driven Campaigns**:
   - Use insights from reviews and sentiment analysis to craft marketing messages that address retirees’ specific pain points, such as cleanliness and safety.
   - Highlight cultural immersion opportunities and community connections in promotional materials.

2. **Partnerships and Branding**:
   - Collaborate with local businesses (e.g., wineries, art galleries) to offer exclusive deals for guests.
   - Position the brand as a "home away from home" for retirees, emphasizing trust and comfort.

### Operational Excellence
1. **Service Quality Improvements**:
   - Establish a feedback loop to act promptly on cleanliness issues raised by guests.
   - Train staff to provide exceptional service tailored to retirees.

2. **Sustainability Practices**:
   - Incorporate eco-friendly practices, such as energy-efficient appliances and waste reduction programs, to align with retirees’ values.

---

## 5. Key Insights and Impact
- **Market Differentiation**: By addressing gaps in cleanliness, value-for-money, and cultural proximity, a new entrant can create a distinct niche.
- **Retiree-Centric Focus**: Catering to the needs of middle-class retirees presents a sustainable and lucrative opportunity.
- **Data-Driven Strategies**: Leveraging analytics ensures precise decision-making, from pricing to marketing.

---

This analysis underscores the untapped potential in Bordeaux’s Airbnb market. By utilizing insights from data manipulation and sentiment analysis, a new entrant can successfully establish themselves as a preferred choice for middle-class retirees seeking comfort and cultural immersion.
