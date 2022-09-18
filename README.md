# automatetheboringstuff
Beginner Projects

**Project 1: The Collatz Sequence**

collatz.py

The Collatz Sequence
--------------------
Write a function named collatz() that has one parameter named number. If number is even, then collatz() should print number // 2 and return this value. If number is odd, then collatz() should print and return 3 * number + 1.

Then write a program that lets the user type in an integer and that keeps calling collatz() on that number until the function returns the value 1. 

Remember to convert the return value from input() to an integer with the int() function; otherwise, it will be a string value.

Hint: An integer number is even if number % 2 == 0, and it’s odd if number % 2 == 1.

The output of this program could look something like this:

Enter number:
3
10
5
16
8
4
2
1

------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Input Validation

Add try and except statements to the previous project to detect whether the user types in a noninteger string. Normally, the int() function will raise a ValueError error if it is passed a noninteger string, as in int('puppy'). In the except clause, print a message to the user saying they must enter an integer.


**Project 2: Conway’s Game of Life**

Conway’s Game of Life is an example of cellular automata: a set of rules governing the behavior of a field made up of discrete cells. In practice, it creates a pretty animation to look at. You can draw out each step on graph paper, using the squares as cells. A filled-in square will be “alive” and an empty square will be “dead.” If a living square has two or three living neighbors, it continues to live on the next step. If a dead square has exactly three living neighbors, it comes alive on the next step. Every other square dies or remains dead on the next step. You can see an example of the progression of steps in Figure 4-8.

![Four steps in a Conway’s Game of Life simulation](https://user-images.githubusercontent.com/41771221/190932788-dcd06f94-5f3e-4040-9538-cc024b48debe.jpg)

Figure 4-8: Four steps in a Conway’s Game of Life simulation

Even though the rules are simple, there are many surprising behaviors that emerge. Patterns in Conway’s Game of Life can move, self-replicate, or even mimic CPUs. But at the foundation of all of this complex, advanced behavior is a rather simple program.

We can use a list of lists to represent the two-dimensional field. The inner list represents each column of squares and stores a '#' hash string for living squares and a ' ' space string for dead squares. Type the following source code into the file editor, and save the file as conway.py. It’s fine if you don’t quite understand how all of the code works; just enter it and follow along with comments and explanations provided here as close as you can:
