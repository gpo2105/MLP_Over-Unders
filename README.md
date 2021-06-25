# Phase 3 Project-George Ogden
## Folder Explanations
### Code
The code folder contains the final notebook ('Final') which is an edited/cleaned up composite of the other notebooks in the folder.  Particularly, Data_Update_I, _II, & _III.

The other notebooks were either not used for the final results or include experimenting/random code.

### Data Folders
The 'Raw Data' folder contains excel, csv and txt files that were downloaded directly from baseball reference except for the odds_data file which came from my other data source.  

Base DFs contains pickled dataframes built from webscrapped data or the afformentioned downloaded data.  This covers all the team annual statistics, the various dataframes covering game information, individual types of team statistics (annual), and some dataframes that were built as part of my original feature data.

Similarly, 'Merged DFs' contains dataframes that were composites of the dataframes in 'Base DFs'.  This includes the combined game information, all the team annual statistics and the final database--before any transformations and splitting.

### Other
The image folder contains images used in the final presentaiton.

The glossaries folder contains word docs with definitions of each team statistic grabbed from baseball-reference.  This includes those that were ultimately excluded as features.

# Bias in O/U Lines for MLB
 
## Introduction
Besides picking Winners & Losers, the most common form of sports gambling is to predict whether a the total number of runs (or points) scored will or will not go over a certain level.

As with other wager types, a sportsbook will set a 'line' that, based on their own beliefs, makes both outcomes equally likely.  This line will come with 'odds' that will insure the book makes a profit, assuming both sides of the bet see even amounts bets are made.  In order to keep both sides even, a book will adjust the line or the odds to entice gamblers to bet on the less-favored outcome.  This iterative process continues until a closing line is set, usually when the game begins.
 
 Most gambling research focuses on finding a better prediction for the total runs.  While much of the inputs will be similiar, this project instead looks to predict when the book's estimation is too low (i.e. when the OVER bet wins).  

## Generalized Model
In theory, I suspect that a bookmakers' bias can be affected by four aspects of given baseball game: the quality of pitching and batting of both teams.  The first step of this project therefore was to find statistics that would best approximate these aspects.  Obviously, these stats needed to be available before the specific game begins so historical data was the most practical solution.  Ideally, the data would include all information up to the start of a given game.  

For pitching
 
 ## Data
 ### Sources
 Finding historical data for MLB games was surprisingly difficult--from what I found no legitimate sportsbook publishes such data.  However, through other research citations, I was able to find a website, [Sportsbook Review Online](https://www.sportsbookreviewsonline.com/scoresoddsarchives/mlb/mlboddsarchives.htm), which provides such data for all sports, including MLB going back to 2010.  For all other data, I relied on [Baseball-Reference](Baseball-Reference.com) which is widely-recognized as the most reliable and granular resource for all things MLB.

### Collection
The gambling data was easily retrieved by downloading excel files directly from the website.  These files, of course, included Over/Under opening & closing lines and odds along with other gambling data.  They also provided data about the matchup--Home & Away team and pitchers--and the runs scored by each team.

Data from Baseball-Reference was a bit more difficult to retrieve.  Some data--specifically team annual statistics--was easily downloaded.  Game-by-Game statistics and player-specific metrics had to be retrieved through webscrapping.  Fortunately, the website follows strict templates so once one type of page was succesfully scrapped, it was just a matter of iterating to collect the rest.  

(It is worth noting that at the last hour, I discovered a not-widely-advertised API for some of the data of interest.)

## Database


 


 
