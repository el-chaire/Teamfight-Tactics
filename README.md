# Predicting eSports Outcomes: Teamfight Tactics

### Summary
- Teamfight Tactics is a game by Riot Games in the Autochess genre, where players draft and position their team to compete with 7 other players in a game
- Getting high placements in ranked games would result in increase in rank points while low placements would result in decrease of rank points.
- Using the information gathered using the Riot Game API and some feature engineering, we are able to predict the probability of whether a team composition in game would have a high placement. From this we derive strategies that would increase the chances of high placements and as a consequence increase the rank of the player. 

### File descriptions
##### Data:
- Obtaining Raw Data: This notbook obtains data from Riot Games using it's API
- Data Preparation 1 - Extracting from Raw Data: Feature engineers the data on the teams in the matches compiling each team composition as a data point and saves to "synergy_carry_value_df.pkl" which can be taken as the main data file for this project
- Data Preparation 2 - Encoding: Encodes "synergy_carry_value_df.pkl" with one hot encoding and ordinal encoding when appropriate

##### Models:
- KNN
- Random Forest
- Neural Network - Best performace with ROC_AUC = ~.9

##### Predictions:
- Mock Data series of file: The series of notebooks that will create the mock data which are hypothetical teams in the game and we will feed it into the model to obtain predictions of probability to obtaining top placement

### Conclusion
We are able to predict the performance of team compositions in Teamfight Tactics reasonable well and we are able to derive reasonable strategies that were built upon the common strategies used to obtain high placements in top level competition (Top 1% in North America). The implementation of these strategies, from 10/13/2021-10/20/2021 caused an increase of personal ranking from top 20% to top 9% which is a new personal best. This can be seen in the following link: https://lolchess.gg/profile/na/elchaire/s5.5

### More information can be found in the .pdf report.