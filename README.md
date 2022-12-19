# PyPoll_Challenge



## Overview of Election Audit



## Purpose

Analyze a CSV file that includes ballots for a US congressional precinct in Colorado. A report will be generated that will show the total number of votes, the percentage and total votes won by the candidates, and determine the winner. An analysis will also be provided that shows how many votes were cast by each county, including the percentage of the total votes cast.
___________________________________________________________________________________________________________________________________________________________

## Election-Audit Results

- Total votes: 369,711
- County results:
	- Jefferson: 10.5% (38,855)
	- Denver: 82.8% (306,055)
	- Arapahoe: 6.7% (24,801)
- Denver had the largest number of votes at 306,055
- Candidate results:
	- Charles Casper Stockham: 23.0% (85,213)
	- Diana DeGette: 73.8% (272,892)
	- Raymon Anthony Doane: 3.1% (11,606)
- Diana DeGette won the election with 272,892 votes, 73.8%

<img width="416" alt="image" src="https://user-images.githubusercontent.com/114355199/208540784-d6ccc1ea-91bd-410d-ba92-8c03c4140b21.png">

__________________________________________________________________________________________________________________________________________________________

## Election Audit Summary

The script provided in this project can be used to audit other elections. The script is based on a CSV file that contains three columns, Ballot ID, County, and Candidate. The script will read the CSV file, process the data then calculate various metrics that include the total number of votes cast, the percentage and number of votes won by each candidate, the total number of votes cast in each county, and the percentage of county votes from the total.

The script is flexible and could be used and modified for any election. The input file would need to be changed to reflect the ballots of the specific election. This would include the ballot ID, county, and candidates.

The script could also be modified for use in local or state elections. For example, for a local election, the county column could be changed to include the city's districts. For state elections, the county column could be changed to include the state's counties.


### Requirements

#### This script requires the following Python modules:

- csv
- os

### Input Data

The input data for this script is a CSV file containing the results of an election. The file should have the following structure:
![FileStructure](https://user-images.githubusercontent.com/114355199/208540220-c43c6ea5-ce14-4168-803e-c47c33e58c25.png)


The first row of the file should contain the column headers. The script expects the CSV file to be in the "Resources" directory, and the file should be named "election_results.csv".


### Output Data

The script creates a text file displaying the results of the election analysis. The file is saved in the "analysis" directory, and is named "election_results.txt". The file shows the following information:

- The total number of votes
- The percentage of votes won by each candidate, along with the total number of votes the candidate received
- The percentage of votes won by each county, along with the total number of votes each county received
- The winner of the election

### Modifying the Script for Other Elections

To use this script for a different election, the following modifications should be made:

1. Change the input data file to match the election's results.
2. Modify the list of candidate options to include the names of all the candidates running in the election.
3. Modify the list of county options to include the names of all the counties or other relevant geographic divisions involved in the election.
4. Change references to "county" in the code to reflect the geographic divisions for the election.
5. Modify the script as needed to calculate the appropriate metric for determining the winner of the election (e.g. total votes, electoral votes, etc.).
