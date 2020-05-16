# Expressions continued

Assuming you've made it this far and have solved the exercies, here are the answers:

1. these are the greater then or equal to (and conversely, less then or equal to) operators. They are similar to > and < except they include inequality. 
2. False. (5 > 4) evaluates to true, and (4 > 5) evaluates to false. True is not equal to False. 
3. C# does preserve order of operations.

We touched on it lightly in the last page, but there's a special set of operations that output True and False. There's also a special set of operations that *only* work on True or False. In table layout similar to last time:

| Operator | Meaning |
|----------|---------|
| <        | Less than |
| >        | Greater than |
| <= | Less than or equal too |
| >= | Greater than or equal too |
| == | Equal too |
| != | Not Equal too |
| ! | Not |
| \|\| | or |
| && | and |

The Not, Or, and And operators (!, \|\|, &&) only apply to values of True or False.

Not inverts it (!True is False, and !False is True), Or outputs True if one of the sides is true, (True || False is True), and and outputs true if both sides are true (True && True is True, every other combination is false). 

Exercises:
1. what is !True == False?
2. What is !True != !False?
3. What is 5>3? Is this the same as 5>3 == True?
4. What is the output of !(5>=5)?

