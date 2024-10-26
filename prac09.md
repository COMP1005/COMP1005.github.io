---
title: "Prac09: Quality and Testing"
---

:::::::::::::::::::::::::::::::::::::: questions 

- Why should we care about code quality?
- How can we improve code quality?
- What tools are available to assist with creating and assessing code?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

1. Understand the need for quality in software, how to assess it and how to achieve it
2. Have an awareness of formal approaches to managing and specifying projects
3. Understand the value of version control in software projects
4. Access and assess packages in the Python Package Index
5. Understand the basics of software testing and its importance

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

- The is a whole field, "Software Engineering", that deals with ensuring software quality. We have touched on some of the areas involved so that you are aware of them.
- Detailed coverage is beyond this unit, however, if you are involved in more complex software development in the future (client, team member, coder, tester) there are many resources available to support you.
- In all of our coding, we should consider software quality and ways to test our code to be confident it performs as intended.
- Tools that can support coding (version control, IDEs, co-pilot/genAI) can improve productivity and reduce risk of losing data/code
- WARNING: you will always need to check back that the code/system you are developing matches the **requirements** - a perfect system that doesn't solve the problem is worthless (actually it's worse than that, as all the tme and money spent in development has been wasted). 

:::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::::::::: checklist

### Reflection
 
1. **Knowledge:** ?
3. **Comprehension**: ?
5. **Application**: ?
7. **Analysis**: ?
9. **Synthesis**: How does having a well-defined program and test design help with managing larger projects? (larger = longer duration, more coders)
10. **Evaluation**: ?
    
::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::::::::: challenge

For those who want to explore a bit more of the topics covered in this practical. Note that the challenges are not assessed but may form part of the prac tests or exam.

1. For a given programming scenario, go through the process of test driven development. Test accounts, past PT1?
   1. Set up a table for your test cases
   2. Write code for your tests cases
   3. Write code to implement the problem solution

::::::::::::::::::::::::::::::::::::::::::::::::
