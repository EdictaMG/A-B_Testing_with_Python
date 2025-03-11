# A/B Testing with Python

In this repository I share my process of performing an A/B test using Python.  For this project, I aimed to answer the question: **Which version of a button in a store website homepage has a higher click-through rate (CTR)?**

The relevant business implication of a website version button having a higher CTR is its improved effectiveness at capturing user attention and prompting them to take the desired action compared to the original version.

## Situation
For this project I return to working with Eniac, a fictitious company in Europe that sells tech products and accessories (previous repositories in which this company is featured are *“Data_Exploration_with_SQL_and_Tableau”* and *“Data_Analysis_with_Python."*)  Eniac is interested in improving the rate of sales made of its iPhone 13 through the clicking of a button that appears in its homepage. 

## Approach
* I perform an A/B test applying chi-square testing on four button versions (A, B, C and D) where A is the original version (control).
* I present a longer manual testing approach, as well as a quicker “coder’s” approach for comparison.
* The statistical significance chosen is 95% with a minimum detectable effect set at 20%.
* The primary metric chosen to compare the different versions is the conversion rate of the iPhone 13 “confirmed” purchases achieved through clicking a specific button (nominator) against the overall click-rate of the same button (denominator).
* To determine the winning button version, I apply a quick approach, using a table of observations to calculate percentages of clicks to no-clicks.  The version with the highest percentage is deemed the winner.  I also apply a “Post-Hoc” test on the various version permutations to determine if any particular version performs significantly better than the rest.

## Files

### Data
- **eniac_a:** test version A data
- **eniac_b:** test version B data
- **eniac_c:** test version C data
- **eniac_d:** test version D data

### Scripts
- **AB_testing_Eniac:** notebook going through the whole AB process, including quicker and longer approaches.

## Using the files

- Update urls in notebook with actual location of data files.
- If data files have been stored in Google Drive, ensure links have ”editor” rights in order to be able to read them into the notebook.

## Languages and Libraries Used

- Python (3.12.4)
- Pandas (2.2.2)
- Numpy (1.26.4)
- Scipy (1.13.1)
- Seaborn (0.13.2)
- Matplotlib (3.8.4)

## Tools used

- Google Colab for notebook
- Google Drive
