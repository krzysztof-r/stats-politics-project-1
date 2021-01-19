# stats-politics-project-1
Part 1 of the Stats and Politics - Cleaning and EDA Deliverable

# Stats and Politics 1: Cleaning and EDA
This assignment will involve analyzing data from previous United States presidential elections. These elections are held every four years, we have provided you with data for 2012 and 2016.

Download the election data below.

This is county-level data (a county is a contiguous administrative region within a state). In addition to the election data, census information is also included.

The data is split into three CSV files:

presidential_2012_votes.csv contains the number of votes for each major political party within each county for the 2012 elections.
presidential_2016_votes.csv contains the number of votes for each major political party within each county for the 2016 elections.
demographic_data.csv contains various census statistics for each county; these include things like the racial makeup of the population or the overall economic status.
Each county in votes.csv and data.csv is identified with a unique code. (This is called the FIPS code.)

The first part of this deliverable is all about importing and cleaning large datasets using Python.

Load up the votes.csv and data.csv files into a Jupyter notebook.

Part 1: EDA
Take some steps to clean the data. Some specific questions to consider:

What is the size of each data frame? How many rows? How many columns?

Look at the entire data set. Choose any 5 columns in the dataset. For each answer the following:

What are each of the columns measuring? i.e. explain your understanding of what this column represents, and why it might be important if we are trying understand the relationship between demographic metrics and how counties vote
Are the values categorical or numeric?
We also encourage you to mentally answer these questions for every column in the dataset.

Part 2: Cleaning
Are any columns duplicate or have duplicate information? If so, remove any duplicative columns (check the demographics file as well as votes files)
Are there any null values? If yes, clean the null values up using appropriate techniques (you will have to research the appropriate techniques, and explain your choices).
Remove the null values from the votes dataframe where the Candidate is other
Clean the null values using the appropriate techniques in the demographic data file and the vote files
You must deal with all null values. i.e. Your submission should not leave any null values.
Finally, augment the data so that each county contains the relative vote share for each party in each election. (e.g. For each county, if the Republicans got 2300 votes and the Democrats got 1900 votes, then the relative vote shares should be 54% and 46%. You should ignore votes that belong to other parties)
Part 3: Visualizations
Produce 4 unique and meaningful visualizations from this dataset. You can use the columns you've explored in part 2 if you wish, or new ones. Briefly discuss the insights you see in each visual.
(An example of a non-meaningful visualization would be a scatterplot of relative Republican vote share vs relative Democrat vote share, since this doesn't show anything interesting about the data).
