## Cow Milk Yield Prediction

A dairy farm owner wants to buy cows to expand his herd. To achieve this, he has signed a favorable contract with a pasture association. The terms allow the farmer to carefully select cows based on strict quality criteria. He determines milk quality using a rigorous methodology while also ensuring that he meets his dairy farm development plan. The farmer wants each cow to produce at least 6,000 kilograms of milk per year, and the milk must meet his strict taste criteria.  

Our task is to develop a machine learning model to help manage risks and make objective purchasing decisions. We need to create two predictive models for selecting cows for the herd:
* The first model will predict the possible milk yield of a cow (target feature: `Удой, кг`);
* The second model will estimate the probability of obtaining tasty milk from a cow (target feature: `Вкус молока`).

The model should select cows based on two criteria:
* The average milk yield per year must be at least 6,000 kilograms;
* The milk must be tasty.

## Data Description

1. The dataset `ferma_main.csv` contains data on the farmer’s current herd.
   * `id` — unique cow identifier.
   * `Удой, кг` — Milk Yield, kg, the amount of milk a cow produces per year (in kilograms).
   * `ЭКЕ` — ECE (Energy Feed Unit), a measure of the nutritional value of the cow’s feed.
   * `Сырой протеин, г` — Crude Protein, g, the amount of crude protein in the feed (in grams).
   * `СПО` — SPR (Sugar-Protein Ratio), the ratio of sugar to protein in the cow’s feed.
   * `Порода` — Breed, the cow's breed.
   * `Тип пастбища` — Pasture Type, the type of pasture landscape where the cow grazed.
   * `порода папы_быка` — Sire Breed, the breed of the cow's father.
   * `Жирность, %` — Fat Content, %, the percentage of fat in the milk.
   * `Белок, %` — Protein, %, the percentage of protein in the milk.
   * `Вкус молока` — Milk Taste, a milk taste rating based on the farmer’s personal criteria, a binary feature (tasty, not tasty).
   * `Возраст` — Age, the cow's age, a binary feature (`менее_2_лет`, `более_2_лет`).

2. The dataset `ferma_dad.csv` stores the name of each cow’s father in the farmer’s herd.
   * `id` — unique cow identifier.
   * `Имя Папы` — Father's Name, the name of the cow’s father.

3. The dataset `cow_buy.csv` contains data on cows from "EcoFarm" that the farmer wants to evaluate before purchasing.
   * `Порода` — Breed, the cow's breed.
   * `Тип пастбища` — Pasture Type, the type of pasture landscape where the cow grazed.
   * `порода папы_быка` — Sire Breed, the breed of the cow's father.
   * `Имя_папы` — Father's Name, the name of the cow's father.
   * `Текущая_жирность, %` — Current Fat Content, %, the percentage of fat in the milk at the time of sale.
   * `Текущий_уровень_белок, %` — Current Protein Level, %, the percentage of protein in the milk at the time of sale.
   * `Возраст` — Age, the cow's age, a binary feature (`менее_2_лет`, `более_2_лет`).

The protein and fat content in the milk is recorded at the time of sale when the seller was feeding the cows their own feed.  
The parameters **ЭКЕ (Energy Feed Unit), Сырой протеин, г (Crude Protein, g), and СПО (Sugar-Protein Ratio)** are missing from the dataset.  
The buyer’s nutrition experts have revised the feeding approach: for new cows, they plan to **increase each of these parameters by 5%**.  
Additionally, the target features `Удой, кг` and `Вкус молока` are missing and need to be predicted.

## Plan

1. Data Exploration
    - 1.1 Dataset #1 `ferma_main` &mdash; main information about the farmer's herd
    - 1.2 Dataset #2 `ferma_dad` &mdash; information about the cows' lineage
    - 1.3 Dataset #3 `cow_buy` &mdash; information about new cows
2. Data Preprocessing
3. Exploratory Data Analysis
    - 3.1 Quantitative Variables
    - 3.2 Categorical Variables
4. Correlation Analysis
    - 4.1 Quantitative Variables
    - 4.2 Categorical Variables
5. Training a Linear Regression Model
    - 5.1 First Linear Regression Model
    - 5.2 Second Linear Regression Model
    - 5.3 Third Linear Regression Model
    - 5.4 Applying Metrics to Assess Model Accuracy
    - 5.5 Determining Confidence Intervals
    - 5.6 Predicting Cow Milk Yield
6. Training a Logistic Regression Model
7. Conclusions

