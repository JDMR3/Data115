# For DATA 115, WSU Fall Semester 2021
---------------------------------------------------------------------------------------------------------------------------------
Motivation for the Project
---------------------------------------------------------------------------------------------------------------------------------
I set out to answer if True Shooting affected Winning percentages, I recently started looking into basketball statistics as I've been watching the NBA but not really paid attention to the stats outside of the major ones (points, assists and rebounds), 

2020-2021 NBA Season, Data Process
----------------------------------------------------------------------------------------------------------------------------------
Gathered my data from https://www.basketball-reference.com/ 
Oringinally a 540 player data set from the NBA's 2020-21 season, decided to organize the data by most games played by the players, and by team, focused on the True Shooting column of the statistics removed all the data after True shooting percentage. Decided to remove players who played less than 20 games, resulted in the removal ofaround 300 people because of this. Those players were removed to reduce the amount skewness.

Some loose numbers with players who were traded, decided to remove the data as I could only export around 600 values from Basketball Reference.

Added a Win Rate column that was not in the data set, to the data by standard win / loss calculation, because the data was organized by team and games played, it was just a matter of calculating the win rate for the 30 teams.

Updated version with all the teams, originally had data on just 50 players, did not have enough data points the Correlation was around 0.5 that did not seem right so recreated the data with the 300 different players.

----------------------------------------------------------------------------------------------------------------------------------![000092 (1)](https://user-images.githubusercontent.com/91152880/144525428-38c892d7-a73d-402c-8a0c-3a2b4cafa84c.png)

-------------------------------------------------------------------------------------------------------------------------------
Analysis: 5 Number Summary, Pearson's r
-------------------------------------------------------------------------------------------------------------------------------
Pearson's R: 0.223486.
-------------------------------------------------------------------------------------------------------------------------------
Pearson's correlation coefficient was used to test the association of the 2 columns, because the amount was between 0.1 and 0.3, it was a postive correlation but it was a there was a small strength of association. 

Makes sense because it takes more than offence to win in the game of basketball, as defence is just as important.

Some players shined on the bad teams and vice versa.

|Quartiles|True Shooting |Win Rate |
|---------|--------------|---------|
|MIN|	  0.363	           |	0.236  |
|1st Q|	0.533            |  0.431  |
|MEDIAN|	0.567          |0.542    |
|3rd Q|	0.601		         |0.619    |
|MAX| 0.736		           | 0.722   |

--------------
![image](https://user-images.githubusercontent.com/91152880/144703315-766af838-15f6-442f-a192-7904ab8a55bb.png)
-----------------
Box and Whisker chart of every team, quite a few outliers (red stars).
Atlanta, Brooklyn, Wash and Milwakee all had higher than avearge TS and they made the playoffs. Golden state also had a high True Shooting percentage however they did not make the playoffs.
Some teams have really efficient people playing for them, while others not so much, causes an imbalance but the higher win rate teams have a good balance. 
The Outliers could be caused by the amount of minutes played or shots that are taken as not everyone can have the ball,

Josh Hall of The Oklahoma City Thunder had the lowest true shooting % with 0.363 played exaclty 20 games, and OKC had the second worst record in the Western Conference at 0.306.

Highest True Shooting% value was DeAndre Jordan of The Brooklyn Nets, with 0.736, and the Brooklyn Nets were second in the Eastern Conference.

Highest win rate team Utah at 0.722, is at the top while the worst team is Houston with 0.236. 

The Center position had some of the highest True shooting percentages on teams.

----------------------------------------------------------------------------------------------------------------------------------
Old data info, not really relevent anymore as I only focused on 50 people
----------------------------------------------------------------------------------------------------------------------------------
![PDS](https://user-images.githubusercontent.com/91152880/142282949-3ecde435-e6b0-46e8-a922-771906083eff.jpeg)
----------------------------------------------------------------------------------------------------------------------------------

Scatterplot comparing True Shooting and Win percentage for the top 50 players, who played the most games in the 2020-2021 season.
----------------------------------------------------------------------------------------------------------------------------------
I evaluated outliers for my win% variable as some players were traded mid season, I took the average for the teams that they played on. Also this data set was  organized based on the top 50 players and by the most amount of games played.
