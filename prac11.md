---
title: "Prac11: Applications - Science and Engineering"
---

:::::::::::::::::::::::::::::::::::::: questions 

- To be updated

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

1. Under Construction

::::::::::::::::::::::::::::::::::::::::::::::::

### Introduction

In this practical you will read and write data using text files. You will also work with some grid-based 
algorithms – testing out different values to see how their parameters affect outcomes. We will also 
look at using list comprehensions to simplify our code.

### Activity 1 - Reading a CSV File

Type in the following code, weather.py, for displaying the weather stored in a file:

```python
#
# weather.py: Print min and max temps from a file
# (source: http://www.bom.gov.au/climate/)

import matplotlib.pyplot as plt

fileobj = open(‘marchweather.csv’, ‘r’) 

# add file reading code here 
line1 = ??
line2 = ??

fileobj.close()

mins = # add splitting code here, each stirng value will need to be coverted to float
maxs = # add splitting code here 

dates = range(1,32)

plt.plot(dates, mins, dates, maxs) 
plt.show()
```

Modify the code to read the data from the marchweather.csv file – available on Blackboard. 
You should download it to your Prac5 directory, look at its contents and format, then modify 
the code accordingly. **Hint:** look at split method, and list comprehensions in lecture slides.

### Submission

Update the README file to include all files created in this practical.

All of your work for this week’s practical should be submitted via Blackboard using
the Practical 05 link. This should be done as a single "zipped" file.
Submit the resulting file through Blackboard. (refer to Practical 00 or 01 for instructions
on zipping files.
 
There are no direct marks for these submissions, but they may be taken into account 
when finalising your mark for the unit. Go to the Assessment link on Blackboard and 
click on Practical 03 for the submission page.

### And that's the end of Practical 05!

::::::::::::::::::::::::::::::::::::: keypoints 

- FIXME

:::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::::::::: checklist

### Reflection
 
1. **Knowledge:** What are the three different read methods we can use on a file? What is the difference between them?
3. **Comprehension**: What does the line file2.write(...) do in Activity 4?
5. **Application**: Given the Game of Life rules, what would happen to the centre
cell in the following cases:
![fig/P05GOLReviewQ.png](GOL images)
7. **Analysis**: What variation of “neighbours” does ```heatsource.py``` use? How would the code change if it were to use the other neighbour approach?
9. **Synthesis**: How would you create a heat source input file with a 4x4 heat source in the centre of the 10x10 grid?
10. **Evaluation**: Name two advantages to reading initial data from a file as in the updated ```heatsource.py```.
::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::::::::::: challenge

For those who want to explore a bit more of the topics covered in this practical. Note that the challenges are not assessed but may form part of the prac tests or exam.

1. Follow the workflow from Activity 3 to process and plot **February** weather data.
2. For students based in Australia, find another country's weather data sharing site, or an international one
If you are not in Australia, see if you can find you local government's weather data sharing site. 
4. Find and download some **Game of Life*** code and get it running.
 
::::::::::::::::::::::::::::::::::::::::::::::::
