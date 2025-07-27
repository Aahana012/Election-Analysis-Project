**Election Analysis Project**

**Introduction:**

This project analyzes polling trends and donation patterns for potential U.S. presidential candidates. It combines insights from polling data and donor information to understand public sentiment, candidate popularity, party affiliations, and funding dynamics leading up to the election.

**Datasets:**

1. Poll Data

•	File: poll_data.xlsx

•	Key Columns: candidate_name, answer, party, population, start_date, end_date

2. Donor Data

•	File: donor_data.csv

•	Key Columns: fund, party, filer_name

**Key Questions Explored:**

1.	Which political parties and candidates are most represented in the polls?

2.	What is the polling trend over time per candidate?

3.	How do different populations (e.g., likely voters vs. registered voters) affect poll counts?

4.	How does the number of polls per candidate vary monthly?

5.	How do vote counts differ between major candidates like Trump and Harris over time?

6.	What are the patterns in political donations across parties and filers?

7.	Who are the top 20 filers based on total funds raised?

**Tools & Libraries:**

•	Python: pandas, numpy

•	Visualization: matplotlib, seaborn

•	Date Handling: datetime, pandas Period

•	Notebook: Jupyter Notebook

•	External Data Reader: pandas_datareader (not used directly but imported)

**Analysis & Visuals:**

1. Poll Data Analysis

   •	Party-wise Poll Count: Countplot showing poll frequency across parties.

   •	Population Breakdown: Hue-based countplot for population type vs party.

   •	Poll Averages: Mean and standard deviation of poll results.

   •	Candidate Poll Frequency: Time series plots of poll frequency by candidate.

   •	Monthly Poll Trends: Line chart grouped by month showing poll count per candidate, colored by party.

   •	Vote Differences (Trump vs Harris): Time-based plot showing vote count difference between the two.

2. Donation Analysis

   •	Donation Distribution: Histogram showing donation spread.

   •	Common Donation Behavior: Filtered histogram for donations below $15,000.

   •	Party-wise Donation Spread: Histogram comparing party donations.

   •	Top Filers by Total Fund: Bar plot of top 20 political filers based on total donations.

**Party Color Mapping:**

party_colors = {
    'Democratic': 'blue',
    'Republican': 'red',
    'Independent': 'purple',
    'Libertarian': 'orange',
    'Green': 'green',
    'Constitution': 'yellow',
    'Unknown': 'black',
    'Other': 'gray'
}

**Insights:**

  •	Democrats and Republicans dominate polling and donations.
  
  •	Trump leads in poll count over Harris, with a notable vote difference.
  
  • Donations are heavily skewed, with most common donations under $15,000.
  
  •	Top filers include major political action committees and campaign organizations.

**Future Enhancements:**

  •	Introduce sentiment analysis on open-ended responses (if available).
  
  •	Use machine learning to predict voter behavior based on donation history.
  
  •	Include geographic analysis (state/county-wise) for deeper electoral insight.
  
  •	Clean and normalize candidate name variants more thoroughly.

**Appendix:**

  •	Mapping of candidate_name to party included.
  
  •	Charts saved using matplotlib, one exported as PNG (top_filers.png).
  
  •	vote_difference column engineered to study polarity between major candidates.

**Conclusion:**

This project blends polling data and campaign funding data to provide a holistic view of the U.S. electoral landscape. Through structured EDA and visual storytelling, it highlights trends in candidate popularity and financial backing, empowering stakeholders to interpret the pulse of the upcoming election.
