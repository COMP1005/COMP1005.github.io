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

We will go through a short programming challenge to see how we develop code with high quality, and use testing to show that it meets our requirements - for valid and invalid inputs.

The coding probelm we will use was a Practical Test 1 in a previous semester. 

``` python
myname = "Tim the Enchanter"
myyear = 898

print(f"Hello, my name is {myname}.")

for i in range(myyear//100):
    if i % 10 == 0:
        print("*", end="")
print()
```

Modify the code in PracTest1.py to: 

1. Correct any errors - get the given code working  
2. Change myname and myyear to be your details 
3. Add code to ask the user their name and year of birth 
4. In an appropriate loop, test that the year is valid, ask them to re-enter the year and continue looping until it is valid
5. Based on the difference between your year and the user’s, print one of three comments – if you’re older, they’re older, or if you’re the same age. 
6. Print out a 3-layer birthday cake with the number of candles to match the user’s age. Candles are staggered in two layers (hint: i%2 for alternating) 

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
