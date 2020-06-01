# Loops
Sometimes you need a certain bit of code to repeat. In order to accomplish this, C# gives you a construct called loops. There's a few different kinds of loops, however we'll only discuss while's and for's for now (although do while's and foreach exist as well. We may cover them later - however that is as of yet undecided.)

To start off with, while's are the easier of the two. While loops take a condition, much like an if, and while that condition is true the code keeps running. 

``while (true) {Console.WriteLine("test");}`` would keep printing test forever, whereas ``while(false){Console.WriteLine("test");}`` would never run the code. This is a useful construct because of variables. Using variables you can change the while's condition on the fly. It is worth knowing however, that the condition is checked *before* any given time the code runs, not *during*. For example, 
```CSharp
bool a = true;
while(a) {
    a = false;
    Console.WriteLine(a);
}
```
The above code would print false once and only once. Using this construct, you can use it to run code as long as some condition holds true. If you did the last exercise, you should of made a program that looked something like this (if it's somewhat different that's fine - there's different, even better solutions to this exercise):

```CSharp
int num = 4; 
if(num % 3 == 0 && num % 5 == 0) { //This condition must be first, try to figure out why.
    Console.WriteLine("FizzBuzz");
} else if (num % 3 == 0) { //why is this a else if and not a if?
    Console.WriteLine("Fizz");
} else if (num % 5 == 0) {
    Console.WriteLine("Buzz");
}
```
Were going to use this code along with a while loop to print Fizz for every number between 0 and 100 that's divisible by 3, buzz for every number divisible by 5, and fizzbuzz for every number that's divisible by 3 *and* 5.

Try doing it yourself before looking at the following solution! 

```CSharp
int num = 0;
while (num <= 100) {//this loop will keep repeating until num is bigger then 100
    if(num % 3 == 0 && num % 5 == 0) {
        Console.WriteLine("FizzBuzz");
    } else if (num % 3 == 0) {
        Console.WriteLine("Fizz");
    } else if (num % 5 == 0) {
        Console.WriteLine("Buzz");
    }
    num +=1; //every time this loop runs we add 1 to num.
}
```

Before you continue onwards to the exercises - I'd like to extremely incentivize slowing down from this point onwards. Exercises will be getting harder, and won't be as self explanatory. The concepts from this point onwards are going to be more annoying to get an intuitive grasp on. But having that intuitive grasp is important, as everything near the end of the book will assume you have that intuitive grasp on these things. So to reitterate, don't skip around and make sure you do these exercises.

Exercises

1. Make a loop that adds every number from 1 to 100, and then prints it to the screen.
2. Make a loop that finds if a number is prime. Hint: A prime number is evenly divisible only by itself and 1. 
3. Ask the user for a number of inputs to give, and then use a loop to run for that many inputs, and add up all of the user's inputs together. Print them to the screen. (hint: the fizzbuzz example may help here, instead of 100 you'll want the user's number.)
