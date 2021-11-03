# Machine-Learning-SQ2020
For training models check out the ipynb files

Allstar.csv Datasets

Brief description of what the dataset is about.

This dataset has a complete list of players that were selected as “All-Stars” in the NBA, and the number of selections for their career. An all-star selection is a notable selection that shows that a player is one of the 24 best players that season. The more all-star selections, generally the better the player was during his career.
Sizeof dataset: number of instances(rows)and attributes(columns).
503 rows × 2 columns
See Notebook.
Data samples:the first five and last data samples. 
	name	All Star Selections
Rk		
1	Kareem Abdul-Jabbar	19
2	Kobe Bryant	18
3	Julius Erving	16
4	LeBron James	16
5	Tim Duncan	15
...	...	...
499	Mo Williams	1
500	Kevin Willis	1
501	Metta World Peace	1
502	Trae Young	1
503	Max Zaslofsky	1
Brief Description of each attribute: what the attribute is about and its data type.
Attributes: Rk, name, Tot, NBA, ABA. 
Rk represents their rank for the number of all star selections.
name represents their first and last name, separated by a space.
Tot represents total all-star appearances.
NBA represents NBA all-star appearances. The NBA was from 1976-present.
ABA represents ABA all-star appearances. The ABA was from 1967-1976.
We felt it would not make sense for us to visualize all star appearances since there are over 4000 NBA players and only 504 players have ever made all star teams meaning that most of the data points will lie at 0.  
 
HallOfFamers.csv

Hall of Famers is a list of all players that have been inducted into the Hall of Fame. This is the highest honor of the NBA where only a select number of players make it.
Size Of Dataset: 199 rows × 4 columns
First 5, Last 5
1959	Chuck Hyatt	G	National championship (Pittsburgh, 1928, 1930)...	[3]
1959	Hank Luisetti	F	3 Pacific Coast Conference championships (Stan...	[4]
1959	George Mikan	C	All-America (DePaul, 1944–45); All-NBA First-T...	[5]
1959	John Schommer	G	Big Ten Championships (Chicago, 1907–09); All-...	[6]
1960	Vic Hanson	G	Helms Foundation Championship (Syracuse, 1926)...	[7]
...	...	...	...	...
2019	Bobby Jones	F	NBA champion (1983)4× NBA All-Star (1977, 1978...	[175]
2019	Sidney Moncrief	G	5x NBA All-Star (1982–1986)All-NBA First Team ...	[175]
2019	Jack Sikma	F/C	NBA champion (1979)7× NBA All-Star (1979–1985)...	[175]
2019	Teresa Weatherspoon	G	First WNBA player with 1,000 points and 1,000 ...	[175]
2019	Paul Westphal	G	NBA champion (1974)5× NBA All-Star (1977–1981)...	[175]
Attributes: Year, Inductees, Pos. Achievement
Year is the year they were inducted into the Hall of Fame.
Inductees is the first and last name of the hall of fame player.
Pos. is the position of the players.
Achievement is the accolade list of the players.
There was nothing to visualize in this dataset because we mainly used it for the names of hall of famers. The actual statistics that we will add to this dataset will be on the processed data file. 
 
MVPs.csv

MVP or Most-Valuable-Player is the best player during a season. It is the highest single-season honor.
Shape: 41 Rows x 2 Columns 
First 5, Last 5
	Player	Count
0	Kareem Abdul-Jabbar	 6
1	Michael Jordan	5
2	Bill Russell	5
3	Wilt Chamberlain	4
4	LeBron James	4
…       …..
36	Derrick Rose	1
37	Wes Unseld	1
38	Bill Walton	1
39	Russell Westbrook	1
40	NaN	1
Attributes: Name, Count
Name represents the first and last name of the player.
Count represents the number of MVPS the player has won in their career.
We felt it would not make sense for us to visualize MVPs since there are over 4000 NBA players and only 40 players have ever been MVPs. Most of the data points will lie at 0.  
 
Seasons_Stats.csv

Seasons_Stats is a list of every single season of a player and their respective statistics for that season. For example, if a player plays 15 seasons, there will be 15 rows for that player for each season they played. The stats will also be including in these rows.
See Notebook.
See Notebook.
Attributes: Year, Player, Pos, Age, Tm, G, GS, MP, PER, TS%, 3PAr, FTr, ORB%, DRB%, TRB%, AST%, STL%, BLK%, TOV%, USG%, OWS, DWS, WS, WS/48, OBPM, DBPM, BPM, VORP, FG, FGA, FG%, 3P, 3PA, 3P%, 2P, 2PA, 2P%, eFG%, FT, FTA, FT%, ORB, DRB, TRB, AST, STL, BLK, TOV, PF, PTS
Year represents the NBA season that the player played in.
Player is the player's first and last name.
Position is the player’s position.
Age is the player’s age.
Team is the team the player played for.
G through PTS are NBA statistics. All meaning of the stats can be found on the official NBA page. Some of these statistics will be dropped during pre-processing as they are irrelevant to the model of finding the probability of a player entering the hall of fame.
See Notebook.

allnba.csv

All-NBA is an end of the season award, awarded to the best players at each position. There is an All-NBA first team (the best at each position), second (second best), and third (third best). This award is generally considered more valuable than an all-star.
Size of Data Set: 277 rows × 5 columns
First 5, Last 5
name	1st Team	2nd Team	3rd Team	All-NBA Teams
Rank					
1	Kareem Abdul-Jabbar	 10	5	0	15
2	Kobe Bryant	11	2	2	15
3	Tim Duncan	10	3	2	15
4	LeBron James	12	2	1	15
5	Karl Malone	11	2	1	14
...	...	...	...	...	...
273	John Wall	0	0	1	1
274	Buck Williams	0	1	0	1
275	Charles Williams	0	0	0	0
276	Kevin Willis	0	0	1	1
277	Metta World Peace	0	0	1	1
Attributes: Rank, Name, 1st, 2nd, 3rd, Total
Rank represents how they rank in terms of the number of all-nba selections.
Name represents their first and last name.
1st, 2nd, 3rd represent the number of selections to each category.
Total is the total number of selections.
We felt it would not make sense for us to visualize all nba appearances either since there are over 4000 NBA players and only 277 players have ever made all nba teams meaning that most of the data points will lie at 0.  

player_data.csv

Player data includes every single player in the NBA since the NBA was created. Along with the name, it includes the years they played, their position, height, weight, birthdate and college. 
Shape: 4550 rows × 8 columns
First 5, Last 5
	name	year_start	year_end	position	height	weight	birth_date	college
0	Alaa Abdelnaby	1991	1995	F-C	6-10	240.0	June 24, 1968	Duke University
1	Zaid Abdul-Aziz	1969	1978	C-F	6-9	235.0	April 7, 1946	Iowa State University
2	Kareem Abdul-Jabbar	1970	1989	C	7-2	225.0	April 16, 1947	University of California, Los Angeles
3	Mahmoud Abdul-Rauf	1991	2001	G	6-1	162.0	March 9, 1969	Louisiana State University
4	Tariq Abdul-Wahad	1998	2003	F	6-6	223.0	November 3, 1974	San Jose State University
...	...	...	...	...	...	...	...	...
4545	Ante Zizic	2018	2018	F-C	6-11	250.0	January 4, 1997	NaN
4546	Jim Zoet	1983	1983	C	7-1	240.0	December 20, 1953	Kent State University
4547	Bill Zopf	1971	1971	G	6-1	170.0	June 7, 1948	Duquesne University
4548	Ivica Zubac	2017	2018	C	7-1	265.0	March 18, 1997	NaN
4549	Matt Zunic	1949	1949	G-F	6-3	195.0	December 19, 1919	George Washington University
Attributes: name, year_start, year_end, position, height, weight, birth_date, college
name represents the players first and last name.
year_start and year_end represent the start and end of their NBA career.
height, weight, birth_date are basic info about the player.
college represents the college the basketball player went to.
We mainly used this data file to grab names so there was nothing to visualize. 
(b) See Notebook.


We consolidated the dataset into two files. To consolidate the files, we had to first modify some of the excel files as the name attribute had special characters such as “*” at the end of the name. To do so, we had to mass delete a character from the excel file using some formulas. Additionally, in the notebook, we deleted irrelevant columns that provided no use in our overall goal of predicting Hall of Fame players. After that, we wanted to make sure each Hall of Fame row for the halloffamer.csv had columns of all-star appearances, all-nba appearances, MVP’s won, and their season statistics. This was all done in the notebook and consolidated into one file. 
Additionally, there were many NULL values as some of the older players didn’t have certain statistics since they didn’t exist back then. To deal with this issue, we filled in the NULL values with the average values as part of the data processing. Furthermore, we had to group by name and merge data frames to get the final halloffame.csv. This first file listed all the hall of fame players alongside their respective career statistics. This ultimately defines our baseline for getting into the hall of fame, as the averaged statistics represent the required career statistics to make it into the basketball hall of fame. This is incredibly important to our final goal because this baseline will be used to predict whether a current player will be able to enter the hall of fame by the end of their career. 
The second file was all the statistics from players up until 2017. Not much modification is needed for this file, however we did use this file to get statistics for the Hall of Famers. The only modifications we did to the file was remove irrelevant columns. 
Some of the interesting findings were that we found some Hall of Famers never were selected as an all-star. These hall of famers were obvious outliers and were mostly found in the pre-1980 NBA. We both discussed that we would like to remove those outliers as they would skew the data for the modern NBA, where you would have to be an all-star to make it to the Hall of Fame. Additionally, this was the case with all-nba selections and MVPs, however there were very few cases, and all of them were 30+ years old data. 
