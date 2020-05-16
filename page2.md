# Expressions

In C#, any line of code can either be an expression, or a statement. We'll cover statements later on, but expressions are anything that can evaluate to a value. A good example is some basic math, 5+5 is an expression that will get evaluated to 10. An expression is going to be either some operation, such as + or -, or a function, which is a piece of code you or someone else wrote that evaluates to a value. In order to show case this, were going to write our first bit of code. For now, all of your code will go inside of this section here:
```CSharp
static void Main(string[] args){
    //in these curly brackets
}
```

You can ignore the namespace and class lines for now.

In order to show the value of an Expression, you can do something called printing a value. This will showcase the value of a expression on screen. In the area shown above, Write ``System.Console.WriteLine(5+5);``. If you run it at this point, you'll likely see a black window quickly appear and dissapear. Inorder to fix this make a new line and write ``System.Console.ReadLine();``
Your code should now look like this:

```CSharp
static void Main(string[] args){
    System.Console.WriteLine(5+5);
    System.Console.ReadLine();
}
```

If all works well, you'll see 10 on screen. If you press enter the window will dissapear. Some other operations aside from normal math include checking for equality, which output's True or False. 

For example, you can replace the 5+5 above with 5==5, what does it output? You can also check for inequality using !=  for example with 5!=5

Some other operations include checking if a item is larger, for example 5 > 4, or checking if an item is smaller, with 5 < 4.

Exercises: 

Another set of operators are the >= and <= operators. Can you figure out what these do?

Without running it, try to figure out the output of (5 > 4) == (4 > 5) hint: you can compare True and False as well, for example True == True would output True.

Check if C# preserves the order of operations in math
