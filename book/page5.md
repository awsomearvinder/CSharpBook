# Control structures
With functions you can execute code and do *things.* That may include printing things to the screen but you can also draw on the screen, communicate with other devices on the internet - and just about anything really. But that in of itself isn't enough. You also need to be able to only run certain code if something evaluates to one thing or another. This is where if statements come in. If statements are a way to allow code to only run if a condition is true. If statements take a bool (the type that can only be true or false), and if the bool is true, the code in the if runs. If the bool is false, the code dosen't run. Syntactically, this is what they look like:
```CSharp
bool value = true;
if(value){
    //this code will only run if the value is equal to true. 
    //in this case the code will run.

    //note you can pass in an expression to where value is instead,
    //as long as the value simplifies to a bool. 

    //for example, if (value == true) is also valid to put where
    //value is, although in this case it's unessecary
}
```

If you wanted code to check if something the user input was even or not, you could do this:

```CSharp
System.Console.WriteLine("Please input a number");
int userInput = Int32.Parse(System.Console.ReadLine());

//all even numbers when divided by 2 have a remainder of 0.
if (userInput % 2 == 0){
    System.Console.WriteLine("The number you input was even!");
}
```

Another construct important to if's are else statements. else statements follow
after if, and run if the condition for the if was false. For example, extending the previous exercise:

```CSharp
System.Console.WriteLine("Please input a number");
int userInput = Int32.Parse(System.Console.ReadLine());

//all even numbers when divided by 2 have a remainder of 0.
if (userInput % 2 == 0){
    System.Console.WriteLine("The number you input was even!");
} else { 
    //All numbers that aren't even must be odd.
    System.Console.WriteLine("The number you input was odd!");
}
```
The final tidbit of knowledge relating to if's is that aside from if's and else's, you can also do else if like so:

```CSharp
System.Console.WriteLine("Please input a number");
int userInput = Int32.Parse(System.Console.ReadLine());

//all even numbers when divided by 2 have a remainder of 0.
if (userInput % 2 == 0){
    System.Console.WriteLine("The number you input was even!");
} else if (userInput % 2 == 1) { 
    //All numbers that have a remainder of 1 when divided by 2 are odd.
    System.Console.WriteLine("The number you input was odd!");
}
```

However, using an else if when an else by itself is enough if bad pratice - it adds complexity to your program for no gain, but when used in combination of if and else, it can be useful.
Note, you can use as many else if's after an if as you want, but only one else which must be the last. This makes sense because else only runs if all the others are false, there's no condition to a else like there is for else if or if's. 

Exercises:
1. Make a program that checks if a number is evenly divisible by 3 and 5, if it's divisible by 3, print Fizz, if it's divisible by 5, print Buzz, if it's divisible by 3 and 5, print FizzBuzz. Hint: (You'll need the && operator for this, as well as multiple else if's in a row.) For now you can make the number either hard coded or chosen by a user. Remember that ``System.Console.ReadLine()`` returns a string, not an int, so you have to convert it to a int before you use it. We'll expand this exercise in the next page.

