## Fifa-Football-Analysis

#### Introduction

As one of the most popular sports in the world, soccer is played by thousands of players, amateurs and professionals. According to the number of players and spectators, football is the most watched sport in the world. The sport may be played practically everywhere, from official football playing fields (pitches) to gymnasiums, streets, school playgrounds, parks, or beaches, thanks to its basic rules and necessary equipment. The Fédération Internationale de Football Association (FIFA), the organization in charge of administering football, claimed that there were about 1.3 billion "interested" football fans and over 250 million active football players at the beginning of the twenty-first century. Therefore, it comes as no surprise that it produces a massive quantity of data. It is crucial in today's data-driven environment to come up with the best, most understandable approach to display the facts, a strategy to create visually discernible patterns that can be matched to data patterns, allowing for the exploration of the data and comprehensibility. The interactive system we describe in this study uses visualization to examine soccer data and spot trends, correlations and revelations. We provide examples of how our approach, particularly for non-visualization professionals, by using World Cup data and exploring potential applications cases.

#### Problem Statement
Our goal is to determine the value of a player with respect to the wage of the player, the age, the potential of the player and height.
This would be helpful for the users to determine the best players that they can choose and proceed with the team.

#### Data Acquisition 
The data was collected from the website www.data.world. The website contains the data from the EA Sports game FIFA. Since 1995 the FIFA Soccer games have provided an extensive and coherent scout of players worldwide. 
The dataset contains 92 attributes and 17954 instances which consists of numerical as well as categorical data. The data contains features about players like their skills and value in the market. Some other attributes were age, height_cm, wage_euro etc… 

#### Data Pre-Processing
The original dataset consisted of 92 attributes from which attributes which were not necessary for our analysis had to be removed. This includes columns such as tags, and position scores of players which were in string data type. Forty-one attributes which were not required for our analysis had to be removed. Therefore the cleaned dataset consists of 51 attributes out of which 11 attributes were categorical ones and 40 numerical attributes. Instances with null values were also discarded. 
For the attribute, ‘body_type’ which consisted of three types Normal, Stocky and lean, but some variables had player’s names as a value in the original dataset. Instead of dropping such instances, we changed their value into one of the three body_types and this was done because these players were necessary for our analysis.
We also cleaned the attribute names and made the first letter as an uppercase and cleaned the names and removed irrelevant words.

#### EDA
Exploratory Data Analysis (EDA) is an approach to analyze the data using visual techniques. It is used to discover trends, and patterns, or to check assumptions with the help of statistical summaries and graphical representations. For Exploratory data analysis, the tool used was R. We plotted some graphs which were visually and statistically necessary. 

#### Model Selection
The model that we chose for our project was Multiple regression. Since our dataset contained numerical data, it was more convenient to use multiple regression. Using a logistic regression was of no use since there wasn't much categorical data to classify them.

Multiple linear regression (MLR), also known simply as multiple regression, is a statistical technique that uses several explanatory variables to predict the outcome of a response variable. The goal of multiple linear regression is to model the linear relationship between the explanatory (independent) variables and response (dependent) variables. 

Advantages of multiple regression:
- The ability to determine the relative influence of one or more predictor variables to the criterion value. 
- The ability to identify outliers, or anomalies.

#### Description of the Model
It was observed from the multiple regression model that the R- squared value for the model was 0.7929 and the adjusted R- squared value is 0.7928. This depicts that our model has an accuracy of 79%.

#### Variables
We used “value” as the dependent variable. We needed to find the value of the players and that’s the reason for choosing “value” as the dependent variable. The independent variables are: “Age”, “Overall”, “Potential”, “Wage”, “International_reputation”, “Stamina”, “Sliding_takcle”, “Standing_tackle”, “Height”. 
These independent variables were found to be the most reasonable variables when considering the dependent variable.

#### Conclusion
The model provides a clear idea about determining the value of a player in euro. The R- squared value gives us an accuracy of 79 percent from which we can say that our model can predict 79 percent of the data correctly. The independent variables that we took for multiple regression had a positive correlation with the ‘value’ variable. Therefore player value prediction is dependent on these factors. So when selecting a player to a team, the team manager can check these factors in a player so that a perfect team is set. Moreover a team needs players in every position like striker, mid-fielder, defender and goalkeeper and knowing these factors about the players will surely help them build up a better team.

