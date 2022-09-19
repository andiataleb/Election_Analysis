# Election_Analysis

## Project Overview
In this project I've assisted a Colorado Board of Elections employee to complete an election audit for a local congressional election. I was tasked to write a code using Python to automate the process for them to be able to find the total number of votes, the total number of votes for each candidate, the percentage of votes for each candidate as well as enabling them in identifying the county with the largest turnout, each county's total number of votes and percentage of votes for each county. This code can be used in other local elections audits with slight modifications.

Steps that were neccessary for performing this audit was:
1. Calculate the total number of votes cast.
2. Getting a complete list of candidate and county names.
3. Calculationg the total number of votes cast in each county.
4. Calculating the pecentage of votes cast in each county.
5. Identifying the county with the largest turnout.
6. Calculationg the total number of votes each candidate received.
7. Calculationg the percentage of each candidate's vote.
8.Determinig the winning candidate based on popular vote.

## Resources
- Data Source: election_results.csv
-Software: Python 3.7.6, Visual Studio Cade, 1.71.0

## Election Audit Results
The results of this congressional election audit are as follow:
- The total number of votes cast in was "369,711".
- Each county votes and their percentage:
Jefferson: 10.5%(38,855)
Denver: 82.8%(306,055)
Arapahoe: 6.7%(24,801)
- The County with the largest turnout was Denver.
- The candidates who received a vote in the election were:
1. Charles Casper Stockham
2. Diana DeGette
3. Raymon Anthony Doane
- The total number of votes for each candidate is as follow:
Charles Casper Stockham: 23.0% (85,213)
Diana DeGette: 73.8% (272,892)
Raymon Anthony Doane: 3.1% (11,606)
- The winner of the election was:
Diana DeGette with the total number of 272,892 votes which is 73.8% of the votes.

## Election Audit Summary
This script that was written for this election can be a valuable tool to be used for other elections in any precinct with some minor modifications. To give some examples of the changes that needs to be done on the script for different elections I can point to the path that needs to be addressed to open the results and the path that should be used to save the analysis on.
For this purpose this line of script needs to be midified based on the location of the designated files:
`file_to_load = os.path.join("Resources", "election_results.csv")`
`file_to_save = os.path.join("analysis", "election_analysis.txt")`

Additionally, depending on the structure of the CSV file containing the election results, the number of row indexes to get the name of candidates or counties should be changed.
`candidate_name = row[2]` ` county_name = row[1]`
This code can be used to audit any size of election data with correct modifications
