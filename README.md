# Regex for Dummies (Like  me!)

This tutorial has been created for people that have zero to no knowledge of anything regex (Regular Expression) related.

## Summary

Regex is a way of communicating with the computer what to expect in terms of input, what to look for, or even what to pick out fronm a given string.
This tutorial will explain what anchors, quantifiers, classes and constructs are and how to use the OR operator, Flags, and Escapes. By the end of this you should be able to understand the following regex:
* ^[a-zA-Z0-9.!#$%&’*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]+)*$
* ^[A-Za-z][A-Za-z\'\-]+([\ A-Za-z][A-Za-z\'\-]+)*$

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
Regex has many companents that are use for different things, such as telling the computer where to start the line and even where to add the space or go to the next line.
Some of these are anchors, quantifiers, classes, etc.

### Anchors
Anchors are used to let the computer knows that when it reads '^' it meants the starting point and when it reads '$' ir means it's the end point.
'^' = start of a line
'$' = end of a line
'\A' = start of a string but not a line
'\Z' = end of a string but not a line

### Character Classes
While using regex, you will need to specify which characters is the computer matching, to do that you would use '\d' for any digits between (0-9) and '\w' for any alphanumeric character (a-zA-Z0-9). Here are the following character classes:
'\d' = digits
'\D' = non-digit
'\s' = space
'\S' = non-space
'\w' = word character
'\W' = non-word character
'\b' = word boundary
'\B' = non-word boundary
'\h' = horizontal space
'\H' = non-horizontal space
'\v' = vertical space
'\V' = non-vertical space

(Heads up! you might not use the capital letter classes that much(?))

### Quantifiers
Quantifiers are used to tell the computer how many to match for if any at all, for example '*' is used for zero or more characters, while '+' is used for one or more characters.
You will always have to specify which characters are there going to be before using the quantifiers.
'*' = zero or more
'+' = one or more
'?' = zero or one
'{n}' = exactly n times
'{n,},' = n or more times
'{n,m}' = between n and m times

### Grouping Constructs
Grouping constructs is how you're going ot separate the characters for the computer by using '()', you can even name the subexpression inside the '()'.
'(subexpression)' = regular group
'(?'name'subexpression) = named group

### Bracket Expressions
The bracket expressions are the ones that will indicate the computer what to match, inside the '[]' you will find all the specifications that you want the computer to know. 
In addition, the '{}' are used to specify the quantity, like we used them with quantifiers!
'[]' = set of characters specified
'{}' = to specify quantities

### The OR Operator
The or operator is used for when you know which word to expect, this operator is '|'. It will match either the characters given before or after, giving priority to the first set.
'|' = OR

### Flags
Flags are used to give regex a headsup code, like telling it to ignore the casing wiht 'i' or make the computer look globaly with 'g':
'i' = Ignore Casing Makes the expression search case-insensitively.
'g' = Global Makes the expression search for all occurrences.
's' = Got All Makes the wild character . match newlines as well.
'm' = Multiline	Makes the boundary characters ^ and $ match the beginning and ending of every single line instead of the beginning and ending of the whole string.
'y' = Sticky Makes the expression start its searching from the index indicated in its lastIndex property.
'u' = Unicode Makes the expression assume individual characters as code points, not code units, and thus match 32-bit characters as well.

### Character Escapes
When wanting the computer to ignore the meaning behind 'i' for example we would write '\i', that means it is being scaped and the meaning behind it it's being ignored, instead of ignoring the casing in a character and it will take it for simply what it is an 'i'. Since the '\' also has meaning to actually use a '\' symbol you will have to use '\\'.
'\' = character escaping

## Author

Sabrina Centeno is the author of this tutorial for dummies, like herself. Please take all the information with a grain of salt :)
Github: https://github.com/Sabplpz
Thanks you!
