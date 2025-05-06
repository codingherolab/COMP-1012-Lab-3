# COMP-1012-Lab-3

Download Here:[COMP 1012 Lab 3](   https://codingherolab.com/product/comp-1012-lab-3/    )

For Custom/Original Work email codingprolab@gmail.com/whatsapp +1(541)423-7793

Exercise 1: Sum of values in a file
Create a text file whose contents has one number per line. The file should look something line:

12
23
34
45
56
67
42
9001
Create a program that reads in the text file (you can hardcode the text filename into your program), computes the number of numbers in the file and the sum of all the numbers that are in the file. Then your program should print the number of numbers in the file and their sum.

Your output should look something like:

Number of numbers: 8
Total: 9280
Exercise 2: sum of digits
In class we’ve seen a for loop used to iterate over lines in a file. A for loop can actually be used to iterate over any sequence of values, so that also includes list and str types.

First, experiment a bit with the for loop – what happens when you write a for loop that iterates over a str?

word = "supercalafrajalisticexpealadocious"
for thing in word:
    print(thing) # what *is* thing?
Once you’ve worked this out, write a program that will prompt the user for a positive whole number. Using a for loop, calculate the number of digits and the sum of digits.

Your output should look something like (highlighted text means the user typed this in):

Provide a number: 321
There are 3 digits and the sum of the digits is 6.
Optional : Sanitize a string
Ask for a string from the user. Do the following operations:

Remove leading and trailing whitespace by using strip().
Remove characters: ~, ! and - by using replace().
Report the sanitized string back to the user.

Your output should look something like (highlighted text means the user typed this in, note here the spaces before and after the characters in the string):

Please input a string:     Hello - my name is Earl!    
Sanitized string: Hello  my name is Earl
Optional: Volume of a cone
Calculate the volume of a cone, given user input.

Prompt the user for the radius of the cone, and the height of the cone.

The equation to calculate the volume of a cone is:

V = πr2(h/3)

Report the volume to the user with two decimal places of precision.

Your output should look something like (highlighted text means the user typed this in):

What is the radius of your cone (in cm)?  12
What is the height of your cone (in cm)?  30
The volume is 4523.89cm^2
Optional: Binary to Decimal
Write a program that will prompt the user for a binary number (0s and 1s only) and convert that number to a decimal (base 10) integer.

Binary numbers are base 2 numbers that use only two digits to represent a number, 0 and 1. We can freely convert between decimal and binary using log, but we’re going to convert between these two bases using basic arithmetic and loops in Python.

As an example, in base 10 we can decompose a number into a set of products of powers of 10.

5629
|||└  9 * 10**0 (ones place)
||└-  2 * 10**1 (tens place)
|└--  6 * 10**2 (hundreds place)
└---  5 * 10**3 (thousands place)
You can calculate the number by a summation of each digit:

decimalValue = 9 × 100 + 2 × 101 + 6 × 102 + 5 × 103

In binary, we can decompose a number into a set of products of powers of two:

1001
|||└  1 * 2**0 (ones place)
||└-  0 * 2**1 (twos place)
|└--  0 * 2**2 (fours place)
└---  1 * 2**3 (eights place)
We can convert a binary number by calculating by a summation of the digits multiplied by powers of two represented by their place:

decimalValue = 1 × 23 + 0 × 22 + 0 × 21 + 1 × 20

Use a for to convert each bit into a decimal number. Have a running sum in your loop to do the summation.

Your output should look something like (highlighted text means the user typed this in):

Please input a binary number > 101010
The number in decimal is 42.
Things to think about:

What should the first power of 2 be? In our example it was 3, how would we represent that more generally based on something we can figure out about the str that was entered? (hint: we need to call a function!)
When looping over a str with a for loop, in what order are we iterating over values? That is, in terms of a string written out in the example, are we going from right to left or from left to right?
