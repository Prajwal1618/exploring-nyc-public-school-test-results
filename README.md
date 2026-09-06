# exploring-nyc-public-school-test-results
Using data manipulation and summary statistics to analyze test scores across New York City's public schools!
# Exploring NYC Public School Test Result Scores

This project analyzes SAT performance across New York City public schools using math, reading, and writing test scores.

The analysis focuses on identifying schools with strong math performance, the top-performing schools based on combined SAT scores, and the NYC borough with the largest variation in SAT performance.

## Project Questions

The analysis answers the following questions:

1. Which NYC schools have the best math results?
2. What are the top 10 performing schools based on combined SAT scores?
3. Which NYC borough has the largest standard deviation in combined SAT score?

## Key Analysis

### 1. Best Math Results

Schools are considered to have the best math results if their average math score is at least 80% of the maximum possible SAT Math score of 800.

The qualifying schools are stored in:

`best_math_schools`

The DataFrame contains:
- `school_name`
- `average_math`

The results are sorted by average math score in descending order.

### 2. Top 10 Schools by Combined SAT Score

A combined SAT score is calculated by adding the average math, reading, and writing scores:

`total_SAT = average_math + average_reading + average_writing`

The top 10 schools are stored in:

`top_10_schools`

The DataFrame contains:
- `school_name`
- `total_SAT`

### 3. Borough with the Largest SAT Score Variation

The combined SAT scores are grouped by borough to calculate:
- Number of schools
- Average SAT score
- Standard deviation of SAT scores

The borough with the largest standard deviation is stored in:

`largest_std_dev`

The final result contains:
- `borough`
- `num_schools`
- `average_SAT`
- `std_SAT`

All numerical values are rounded to two decimal places.

## Key Findings

- The schools with the strongest math results were identified using a minimum average math score of 640.
- The top 10 schools were identified based on their combined average SAT scores.
- **Manhattan** had the largest standard deviation in combined SAT scores, with a standard deviation of **230.29** across **89 schools**.

## Tools & Technologies

- Python
- Pandas
- Jupyter Notebook

## Dataset

The project uses `schools.csv`, containing SAT performance data for New York City public schools.

## Project Structure

```text
Exploring-NYC-Public-School-Test-Result-Scores/
│
├── Exploring_NYC_Public_School_Test_Result_Scores.ipynb
├── schools.csv
└── README.md
