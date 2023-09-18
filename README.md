# Analysis of US Crime Rates

## **Overview**
- **What problem is being solved?**
  
I was trying to find the property crime rate of all the schools together in each State of the US. I wanted to visualize and compare the different crime rates of US States together. 

- **Where is the information from?**
  
The information was taken directly from the US Federal Bureau of Investigation (FBI) 2015 crime database website.

- **Why is this interesting?**
  
Crime-related topics have always intrigued me to a certain extent so seeing the crime data set in the list of data really piqued my interest. I was interested to see which State had the highest crime rate and whether there is a trend with highly populated States (the results were actually completely different from what I expected)

## **Design Choices**

**What design choices were made and why were these choices made?**

The most important design choice that I had to make was the data type of each US State - an Enumeration or a string. At first, I thought a string would be a better idea since it was less complicated however, I thought the enumeration could provide more clarity on what the data was. When writing out my functions I realized that it would make sense for the states to be a "one of" because it more the code simpler to understand (even if there were 50 different cases).
Another important choice was to make sure that my crime rate functions didn't divide total property crime by zero enrollments. When dividing by zero, python gave a long error message of "not divisible by zero". To make this issue doesn't happen I also had to include an if condition in my rate function, if total enrollment is zero, automatically returns zero as the rate.

## **Problem Solving**
**Describes how the problem was solved**

After reading the info in the data set. I added up all the enrollment numbers of each state so that I would have the total enrollment for each state (50 functions for total enrollment per state). In those functions alone I wrote if and elif conditions so that each function would account for only one state). Then I repeated the same step only replacing enrollments by property crime to find the total property crime of each state (another 50 functions). The final calculation set was when I divided the value of total property crime by the total enrollments of each state only if their total enrollments or the inputted list of CrimeData was not zero. After obtaining the rates for every single, I made a function that took all the rates together and outputted a list of floats that represented the crime rate of each state. Finally, I made a visualization function that visualized each state and my calculations to display the property crime rate of all the schools together in each State of the US. The bar graph produced helped to visually see and compare the different crime rates of US States together.

## **Most Challenging**
**Discusses which part of the project was the most difficult and why.**

Typing out more than 250 functions for this project was the most difficult part. Due to the nature of the data and idea, I had to type a function for every single State and I had to make sure that there were helper functions for those functions present as well. Any additional functions that weren't used would be considered a waste of time and energy so I had to carefully think through what functions I needed to obtain the solution to my proposed problem. I had to be very careful with how I typed because a misspelling would give me a huge error saying the data is wrong and errors of such sorts. 

## **Future Work**
**Provides examples of ways in which systematic programming design skills can be used to solve problems in the chosen topic area in the future.**

My chosen topic area is Computer Science therefore the skills I learned in this class will definitely deem helpful in the future. The skills learned such as how to write data definitions functions, templates and analysis programs will definitely be used in the near future for my personal projects (although not the exact same formatting as learned, the fundamentals are very similar). These skills can also be used in future job opportunities.
