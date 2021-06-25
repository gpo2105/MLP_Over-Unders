# Bias in O/U Lines for MLB
 
## Introduction
Besides picking Winners & Losers, the most common form of sports gambling is to predict whether a the total number of runs (or points) scored will or will not go over a certain level.

As with other wager types, a sportsbook will set a 'line' that, based on their own beliefs, makes both outcomes equally likely.  This line will come with 'odds' that will insure the book makes a profit, assuming both sides of the bet see even amounts bets are made.  In order to keep both sides even, a book will adjust the line or the odds to entice gamblers to bet on the less-favored outcome.  This iterative process continues until a closing line is set, usually when the game begins.
 
 Most gambling research focuses on finding a better prediction for the total runs.  While much of the inputs will be similiar, this project instead looks to predict when the book's estimation is too low (i.e. when the OVER bet wins).  

 ## Data
 ### Sources
 Finding historical data for MLB games was surprisingly difficult--from what I found no legitimate sportsbook publishes such data.  However, through other research citations, I was able to find a website, [Sportsbook Review Online](https://www.sportsbookreviewsonline.com/scoresoddsarchives/mlb/mlboddsarchives.htm), which provides such data for all sports, including MLB going back to 2010.  For all other data, I relied on [Baseball-Reference](Baseball-Reference.com) which is widely-recognized as the most reliable and granular resource for all things MLB.

### Collection
The gambling data was easily retrieved by downloading excel files directly from the website.  These files, of course, included Over/Under opening & closing lines and odds along with other gambling data.  They also provided data about the matchup--Home & Away team and pitchers--and the runs scored by each team.

Data from Baseball-Reference was a bit more difficult to retrieve.  Some data--specifically team annual statistics--was easily downloaded.  Game-by-Game statistics and player-specific metrics had to be retrieved through webscrapping.  Fortunately, the website follows strict templates so once one type of page was succesfully scrapped, it was just a matter of iteration to collect the rest.  

(It is worth noting that at the last hour, I discovered a not-widely-advertised API for some of the data of interest.)


 


 
