## About

For this project, I sought to determine whether the opening moves made in a chess game affected the outcome of the game. I chose to perform analysis of the top five most used chess openings. These were the Sicilian Defense, French Defense, Queen’s Pawn Game, Italian Game, and King’s Pawn Game. I found through my exploratory data analysis, that these openings did not have a high correlation to games ending in a draw, or games that ended due to running out of time. Three openings, Sicilian Defense, French Defense, and Queen’s Pawn Game, related to a large number of games ending in a player resigning. 

I created several PMFs, CDFs, and Scatterplots to examine the data and determine how best to create my regression model. I ultimately chose to build a Multinomial Logistic Regression model to determine the relationship between opening moves and game outcome.


## Data

Data for this project was pulled from [Kaggle](https://www.kaggle.com/datasets) surrounding games played between online chess players.


## Conclusion

I discovered through my analysis (Multinomial Logistic Regression) that there is a statistically significant relationship between these the opening moves in a chess game and the outcome of the game. This significance does not necessarily mean that one opening move over the other guarantees a win or a loss, but it does show that it can impact the game. 
