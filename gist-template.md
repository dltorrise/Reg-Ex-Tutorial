# RegExr Tutorial 

RegExr stands for Regular Expressions. A regular expression is a pattern of charaters used to define a search pattern. This will find a specific type of characters. RegEx is universal among coding languages. 

## Summary

In this tutorial, I will be describing how to match a hex value with a regular expression. A hex value is a color that is expressed in a hexadecimal value. This comes in the form of number sign (#) and either 3 or 6 digits between 0 and 9 or letters between a and f. 
 
Here is an example of a regular expression that would match a hex value
 `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)

## Regex Components

### Anchors

The ^ anchor is used to signify the string begins with '#'. This is customary in hex codes. $ is also used to say that the expression has to match the end of the line. 

In the beginning of the expression, you can see `^#` and also a `$` at the end means the expression has to end at the end of the line, unless a multi-line flag in enabled. Flags will not be covered in this tutorial. 

### Quantifiers

The {6} and {3} quantifiers are used with the OR operator to signify that either there will be 6 or 3 alphanumeric characters. A quantifier will match n amount of tokens before it. In addition ? matches the pattern zero or one time.

For example, the `[a-f0-9]{3}` checks if there is letters a-f or digits 0-9 three times in a row. 

### Grouping Constructs

A grouping construct is used to determine if different sections of a string fulfil different requirements. The primary way to group a section of regex is with parenthesis. One type of grouping construct is a capturing group. In this example, the capturing group contains an or operator. 

You can see one grouping construct in the expression: `([a-f0-9]{6}|[a-f0-9]{3})`

### Bracket Expressions

Anything inside a set of brackets represents a character range that we want to match. They outline characters we want to include. We mentioned a bracket expression earlier when we discussed quantifiers: `[a-f0-9]`. This searches for letters a-f and numbers 0-9.

### Character Classes

A character is how reg ex decides what to match. Bracket expressions are a type of character class that groups where you can create your own character class. There are no built-in character classes in this specific expression but the bracket expression `[a-f0-9]` in the OR operator qualifies. 

### The OR Operator

A pipe (|) functions as a logical OR which means the string with either contain one sets of constraints or another. This is used with the quantifiers {3} and {6} to signify that the hex code will either 3 or 6 alphanumeric characters. The two different constraints will be contained within a capturing group (parenthesis). 

The OR expression in this code is: `([a-f0-9]{6}|[a-f0-9]{3})`

## Author

Danielle Torrise a student of Northwestern's Full Stack Web Development Bootcamp. She loves to watch scary movies, play with her dogs, and take long walks on the beach. 🏖️

View her [github profile](https://github.com/dltorrise) here.
