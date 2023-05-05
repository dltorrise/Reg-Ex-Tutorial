# RegExr Tutorial 

RegExr stands for Regular Expressions. A regular expression is a pattern of charaters. 

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

* Matching a Hex Value: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

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

The {6} and {3} quantifiers are used with the OR operator to signify that either there will be 6 or 3 alphanumeric characters. A quantifier will match n amount of tokens before it. 

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

A pipe (|) functions as a logical OR which means the string with either contain one sets of constraints or another. This is used with the quantifiers {3} and {6} to signify that the hex code will either 3 or 6 alphanumeric characters. The two different constraints will be contained within a capturing group (parenthesis). 

### Flags

### Character Escapes

## Author

Danielle Torrise a student of Northwestern's Full Stack Web Development Bootcamp. She loves to watch scary movies, play with her dogs, and take long walks on the beach. 🏖️

View her [github profile](https://github.com/dltorrise).
