# Functions
At this point, you can call functions and you can play around with loops, ifs, and perform basic operations. However, a lot of times you'll want to be able to make your own functions. When you have an extremely large (thousands of lines) codebase, reusing code where you can is *extremely* important. For this, we can make our own functions that we can call in our program. This means this code would only be defined in one place and we can call it from other locations. 

Functions usually take an input (Console.WriteLine() takes in a value of any type for example) and then return an output (Console.ReadLine() returns a string typed by the user).

We can make our own functions similar to that, via "declaring" a function. The syntax to declare a function is
```CSharp
static output_type name_of_function(input_type input_name) {
    //code here
    return output; //anything following a return is the output of the function.
}
```
If that looks confusing, here's an example of us making our own "print" function that prints a value on screen via Console.WriteLine()

```CSharp
static void print(string val){ //function that takes in a string named value. 
    //void means there is no output.
    Console.WriteLine(val);
}
```
Put this function declaration outside of ``static void Main(string[] args){}``, and inside of Main call ``print("test");`` This should print test into a cmd. Your final code would look something like this:

```CSharp
class Program{
    static void Main(string[] args){
        print("hi");
        Console.ReadLine();
    }
    static void print(string val){
        Console.WriteLine(val);
    }
}
```

Chances are you're extremely confused by all this right now, but try making your own functions.

For example, a function that takes a number, and checks if it's even could be written like this:

```CSharp
static bool isEven(int num){
    return num % 2 == 0; //this evaluates to true if num is even, and false if num is odd.
}
```

If you tried to Write it out to the screen with Console.WriteLine(isEven(5)), you'll see it mostly just works.

Exercises

1. see if you can make the if's and else if's in fizzbuzz go into a seperate function called fizzbuzz(), and have it return a string of either fizz, buzz, or fizzubzz. Use that function for the fizzbuzz game from the last lesson instead.
2. Make a function that checks if a number is odd called isOdd, that returns a bool.
3. Functions are expressions, and they are expressions *because* they can output a value, return is the statement used to signify what to output out of the function. If there's code below a return, will the the code run?

