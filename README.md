"# Predict-Football-RidgeRegression" 

## Libraries used:
#Prediction and Prepare data
-Pandas
-Pickle
-Sklearn 
-Numpy
#Crawl Data (only an addition and not the main point of the project)
-BeautifulSoup
-requests

## Motivation:
As a big soccer fan it is super interresant to do soccer predictions. Soccer is the most popular sport in the world and large amounts of money are invested in betting every year. Now when making a bet, it would be great to use machine learning tools to generate your own predictions in order to win the bet.

## Files: 
-Predict_RidgeRegression.ipynb: The main point of the project. This is where the predictions are made. 
-Statistics.ipynb: Just an addition to see how the data was collected. 
-Statistics2018-, Statistics2019-, Statistics2020.pkl: Statistics for the 2018, 2019, 2020 seasons.
-1 Feature RR.xlsx, Combi Feature RR.xlsx: Excel tabs showing the results for certain combinations.
- Ridge Regression.pptx: Summary and visualization of the results
- List_of_Features: Feature list that can be used

## Points from CRISP-DM

1.  Business Understanding
In this project, we try to predict other soccer games with statisics of soccer games.
This raises the questions:
- Which feature makes soccer predictions most successful?
- Is a combination of features useful?
- What percentage of games can be successfully predicted?

2. Data Understanding
The data was taken from the site www.kicker.de. Kicker is the biggest sports magazine in Germany and collects statistics for every soccer team. Thus one has from each of the 18 teams to each game many statistics.
If you want to predict a match of two teams, you have to get the statistic values from the previous matches of these teams. 

3. Prepare data 
First the data is crawled and saved in a pkl file. In this file all matches (9) of 34 matchdays are stored. 
Since a game consists of two teams and the game day can be selected by the user, the data must be dynamically specified so that data from two teams can be collected and compared for different game days. In addition, you have to make sure that you only collect the relevant data from previous match days.

4. Model data
As model data we now have the previous statistics of both teams and the teams of the queried models. Ridge Regression is used as the model. The features are tested individually and considered as a combination. The combinations are chosen with RandomForrest and by hand.

5. Results
Different scenarios are tested. First, all features are tested individually and a number of combinations. In addition, a different a number of previous match days are considered. In combination of these cases it is investigated how best to predict soccer matches. In the Excell table you will find the individual test results. These are summarized again in the Powerpoint. 

6. Deploy 
With this event the company can give a certain tendency for each match. Thus, users can use this odds to bet on soccer matches. The better the prediction is, the more users will access the kicker. This can increase the size of the readership of the sports magazine.
