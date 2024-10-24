# Data Analytics Bootcamp @ neuefische GmbH - Capstone Project

A collaborative project focused on analyzing the **Impact of Renewable Energy on Emissions Reduction**, uncovering trends and insights.

## 🔍 Project Overview 

This capstone project was completed as part of the **Data Analytics Bootcamp** @ neuefische GmbH. The project has been developed in 4 weeks in June 2024 by [Steve](https://github.com/Goal1803), [Trina](https://github.com/trinakohestani) and me. 

The main objectives of the project were:

- Define the project around a business question
- Find relevant data
- Complete a data technical analysis 
- Present findings in a final presentation

## 💻 Technologies used 

- Jupyter Notebooks
- Python (pandas, matplotlib, seaborn)
- SQL
- Tableau
- GitHub

## 📁 Project structure 

- `data/`: Contains the dataset used for analysis 
- `notebooks/`: Jupyter Notebooks containing data cleaning, analysis, and visualizations. One notebook per hypothesis presented. 
- `presentation/`: Final presentation used for the graudation event 
- `README.md`: Project documentation and instructions.

## 📊 Project Summary 

This project explores the **growth and impact of renewable energies** during the last 20 years and examines their effect on global CO2 emissions. 

As data show, **energy is the main driver** of CO2 and GHG emissions:

![Screenshot 2024-10-24 at 13 41 28](https://github.com/user-attachments/assets/39da959f-15b9-4087-b80a-56e39a23f71d)

Although we observed a significant drop on emissions from 2019:

![Screenshot 2024-10-24 at 13 50 17](https://github.com/user-attachments/assets/003d78ec-18bf-4835-9e8e-630a32adf9c4)

Which led us to define our research question: *'What are the trends in renewable energy and how does it contribute to the reduction of emissions?'*. To help answer it, we developed three hypothesis:

1. Solar and wind energy are the fastest-growing types of renewable energy
2. Higher share of renewable energy generation is associated with lower carbon intensity levels, indicating a cleaner energy production
3. Carbon footprint is determined by the level of economic development and the share of renewable energy consumption

### Hypothesis 1

**Solar and wind energy are the fastest-growing types of renewable energy**

Despite solar and wind energy having lower generation intensity,

![Screenshot 2024-10-24 at 14 41 33](https://github.com/user-attachments/assets/02af7a0e-a2af-4468-b40a-f107f77e3548)

their rapid growth of energy generation stands out from other renewable energy sources. 
 
![Screenshot 2024-10-24 at 14 44 13](https://github.com/user-attachments/assets/41f61d64-8f80-42b0-87d8-4b009a5d0f4b)

Those two are the most popular renewable energy sources due to their availability, scalibility and lower costs. Their environmental benefits and versatility make them preferred choices, accelerating their adoption in the renewable energy mix.

Therefore, we accept the first hypothesis: Solar and wind energy are the fastest-growing types of renewable energy ✅

When taking a closer look at the 15 countries with the lowest carbon intensity, we observed that the share of hydropower energy is significanty higher than other sources.

<img width="870" alt="Screenshot 2024-10-24 at 15 59 46" src="https://github.com/user-attachments/assets/52693c91-ef3e-4ebf-b015-a7567552ed44">


### Hypothesis 2

**Higher share of renewable energy generation is associated with lower carbon intensity levels, indicating a cleaner energy production**

Having observed the negative relationship between global carbon intensity and renewable energy generation share: 
   
<img width="554" alt="Screenshot 2024-10-24 at 14 58 03" src="https://github.com/user-attachments/assets/368a8ff6-0791-4e9d-bc28-aae9061a5d6a">

We calculated the following values:

- Correlation coefficient = **-0.81** 
- p-value = **< 0.001**
- R-Squared = **0.66**
- F-Statistic = **6739**

therefore, we can confirm that:

-    There is a **strong inverse relationship** between these two variables, meaning the higher the share of renewable energy generation, the lower are the carbon intensity levels
-    This correlation is **statistically significant**
-    **66% of the variability** in carbon intensity can be explained by the share of renewble energy generation, which suggests a moderately strong explanatory power
-    Indicates a very strong relationship in our analysis, explaining a substantial portion of the variance 

The second hypothesis is also accepted: Higher share of renewable energy generation is associated with lower carbon intensity levels, indicating a cleaner energy production ✅

### Hypothesis 3

**Carbon footprint is determined by the level of economic development and the share of renewable energy consumption**

Looking at the relationship between carbon footprint and GDP per capita,

!<img width="616" alt="Screenshot 2024-10-24 at 15 23 07" src="https://github.com/user-attachments/assets/59a8012f-fbb3-4bfb-a347-1648550c6292">

and the following calculations:

- Correlation coefficient = **0.69** 
- p-value = **< 0.001**

We confirm the **positive relationship** between carbon footrpint and GDP per Capita, being a **statistically significant**.

On the otherside, observing the relationship between carbon footprint and renewable energy consumption,

<img width="632" alt="Screenshot 2024-10-24 at 15 23 58" src="https://github.com/user-attachments/assets/2d77a52a-5358-49f9-ae89-2a5d1d145a03">

and the following calculations:

- Correlation coefficient = **-0.58** 
- p-value = **< 0.001**

We count on a **negative relationship** between carbon footrpint and renewable energy consumption, also being a **statistically significant**.

After performing a **regression model**, having carbon footprint as dependent variable and GDP per capita and share of renewable energy consumption as independent variables, the results are:

- R-Squared = **0.609**
- F-Statistic = **2283**

meaning that 60.9% of the variance in CO2 emissions per capita can be explained by the independent variables. 

However, with the aim of improving our model, two other variables were included as independent variables: industry share and energy intensity. With a more complete model we got the following results:

- R-Squared = **0.711**
- F-Statistic = **2283**

  

meaning that **71.1 % of the variability** in CO2 emissions per capita can be explained by the four independent variables: GDP per capita, renewable energy consumption, industry share and energy intensity, being significant to explain crbon footprint levels.

Therefore, we can also accept the third hypothesis: Carbon footprint is determined by the level of economic development and the share of renewable energy consumption ✅

### Key take aways and recommendations

- Countries with **favorable weather conditions** should focus on solar and wind energy as their top choices​
- Countries with **water abundance** should focus on hydropower in their renewable energy mix
- It is advisable to prioritize other types of renewable energy sources and **diversify** their energy portfolio to prevent over-reliance on weather-dependent sources​
- Incentivize renewable energy sources and adopt measures to **improve energy efficiency** and diversify economies with a high industrial share
