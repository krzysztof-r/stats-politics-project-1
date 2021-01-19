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

# Stats and Politics 2: Data Analysis
You've worked hard to clean and organize your data, and you were excited to draw insights from it. HOWEVER, when you return to check on the data you were storing online, you discover 70% of the demographic data has been wiped clean! You were able to deliver exact insights before, but now, you only have 30% of the data so you will have to turn to statistics to derive confidence in your analysis.

Your instructors will provide you with a new dataset for this analysis. The dataset will be composed of three files which you will have to join on the FIPS code using pandas

Which data columns are strongly or moderately correlated with the Republican vote share? Which columns are not? Does this pattern appear in both elections? Are these correlations statistically significant?

(Hint: You will need to research what qualifies as "strongly or moderately correlated" and provide the references that guided your decisions)

You are given the results of a poll of voting preferences for the 2016 US Election.
The sample size for the poll was 2,133. The sample was taken from eligible voters in the states of Florida and Pennsylvania.

Out of 1,042 respondents in Florida, approximately 46.84% would vote for the Democrats, and 45.22% for the Republicans
Out of 1,091 respondents in Pennsylvania, approximately 48.94% would be voting for the Democrats, and 41.2% for the Republicans
Run a hypothesis test to see whether voters' location is independent of their voting preference. Make sure to state your hypotheses and discuss your test result.

Fit and optimize linear regression and logistic regression models that predict 2016 relative vote share of the Republican party within a county using the county-level demographic data. For each model, answer the following questions:

What are the independent and dependent variables in this case? Which dependent variables are most positively and negatively predictive?
How good is the fit of your model? What metric is a good measure to evaluate your model? Discuss your results.
