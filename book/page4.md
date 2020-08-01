# Calling functions

At this point, you can make and work with data, but you can't actually *do* anything with that data. In order to do something with the data you need to use something called functions. Functions take in data, do a set of operations, then output some data back. ``System.Console.WriteLine()``is a function that takes in some object to be printed, prints it on screen, and then outputs a value of nothing.

Another function you've used is ``System.Console.ReadLine()`` in order to stop the program from closing. The reason why the program closes immediately without it is because the program very quickly runs everything in your code, and then exits automatically. ``System.Console.ReadLine()`` is a function that waits for a input typed by the user followed by enter, and then outputs that value. Until that function has an output, the program has to keep running. A function is an expression as well - in the case of ``System.Console.ReadLine()`` it evaluates to whatever the user types.

A simple program to showcase this would be: 
```CSharp
static void Main(string[] args){
    System.Console.WriteLine("What's your name?");
    string name = System.Console.ReadLine();
    System.Console.WriteLine("Hi " + name);
    System.Console.ReadLine(); // without this the program closes automatically again.
}
```

Exercises

1. Another function is ``System.Int32.Parse(string)`` which takes a string as it's input (in the parenthesis) and converts that string into a int. Using this and ``System.Console.ReadLine()`` (which returns a string) can you make a program that asks the users for two numbers, and then adds them?
2. What happens if you don't give the program from exercise 1 a number?
3. Play around a bit, get comfortable calling functions and working with the data they output. Check if numbers are equal, print them out, take user input and check if it's equal to something. After this point were going to start introducing more functions and making real programs. 
