# GradeBook Analyzer - Python CLI
Author: Yash Verma  
Roll No: 2501730159  
Course: B.Tech CSE (AI/ML)  
Date: 25-Nov-2025

## Purpose
A simple command-line GradeBook Analyzer that reads student marks (manual or CSV), computes statistics (average, median, min, max), assigns letter grades (A–F), shows pass/fail lists, and prints a formatted results table.

## Features
- Manual input of student names and marks
- CSV import (`Name,Marks`) support
- Calculates: Average, Median, Highest, Lowest
- Assigns grades: A (90+), B (80–89), C (70–79), D (60–69), F (<60)
- Pass/Fail filtering (pass >= 40) using list comprehensions
- Displays results in a neat table
- Menu loop for repeated runs

## Files in this repo
- `gradebook.py` : Main script (CLI)
- `students_sample.csv` : Sample CSV to test CSV import (optional)
- `README.md` : This file

## How to run
1. Make sure you have Python 3 installed.
2. Place `gradebook.py` and `students_sample.csv` in the same folder (if using CSV).
3. From the terminal / VS Code integrated terminal run:

4. ## CSV Format Example
CSV file must contain two columns: Name and Marks  
The first row should be the header.

Example:

Name,Marks
Alice,78
Bob,92
Priya,76
Amit,54
Simran,33

## Testing Instructions

### Test 1: Manual Input
1. Run the script using:
   python gradebook.py
2. Choose option 1 (Manual Entry)
3. Enter at least 5 students with different marks
4. Verify:
   - Average is correct
   - Median is correct
   - Highest & lowest student are correct
   - Grades match the score ranges
   - Pass/Fail list is correct
   - Table format displays correctly

### Test 2: CSV Input
1. Use the sample CSV file `students_sample.csv`
2. CSV content should look like:

   Name,Marks  
   Alice,78  
   Bob,92  
   Priya,76  
   Amit,54  
   Simran,33  

3. Run:
   python gradebook.py
4. Choose option 2 (Load from CSV)
5. Enter: students_sample.csv
6. Verify:
   - All student data loads correctly
   - Calculations (avg, median, min, max) are correct
   - Grades are assigned properly
   - Pass/Fail list matches marks
   - Table prints cleanly

### Test 3: Loop Functionality
1. After completing one run, choose “yes” when asked:
   do you want to continue? (yes/no)
2. Run new test (manual or CSV)
3. Finally choose “no” to exit the program.


