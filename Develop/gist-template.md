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
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

The ^ anchor is used to signify the string begins with '#'. This is customary in hex codes.

### Quantifiers

The {6} and {3} quantifiers are used with the OR operator to signify that either there will be 6 or 3 alphanumeric characters. A quantifier will match n amount of tokens before it. In addition ? matches the pattern zero or one time.

### Grouping Constructs

A grouping construct is used to determine if different sections of a string fulfil different requirements. The primary way to group a section of regex is with parenthesis. One type of grouping construct is a capturing group. In this example, the capturing group contains an or operator. 

### Bracket Expressions

Anything inside a set of brackets represents a character range that we want to match. They outline characters we want to include. 

### Character Classes

???

### The OR Operator

A pipe (|) functions as a logical OR which means the string with either contain one sets of constraints or another. This is used with the quantifiers {3} and {6} to signify that the hex code will either 3 or 6 alphanumeric characters. The two different constraints will be contained within a capturing group (parenthesis). 

## Author

Danielle Torrise a student of Northwestern's Full Stack Web Development Bootcamp. She loves to watch scary movies, play with her dogs, and take long walks on the beach. 🏖️

View her [github profile](https://github.com/dltorrise).
