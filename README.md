# workplace-research-project
All code pertaining to The Workplace research project.

Data can be downloaded from https://data.stackexchange.com/workplace/queries.

## Code Files

### Gender-part2.ipynb

**Purpose:** Script used to find the distribution of posts by each gender, by dominant topic.

**Files In:** doc-topics-65.txt, Users-location.csv, gender-part1.csv, gender-complete.csv

**Files Out:** gender-final.csv, gender-grouped-uniquified.csv

### Gender.ipynb

**Purpose:** Script used to attach the posts to the authors (userId).

**Files In:** Posts.csv, Users.csv

**Files Out:** gender-part1.csv

### RQ2-Impact.ipynb

**Purpose:** Script used to find the absolute impact of the dataset.

**Files In:** doc-topics-65.txt, Posts-update.csv

**Files Out:** rq2_absolute-impact3.csv

### RQ4-Time.ipynb

**Purpose:** Script used to analyse data for RQ4.

**Files In:** doc-topics-65.txt, Posts-update.csv

**Files Out:** median-time-difference.csv

### RQ4.ipynb

**Purpose:** Script used to analyse data for RQ4.

**Files In:** doc-topics-65.txt, Posts-update.csv

**Files Out:** rq4-sum.csv

### Reputation.ipynb

**Purpose:** Script used to determine the reputation of each user.

**Files In:** doc-topics-65.txt, Posts-for-reputation-cut.csv

**Files Out:** reputation-pivot-table.csv, reputation-topic-count-aggregated.csv

### absolute-impact.ipynb

**Purpose:** Script used to find the absolute impact of the dataset.

**Files In:** doc-topics-65.txt, Posts-update.csv

**Files Out:** Posts-by-month.csv, absolute-impact3.csv

### accepted-answers.ipynb

**Purpose:** Script used to remove answer posts from the dataset that were not marked "accepted". It takes the original dataset and combines them into one, while removing the accepted answers (Note: Posts-update.csv and Posts_v2.csv contain the same dataset).

**Files In:** Posts1.csv, Posts2.csv, Posts3.csv

**Files Out:** Posts-update.csv

### data_processing.ipynb

**Purpose:** Script used to do the preprocessing of posts. This includes removing HTML characters, spaces, special characters, numbers, punctuation, and stop words. Porter Stemming was used to get the roots of words.

**Files In:** en.txt, Posts_v2.csv

**Files Out:** Posts_v2.csv

### finding-coherence.ipynb

**Purpose:** Script used to check the coherence of different runs of k topics with the MALLET algorithm.

**Files In:** topic-state-70.txt, Posts1.csv, Posts2.csv, Posts3.csv

**Files Out:** None

### topic-distribution.ipynb

**Purpose:** Script for figuring out the dominant topic of each post based on the results from MALLET.

**Files In:** doc-topics-65.txt, Posts-update.csv

**Files Out:** topic count.csv, Topics folder

### user-frequency.ipynb

**Purpose:** Script used to count how many posts each user posted.

**Files In:** user-freq.csv

**Files Out:** user-frequency2.csv

### write_to_txt.ipynb

**Purpose:** Script that converts each line of the dataset into a seperate text file. The text files are named with the post ID, and the body has the cleaned data. This is the format required to run the MALLET algorithm.

**Files In:** Posts_v2.csv

**Files Out:** None

