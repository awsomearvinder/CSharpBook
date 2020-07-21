# Expressions

In C#, any line of code can either be an expression, or a statement. We'll cover statements later on, but expressions are anything that can evaluate to a single value. A good example of an expression is math, for example, 5+5 is an expression that will be evaluated to 10. All expressions will either be some operation, such as + or -, or something called a "function call"(which we will learn later) In order to show case this, we're going to write our first bit of code. For now, all of your code will go inside of this section here:
```CSharp
static void Main(string[] args){
    //in these curly brackets
}
```

You can ignore the namespace and class lines for now.

In order to show the value of an Expression, you can do something called printing a value. This will showcase the value of an expression on screen. In the area shown above, Write ``System.Console.WriteLine(5+5);``. If you run it at this point, you'll likely see a black window quickly appear and dissapear. In order to fix this make another new line and write ``System.Console.ReadLine();``

Your code should now look something like this:

```CSharp
static void Main(string[] args){
    System.Console.WriteLine(5 + 5);
    System.Console.ReadLine();
}
```

If all works well, you will see a 10 on screen. If you press enter the window will dissapear. All the important Math oeprators are Inside of C#, as shown by this table here:


| Operator | Meaning | 
|----------|---------|
| * | Multiplies|
| / | Divides | 
| + | Adds | 
| - | Subtracts |
| % | Divides and gets remainder |

Another important operation includes checking for equality, which output's True or False. 

For example, you can replace the 5+5 above with 5==5, what does it output? You can also check for inequality using != with for example with 5!=5

Some other operations include checking if a item is larger, for example 5 > 4, or checking if an item is smaller, with 5 < 4.

Exercises: 

1. Another set of operators are the >= and <= operators. Can you figure out what these do?

2. Without running it, try to figure out the output of (5 > 4) == (4 > 5) hint: you can compare equality on True and False as well, for example True == True would output True.

3. Check if C# preserves the order of operations in math
