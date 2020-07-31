# Data Types & Variables

In C#, every expression evaluates to a value with a data type. These data types are *extremely* important to understand and work with, and will be brought up regularly so it's highly reccomended to understand these well before going on. Any numerical value that is a whole number is a data type called ``int``, every number with a decimal value is a type called ``float``, every True/False is a type known as ``bool``, and every set of characters is a ``string``.  We've worked with the type's int and bool already, int can have math be done on them, and bool's are a binary true or false at any given time. Float's are pretty intuitive so I want talk too much about them here, but string's are different, they represent other kind's of data, data that you can't intuitively do math on. 

A series of characters are called strings, including everything in this blog post. String's are written in double quotes to help seperate them from other code. If you go back to the ``System.Console.WriteLine()`` stuff you were doing in the last section, you can print out words and letters by replacing the inside of the parenthesis like so: ``System.Console.WriteLine("Hello World");``

Using this you can print whatever you want, numbers, letters, or even emojis. The only mathematical operators that apply to strings are ``==`` as well as the ``+``. The equality check work's as normal, comparing if two string's have the same characters, but the + combines two strings. For example, ``System.Console.WriteLine("Hi " +  "John");`` would print "Hi John" on screen. 

A Table for reference with all the major data types you'll encounter day to day:
| Type | What it stores|
|------|---------------|
| int | whole numbers |
| float | Decimal numbers |
| bool | True or False |
| string | string of characters |

Note: there is also a char type, which is a single character, as well as variants of these types with slightly different characteristics, however these 4 are the one's we'll be using for now. 

Types are important because they're required to understand how to store and work with data. This data is normally stored in something called a variable. A variable can have it's content's modified through the duration of the program, which makes them extremely valuable when you need to use the same piece of data, or change a piece of data throughout the program's lifetime. For example, you could do a program like this:

```CSharp 
static void Main(string[] args){
    int a = 3; //when making a new variable, you have to declare it's "type" first.
    System.Console.WriteLine(a); //This will print 3
    a = 5;
    System.Console.WriteLine(a); //This will print 5
    a = a + 2; //a is now 7
    System.Console.ReadLine(); //The screen closes immediately if this isn't here.
} 
```
Exercises:

1. Try making a variable with the type int that stores 3/2, does the program error? If it dosen't, what's the value of 3/2 since ints can only hold whole types? 
2. Make two int variables that hold a 15 and a 4 respectively. print the result of (variable1 % variable2). What value is printed, and is it the value you were expecting?
3. Make a variable called name that stores your name. Print ("Hi " + name) on screen.
4. If you print a string with "\n" in it, the character does something special. Can you figure out what "\n" does? 
