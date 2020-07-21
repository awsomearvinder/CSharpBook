# Loops (cont.)
You've seen while loops now, however you might remember on the last page that I mentioned another kind of loop. A *for* loop. A for loop is a loop that is specifically designed with the common usecase of making a variable, checking if the variable meets some condition, and what to do to the variable after every itteration. Another, alternatively nicer method of doing the FizzBuzz challence we did on the last page can be done with a for loop as well, like so.

```CSharp
//int i = 0; runs the first time the loop is made.
//i<=100 is the check that runs every itteration. (like the in while)
//i+=1 runs after every itteration.
for(int i = 0; i <=100; i+=1) { //typically, for simple loops like this we just use "i".
    if (i % 3 == 0 && i % 5 == 0) {
        Console.WriteLine("FizzBuzz");
    } else if (i % 5 == 0) {
        Console.WriteLine("Fizz");
    } else if (i % 3 == 0) {
        Console.WriteLine("Buzz");
    }   
}
```


For loops share a lot of similarities to while loops - they just allow you to add more information at once ahead of time into the loop, rather then splitting the information across multiple lines. With a while, we had to add 1 to i (or num) *inside* the loop. We made the variable above it outside, and we checked the condntion inside of the while's condition. 

This loop has the clear advantage of giving all that information at once in one line. A for loop is infact just fancy sugar for a while loop. Behind the scenes the for loop will be transformed to the same while loop when you compile - it's just easier to understand for the programmer, since everything's in one place. 

Exercises

1. Recreate some of the exercises from the last page with for's. Which look better? Alternatively, which look worse?

2. Change some of the lines in the for, try incrementing it by two, increment i by negatve values, play with the condition. Can you use a string instead of a int? What else can you do with this construct?
