# Data115
For DATA 115, WSU Fall Semester 2021
---------------------------------------------------------------------------------------------------------------------------------
Motivation for the Project
---------------------------------------------------------------------------------------------------------------------------------
I set out to answer if True Shooting affected Winning percentages, I recently started looking into basketball statistics as I've been watching the NBA but not really paid attention to the stats outside of the major ones (points, assists and rebounds), 

----------------------------------------------------------------------------------------------------------------------------------![000092 (1)](https://user-images.githubusercontent.com/91152880/144525428-38c892d7-a73d-402c-8a0c-3a2b4cafa84c.png)

----------------------------------------------------------------------------------------------------------------------------------
2020-2021 NBA Season
----------------------------------------------------------------------------------------------------------------------------------
Around 350 player data set for the 2020-21 NBA season's most games played people organied by team, focused on the True Shooting aspect of the statistics and team they were played on, removed players who played less than 20 games removed around 300 people because of this. Those players were removed to reduce the amount skewness,  
Updated version with all the teams, not just 50 players, little convoluded but the highest win rate team Utah at 0.722, is at the top while the bottom team is Houston with 0.236. 
Some loose numbers with players who were traded, decided to remove the data as I could only export around 600 values from Basketball Reference.

-------------------------------------------------------------------------------------------------------------------------------
Analysis: 5 Number Summary, Pearson's r
-------------------------------------------------------------------------------------------------------------------------------
Pearson's R: 0.223486.
Makes sense, some players shined on the bad teams and vice versa. The Center position had some of the highest True shooting percentages on the teams.
--------------------------
|------|True Shooting |	Win Rate |
|--------------|-----------|
|MIN|	0.363	   	0.236    |
|1st Q|	0.533	 	0.431    |
|MEDIAN|	0.567  0.542 |
|3rd Q|	0.601		0.619    |
|MAX| 0.736		 0.722     |


Josh Hall of The Oklahoma City Thunder had the lowest true shooting % with 0.363 played exaclty 20 games, and OKC had the second worst record in the Western Conference at 0.306.

Highest True Shooting% value was DeAndre Jordan of The Brooklyn Nets, with 0.736, and the Brooklyn Nets were second in the Eastern Conference.

----------------------------------------------------------------------------------------------------------------------------------
Old data info, not really relevent anymore as I only focused on 50 people
-----------------------------------------------------------------------------------------------------------------------------------
![PDS](https://user-images.githubusercontent.com/91152880/142282949-3ecde435-e6b0-46e8-a922-771906083eff.jpeg)
-----------------------------------------------------------------------------------------------------------------------------------
Scatterplot comparing True Shooting and Win percentage for the top 50 players, who played the most games in the 2020-2021 season.
-----------------------------------------------------------------------------------------------------------------------------------
I evaluated outliers for my win% variable as some players were traded mid season, I took the average for the teams that they played on. Also this data set was  organized based on the top 50 players and by the most amount of games played.
