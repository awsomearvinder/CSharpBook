# Data Types & Variables

In C#, every expression evaluates to a value with a data type. These data types are *extremely* important to understand and work with, and will be brought up regularly so it's highly reccomended to understand these well before going on. Any numerical value that is a whole number is a data type called ``int``, every number with a decimal value is a type called ``float``, every True/False is a type known as ``bool``, and every set of arbitrary characters is a ``string``.  We've worked with the types int and bool already. Each data type can have different operations that can be done on them - ints can have math be done on them, and bools can be combined with logical operators that evaluates to another bool (True/False). Floats are pretty intuitive so I want talk too much about them here (for the most part they're similar to ints in what they can do), but strings are different, they represent other kinds of data, data that you can't intuitively do math or logic on. 

As stated earlier strings are a series of characters. A good example of a string would be this page of this book, it may have numerical data in it, but ultimately it's just a series of characters. Strings can be identified in code if they're surrounded by double quotes ("). If you go back to the ``System.Console.WriteLine()`` stuff you were doing in the last section, you can print out words and letters by replacing the inside of the parenthesis like so: ``System.Console.WriteLine("Hello World");`` (again, note the double quotes, this is because the data we're giving ``WriteLine`` is a string, and we seperate strings from normal code with quotes).

Using this you can print whatever you want, numbers, letters, or even emojis. The only mathematical operators that apply to strings are ``==`` as well as the ``+``. The equality check work's as normal - comparing if two strings have the same characters - and the Add operation intuitively combines two strings. For example, ``System.Console.WriteLine("Hi " +  "John");`` would print "Hi John" on screen. 

A Table for reference with all the major data types you'll encounter day to day:
| Type | What it stores|
|------|---------------|
| int | whole numbers |
| float | Decimal numbers |
| bool | True or False |
| string | string of characters |

Note: there is also a char type, which is a single character, as well as variants of these types with slightly different characteristics (double, long, short, etc.), however these 4 are the one's we'll be using for now. 

Types are important because they're required to understand what operations you can do to given data. This data is normally stored in something called a variable. A variable is like a container which can have it's contents modified through the duration of the program, which makes them extremely valuable when you need to use the same piece of data, or change a piece of data throughout the program's lifetime. For example, you could do a program like this:

```CSharp 
static void Main(string[] args){
    int a = 3; //when making a new variable, you have to declare it's "type" first.
    System.Console.WriteLine(a); //This will print 3
    a = 5;
    System.Console.WriteLine(a); //This will print 5
    a = a + 2; //a is now 7 (5 + 2)
    System.Console.ReadLine(); //The screen closes immediately if this isn't here.
} 
```
Exercises:

1. Try making a variable with the type int that stores 3/2, does the program error? If it dosen't, what's the value of 3/2 since ints can only hold whole types? 
2. Make two int variables that hold a 15 and a 4 respectively. print the result of (variable1 % variable2). What value is printed, and is it the value you were expecting?
3. Make a variable called name that stores your name. Print ("Hi " + name) on screen.
4. If you print a string with "\n" in it, the character does something special. Can you figure out what "\n" does? 

As a side note, in the example above we do ``a = a + 2``, which seems kind of counterintuitive (we take a, add 2, then store it in a again?), another shorthand for this which may seem easier in the future is ``+=``, which adds to itself.
``a = a + 2`` could be rewritten as ``a += 2;``. This also applies for other operations, such as ``a-=2;`` or ``a*=2;``. 
