## Market Research on Video Games
For the task received from the business, we need to conduct research on the video game market to identify patterns that determine the success of a game. This will allow the client to bet on a potentially popular product and plan marketing campaigns. For the research, we will use historical data on game sales taken from open sources. The data will include ratings from users and critics, information on genres and platforms (e.g., Xbox or PlayStation).

## Data Description:
* `Name` — game title
* `Platform` — game platform
* `Year_of_Release` — release year
* `Genre` — game genre
* `NA_sales`— sales in North America (millions of copies sold)
* `EU_sales` — sales in Europe (millions of copies sold)
* `JP_sales` — sales in Japan (millions of copies sold)
* `Other_sales` — sales in other regions (millions of copies sold)
* `Critic_Score` — critic score (maximum 100)
* `User_Score` — user score (maximum 10)
* `Rating` — rating by the ESRB organization, defining the game's age category

## Plan
1. **Data Familiarization**  
2. **Data Preprocessing**  
   - 2.1. Table Header and Data Types  
   - 2.2. Handling Duplicates  
   - 2.3. Handling Missing Values  
      - 2.3.1. NAME & GENRE  
      - 2.3.2. YEAR_OF_RELEASE  
      - 2.3.3. RATING  
      - 2.3.4. CRITIC_SCORE  
      - 2.3.5. USER_SCORE  
   - 2.4. Calculating Total Sales Indicator  
3. **Exploratory Data Analysis**  
   - 3.1. Dynamics of Game Releases Year by Year  
   - 3.2. Dynamics of Platform Profitability Year by Year  
   - 3.3. Sales Distribution Among Top-5  
   - 3.4. Impact of Ratings on Sales  
   - 3.5. Sales Distribution by Genre  
   - 3.6. Sales Distribution by Platform  
4. **User Profile**  
   - 4.1. Popular Consoles  
   - 4.2. Popular Genres  
   - 4.3. Impact of Rating  
5. **Hypothesis Testing**  
   - 5.1. Hypothesis #1. Ratings of Xbox One and PC Platforms  
   - 5.2. Hypothesis #2. Ratings of Action and Sports Genres  
6. **Conclusions**
