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

![election analysis results](https://github.com/scaslo2/election_analysis/blob/a832c4d652ca47212fc9be325a557d13a2e28173/election_analysis_results.png)

## Election-Audit Summary
Using this script, we are able to analyze huge datasets in a matter of seconds. This can be a critical tool for future election audits, to analyze results significantly faster and with significantly more accuracy than before. With only a few modifications, this same tool can be applied to any election.

In our script we are able to easily identify and select the candidate name and county name by using the row[] array. For example, after looking at the .csv, we know that we can get the candidate name from column C or row[2] and we can get county name from column B or row[1].
![County and Candidate Names](https://github.com/scaslo2/election_analysis/blob/main/find%20county%20and%20candidate%20name.png)

For future elections, we may not have standardized data formats and therefore it would be best practice to modify this section of the code to be more dynamic - to be able to search for headers that identify the county and candidates names. Another way around this would be to add a section at the beginning of the script that would format the data for us. 


Given that we only analyzed a state election if we want to use this same script for a different type of election, i.e. a presidential election, we would need to edit our variables. In our script we look at the county level:
![County Names](https://github.com/scaslo2/election_analysis/blob/728192157a2e06fcc7639b2cf8cf2163e98ef73d/county_info.png)

In a presidential election, we may want to analyze data for the state level. We could add to or alter the scipt above to have a list of states and a dictionary of the number of votes by state. We can then use this to show things like the state with the most number of votes for a president, the distribution of votes by state, etc. 

With these small modifications we can utilize this script for any type of election and make sure to analyze our data in a more efficient manner. 
