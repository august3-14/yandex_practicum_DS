# Analysis of Apartment Sale Listings
You have access to data from the Yandex Real Estate service—an archive of apartment sale listings in St. Petersburg and neighboring settlements over several years. Your task is to learn how to determine the market value of real estate properties. To achieve this, conduct an exploratory data analysis and identify the factors influencing property prices. This will enable the development of an automated system to detect anomalies and fraudulent activities.

For each listed apartment, two types of data are available. The first type is entered by users, while the second is generated automatically based on mapping data. For example, information such as the distance to the city center, the airport, and other landmarks is retrieved automatically from geoservices. The number of parks and water bodies is also determined without user input.

## Data Description
* `airports_nearest` — distance to the nearest airport (meters)
* `balcony` — number of balconies
* `ceiling_height` — ceiling height (meters)
* `cityCenters_nearest` — distance to the city center (meters)
* `days_exposition` — number of days the listing was active (from publication to removal)
* `first_day_exposition` — publication date
* `floor` — floor number
* `floors_total` — total number of floors in the building
* `is_apartment` — whether the property is an apartment (Boolean type)
* `kitchen_area` — kitchen area (square meters)
* `last_price` — price at the time of removal from the listing
* `living_area` — living area (square meters)
* `locality_name` — name of the locality
* `open_plan` — open-plan layout (Boolean type)
* `parks_around3000` — number of parks within a 3 km radius
* `parks_nearest` — distance to the nearest park (meters)
* `ponds_around3000` — number of water bodies within a 3 km radius
* `ponds_nearest` — distance to the nearest water body (meters)
* `rooms` — number of rooms
* `studio` — whether the property is a studio (Boolean type)
* `total_area` — total apartment area (square meters)
* `total_images` — number of apartment photos in the listing

## Plan
1. **Data Review**  
  1.1. Changing Data Types  
  1.2. General Data Assessment  
2. **Data Preprocessing**  
  2.1. Handling Missing Data  
    2.1.1. LOCALITY_NAME  
    2.1.2. IS_APARTMENT  
    2.1.3. PONDS and PARKS  
    2.1.4. BALCONY  
    2.1.5. LIVING_AREA  
    2.1.6. KITCHEN_AREA  
    2.1.7. Other Indicators  
  2.2. Handling Duplicates  
3. **Additional Data**  
  3.1. SQ_METER_PRICE  
  3.2. WEEKDAY, MONTH, YEAR  
  3.3. FLOOR_TYPE  
  3.4. CITY_CENTER_KM  
4. **Exploratory Data Analysis**  
  4.1. Handling Outliers  
    4.1.1. TOTAL_AREA  
    4.1.2. LIVING_AREA  
    4.1.3. KITCHEN_AREA  
    4.1.4. LAST_PRICE  
    4.1.5. ROOMS  
    4.1.6. CEILING_HEIGHT  
    4.1.7. FLOORS_TOTAL  
    4.1.8. FLOOR_TYPE  
    4.1.9. CITY_CENTERS_NEAREST  
    4.1.10. PARKS_NEAREST  
  4.2. Apartment Sale Speed  
  4.3. Factors Affecting Property Price  
  4.4. Calculation of Average Price per Square Meter  
  4.5. Apartment Price vs. Distance from City Center  
5. **General Conclusions**
