# Airbnb Listings EDA & Data Viz Project: New York

![Renting-out-on-Air-BnB-980x655](https://github.com/user-attachments/assets/13abc58f-626a-4c0c-837c-16ecf451f186)

## Project Overview
This project performs **Exploratory Data Analysis (EDA)** on New York Airbnb data to uncover trends and patterns in rental listings using libraries like **Pandas, Numpy, Matplotlib, Seaborn** for cleaning, visualization, and analysis. 

## Objective
The goal of this project is to:
1. Detect and remove potential **outliers** in rental prices.
2. Analyze **price distribution and average price per bed** across different neighborhoods.
3. Analyze the **ratings** distribution for all rental listings.
4. Find relationship between **price** and **rating** of the rental listings.

## Dataset
The dataset contains **20,770 rows and 22 fields**, including:
- `id`: Unique identifier for each listing  
- `name`: Title of the Airbnb listing  
- `host_name`: Name of the host  
- `neighborhood_group`: Area where the listing is located  
- `latitude/longitude`: Geolocation of listings  
- `price`: Per night rental price  
- `room_type`: Type of accommodation (e.g., entire home, private room)  
- `reviews_per_month`: Average monthly reviews for the listing  
- `availability_365`: Number of available days in the year

## Workflow

### 1. Data Cleaning
- **Handle missing data**: Dropped all NULL values from the dataframe.
- **Handle duplicate entries**: Dropped all duplicate entries from the dataframe.
- **Remove outliers**: Listings with **price > $2,000** were capped to avoid skewed visualizations.

### 2. EDA & Data Visualization
1. **Price distribution**: 
   - Visualized the price distribution after removing potential outliers using histogram.
   - Identified **rent < 250$** as the most common rental price range.

2. **Rating Distribution**:
   - Analyzed ratings given by guests.
   - **Ratings > 4** had the max. frequency.

3. **Price Distribution Across Neighbourhood**:
   - Used barplot to show rent across differnet areas in New York.
   - Further categorized it based on room types.

4. **Price/Bed Distribution Across Neighbourhood**:
   - Used barplot to analyze rent per bed across differnet areas in New York.
   - Further categorized it based on room types.

5. **Relationship between Price and Ratings**:
   - Used scatterplot to show the relationship between rental price and ratings given by guests.
   - **Ratings > 4** were common for listings with high rental.

6. **Geographic Distribution of Airbnb Listings**:
   - Used scatterplot to vizualize Airbnb locations using their longitude and latitude values.
   - Found out Hotel Rooms were extremely less and majority of the room types were either Private or Entire Home.

## Key Findings and Insights


## Conclusion
This project offers valuable insights into the New York Airbnb listings, helping both guests and hosts make informed decisions. By using **EDA techniques**, we identified key trends and developed actionable recommendations. Future improvements can involve advanced analytics and predictive modeling to further enhance the findings.
