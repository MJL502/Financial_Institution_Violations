# Fainancial_Institution_Violations

## Description
- This project analyzes data from the FIDC to determine if there are correlations between institutions with violations and Region, Size of Institution, Age of Institution, and/or type of Institution.

## RESULTS:

- The average number of field goal attempts per game (per team) is 1.62 per team. 
- The average percentage of made field goals is 84.4%.
- The average number of made field goals per game is 1.4 per team.  
- The 'TOP 25 BEST AND WORST CRITERIA' chart is the most important.  It shows which factors have the biggest influence (positive and negative).  There are also charts for each category, so a person picking a kicker to start in any given week can compare his choices using the results we have from any of our categories.
- NEGATIVE - Of the categories we analyzed, 'defense against' plays the biggest role when predicting a lower than average number of field goals.  
- POSITIVE - Stadium, Defense against, and Kicker can all be used to predict higher than average field goals per game more than environmental factors (wind, temperature, etc.).  
- Environmental factors do have a measurable effect, but not nearly as much (positive or negative) as the other categories.  

## Technologies:

- Python
- SQL
- Jupyter Notebook
- _________________________________
- _________________________________
- _________________________________

## Getting Started:

1. Clone `https://github.com/MJL502/Financial_Institution_Violations`
2. Make sure you have pandas installed on your machine
3. Make sure you have Jupyter Notebook installed on your machine
4. Make sure _____________________________
5. Open Financial_Institution_Violations.ipynb
6. Click 'Run All'
7. If it asks you "____", choose ______.


## Features:

- [ ] 1. Reads data in from a csv file (the historical_field_goal_data.csv in the data file)
- [ ] 1. Creates dictionaries (for each year)
- [ ] 2. Uses functions to remove Null values (specifically to remove null values from the temperature column and replace them with a value of 0)
- [ ] 3. Uses custom functions to analyze data (an example is the compare_single_criteria function)
- [ ] 4. Uses seaborn / matplotlib to create graphs showing data by category, most advantageous, and least advantageous.
- [ ] 5. Data is interpreted in the read me file (see Description and Results above)


## LIMITATIONS:

- There were 2,405 games.  There were 2,352 games with a field goal attempt (98%).  There were 53 games with no field goal attempts (2%). This model looks at a specific criteria and multiplies field goal attempts per game by field goal percentage to predict the number of made field goals that will occur.  However, there is no data in our data set from games in which there were no field goal attempts.  While this does not effect field goal percentage, it does effect field goal attempts per game, and thus it effects our prediction of total number of field goals that will occur.  Since we do not have the criteria for those games (temperature, windspeed, etc.) we cannot retroactively add that data back in.  The number of games without a field goal is small enough that it should not effect the model's ability to accurately predict which criteria will produce the most or least field goals per game, but the number of predicted field goals per game may not be accurate past 2 decimal points.  My theory is that most games with no field goal attempts are a result of one of the criteria that produce lower fg's per game being present, and thus if it were possible to add the results in, they would actually reinforce our findings and increase the difference between the best and worst criteria.


## OBSTACLES:

- There were several stadiums that changed names over the years.  These stadiums had to have their names changed to a common name so comparisons by stadium would be accurate.  Likewise, there are teams that moved cities, and since the team name in four columns is based on city, the team names had to be changed to common name for comparisons.  As an example, the Raiders were identified as OAK in the first years of the data set and LV in the later years.  This caused comparisons by team to throw errors because when it tried to analyze data for LV in certain years, they did not exist (same for OAK).  By creating a common name (OAK-LV) all the methods work correctly.  It was more efficient to adjust the data than it would have been to modify the methods.


## TODO:

- [ ] REFACTOR


## LICENSE:

- None