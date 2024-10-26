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

1. Correct any errors - get the given code working  (errors have already been removed)
2. Change myname and myyear to be your details 
3. Add code to ask the user their name and year of birth 
4. In an appropriate loop, test that the year is valid, ask them to re-enter the year and continue looping until it is valid
5. Based on the difference between your year and the user’s, print one of three comments – if you’re older, they’re older, or if you’re the same age. 
6. Print out a 3-layer birthday cake with the number of candles to match the user’s age. Candles are staggered in two layers (hint: i%2 for alternating)

```
SAMPLE OUTPUT
Hello, my name is Penny
What is your name? Sheldon
What year were you born? 1980
Birthday greetings, Sheldon the aged!
Here is a birthday cake with 44 candles!

 * * * * * * * * * *
*|*|*|*|*|*|*|*|*|*|
| | | | | | | | | |
####################
====================
####################
====================
####################
```

### Activity 1 - Program Logic

Before starting any coding, it is possible to get a feel for the "shape" of the program. This program will:

1. Ask for input
2. Validate it in a loop until the year is valid
3. Give one of three output options
4. Print out an ASCII birthday cake (in a series/nested loops).

We can then do a mapping from the program shape to the code structures required.

1. print/input
2. while loop - exit when year is valid
   - define invalid: could be year > 100 years ago, or >= the current year
4. if/elif/else - output text based on difference in birth years
5. calculate age
6. output cake based on age:
   - three loops for candles
   - loop for each layer (or strings) - width based on age
   - loop through alternating layers (cake and cream)

Make sure you understand how this matches up to the original specification. Sometimes a quick bit of coding can help you understand the problem - it will expose the parts of the problem you don't understand.

You might want to implement a solution to this in Python. Prehaps leaving out the cake printing, as that can take a while... a cake of the correct width without candles is enough for this activity.

### Activity 2 - Test Logic

The birthday cake scenario has **one user input: birth year** that affects the text that is output, and the size of the cake. If an invalid year is entered, the code will loop until it is valid. 

In the lecture, we introduced a Test Plan - a table where we can systematically define input combinations and the expected outputs. This could be completed before any code is written. Then, the code can be tested against the Test Plan, and the final column **Pass/Fail** completed with respect to the **Expected Result** column.

|Test # | Variable1 | Variable2 | Expected result | Pass/Fail |
|-------|----------|----|----|-----| 
| 1 | value1 | value2 | result1 | P/F |
| 2 | value3 | value4 | result2 | P/F |
| 3 | value4 | value6 | result3 | P/F |
| ... | ... | ... | ... | ... |

::::::::::::::::::::::::::::::::::::: 

## Writing a test plan: Testing... testing...

Looking at the birthday cake code, what inputs could you explore across a range of test cases to see if it is working correctly?

:::::::::::::::::::::::: solution 

## Solution

Enter "Bruce" **and then** something other than "Bruce" to test both paths through the code. 
Note that "Bruce" and "bruce" are not equal. Testing requires at least every path through the code is executed.

::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::

### Activity 4 - Test your birthday cake code


### Activity 5 - Hello chatGPT


### Activity 6 - Surprise packages

Across the semester, we have imported packages including matplotlib, numpy and random, and learnt how to write and import our own modules. The lecture explained the process to creating and listing our own packages in the Python Package Index.

In this activity, we'll look at the Python Package Index to see the range of packages available, and develop our spidey-senses to know which packages are "safe" and which might be more risky.



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
