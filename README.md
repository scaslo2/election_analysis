# Election_Analysis
## Overview of Election Audit
A Colorado Board of Elections employee has given the following tasks to complete the election audit of a recent local congressional election. 

1. Calculate the total number of votes cast.
2. Get a complete list of candidates who received votes.
3. Calculate the total number of votes and the percentage of votes each candidate received.
4. The voter turnout and percentage of votes for each county.
5. The county with the highest turnout.
6. Determine the winner of the election based on popular vote.

## Resources
- Data source: election_results.csv
- Software: Python 3.6, Visual Studio Code 1.56.2

## Election-Audit Results:
The analysis of the election show that:
1. There were 369,711 votes cast in the election.
2. The candidates were:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
3. The candidate results were:
  - Charles Casper Stockham received 23.0% of the vote and 85,213 number of votes.
  - Diana DeGette received 73.8% of the vote and 272,892 number of votes.
  - Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes.


4. The voter turnout for each county was:
  - Jefferson: 10.5% (38,855 voters)
  - Denver: 82.8% (306,055 voters)
  - Arapahoe: 6.7% (24,801 voters)

5. Which county had the largest number of votes?
  - Denver County had the largest number of votes, with 306,055 votes and 83.8% of the votes.

6. The winner of the election was:
  - Diana DeGette, who received 73.8% of the vote and 272,892 number of votes.


## Election-Audit Summary
Given how efficient this analysis was, we can look to use the same script for any election so long as we make sure to some small modifications.

In our script we are able to easily identify and select the candidate name and county name by referencing the row index. For example we know that we can get the candidate name from column C or row[2] and we can get county name from column B or row[1] (see image below).
![County and Candidate Names] ()

For future elections, we may not have standardized data formats and therefore it would be best practice to modify this section of the code to be more dynamic - to search for headers that identify the county and candidates names.

