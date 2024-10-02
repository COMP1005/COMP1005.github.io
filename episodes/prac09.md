---
title: "Prac09: Quality and Testing"
---

:::::::::::::::::::::::::::::::::::::: questions 

- Why should we care about code quality?
- How can we improve code quality?
- What tools are available to assist with creating and assessing code?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

1. DRAFT

::::::::::::::::::::::::::::::::::::::::::::::::

### Introduction

We will be using python notebooks for this practical to keep track of our steps and get use to how they work. The activities will surround the use of pandas to work with structured data.

### Activity 1 - Running a Jupyter notebook

Create a Prac09 directory for this practical and change into it.

Type: jupyter notebook at the command line to start the jupyter notebook in your browser.

Once in the dashboard for jupyter, create a new notebook with the default kernel and call 
it "tuple" (creates the file "tuple.ipynb")

Create a markdown cell to give a short description: "Testing out jupyter notebook with Tuple task"

Create a code cell and type in the following:
```python
tup1 = ('spam', 'eggs', 42) 
tup2 = (1, 4, 9, 16, 25 ) 
tup3 = "yes", "oui", "ja", "si" 
print(tup1)
print(tup2) 
print(tup3)
```

### Submission

Update the README file to include all files created in this practical.

All of your work for this week’s practical should be submitted via Blackboard using
the Practical 09 link. This should be done as a single "zipped" file.
Submit the resulting file through Blackboard. (refer to Practical 00 or 01 for instructions
on zipping files.
 
There are no direct marks for these submissions, but they may be taken into account 
when finalising your mark for the unit. Go to the Assessment link on Blackboard and 
click on Practical 09 for the submission page.

### And that's the end of Practical 09!

::::::::::::::::::::::::::::::::::::: keypoints 

- FIXME

:::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::::::::: checklist

### Reflection
 
1. **Knowledge:** What is the language used for formatting an Jupyter Notebook?
3. **Comprehension**: Why did we need to use ```../Prac07``` to run the file in Activity 3?
5. **Application**: How would you do the following in Jupyter Notebook?
 1. Execute the current cell
 2. Clear all the output for all cells
 3. Run all cells
 4. Change a cell from coe to markdown
7. **Analysis**: Pandas lets us easily create a new column in a dataframe e.g. ```df = df.assign(temprange = df["Maxtemp"] - df["Mintemp"]). What code would you write to:
  1. Print the values in the new column
  2. Give descriptive information for the new column
  3. Plot only the new column's data
9. **Synthesis**: We went through a workflow in Activity 4 to count words in the story Rumplestiltskin. What parts of the workflow would change to analyse "THE ELVES AND THE SHOEMAKER", also in Grimm's Fairytales
10. **Evaluation**: Compare the datatypes: Pandas Dataframes, Numpy arrays and lists
  1. What are the features of each?
  2. When would you choose to use each of these datatypes?
::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::::::::: challenge

For those who want to explore a bit more of the topics covered in this practical. Note that the challenges are not assessed but may form part of the prac tests or exam.

1. TBA

::::::::::::::::::::::::::::::::::::::::::::::::
