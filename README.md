# A/B Testing with Python

This repository walks through the process of running an A/B test using Python to answer a simple but important question:

**Which version of a homepage button leads to the highest click-through rate (CTR)?**

Understanding which button design drives more clicks can directly impact sales by encouraging more users to take action—in this case, to purchase the iPhone 13.

## Situation
This project revisits **Eniac**, a fictional European company that sells tech gadgets and accessories (also featured in my repositories *Data_Exploration_with_SQL_and_Tableau* and *Data_Analysis_with_Python*). Eniac wanted to optimize the design of a button promoting iPhone 13 sales on their homepage by testing four variations.

The goal was to determine which version of the button (A, B, C, or D) leads to the most confirmed iPhone 13 purchases via clicks on that button. Version A served as the control (original design).

## Approach

- A/B testing was performed using the **Chi-square test** to assess statistical significance.
- I used two approaches:
  - A detailed step-by-step method (great for learning or presentations).
  - A streamlined “developer-style” version for quick analysis.
- **Confidence level:** 95%
- **Minimum detectable effect:** 20%
- **Primary metric:**  
  CTR, defined as  
  `confirmed purchases (via button click) / total button clicks`

To identify the best-performing version:
- I calculated the click-to-no-click ratio for each version.
- Then applied **Post-Hoc tests** on all version pairs to see which button significantly outperformed the others.

## Files

### Data
- `eniac_a.csv` — Data for version A (control)
- `eniac_b.csv` — Data for version B
- `eniac_c.csv` — Data for version C
- `eniac_d.csv` — Data for version D

### Scripts
- `AB_testing_Eniac.ipynb` — Notebook with the complete A/B testing workflow, including both manual and fast-track approaches.

## Using the files
- 1. **Update file paths** in the notebook to point to the actual location of your data.
2. If using **Google Drive**, make sure your file links have *“editor”* access so they can be loaded into the notebook.

## Languages and Libraries Used

- Python (3.12.4)
- Pandas (2.2.2)
- Numpy (1.26.4)
- Scipy (1.13.1)
- Seaborn (0.13.2)
- Matplotlib (3.8.4)

## Tools used

- Google Colab for running the notebook
- Google Drive for data storage
