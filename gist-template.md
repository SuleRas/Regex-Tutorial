## Email Regex-Tutorial.

In this tutorial we'll be explaining what is an email regular expression, what each components do and how to break it down to understand the syntax.

## Summary

A regex or "regular expression" is a pattern of characters used to validate, extract, find, search and replace text or a match a position within a body of text.
Regex's are used across most computer programming languages and in Javascript a regex is an object.

Now that we know it's definition we'll be working on this email regex: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)

## Regex Components :

### Anchors

To perform our email validation we'll use the "^" (caret sign) which opens the regex expressions and must be in the beginning of the string and we'll use "$"(dollar sign) to close the regex expression and must be in the end of the string.

### Quantifiers

Quantifiers in regular expression refers to the number of characters or expressions to match.
In this case we've got two quantifiers for our email regex: "+" and "{2,6}".

-The + quantifier helps with connecting the email name + email service provider + .com. (testabc + @gmail + .com) easier way to read it.
-{2,6} How many of a character we're allowed to have in the curly brackets, lower limit of 2 and upper limit of 6.

Extra tips:
-{2,} This indicates a required lower limit character of 2 and no upper limit. (N/A)
-{,6} Upper limit of 6 no lower limit. (N/A)
-{2} This indicates that only number 2 characters are accpetable.

### Grouping Constructs

Parenthesis() begins and ends a Group Constructs, like in a mathematical operation you'd have to treat everything in the parenthesis, meaning that every parenthesis
has to be treated as a unit of is own.
Three groups are available, a list before the @, a list before the . and a last list before $.
(group1)@(group2).(group3) easier way to read it.

### Bracket Expressions

We've got three Bracket Expressions and can use them to create a set of character for matching each section.
[a-z0-9_.-], [\da-z.-], and [a-z.].
Each bracket refers to a part of the email, for example the first bracket refers to any lowercase character from a-z and number from 0-9 or a period.

### Character Classes

Character Classes is used to distinguish different types of characters. For example, distinguishing between letters and digits in our case is the backlash d (\d).

# Author

In the process of being a software developer. (If you'd like to learn more about regex check these two websites: https://ihateregex.io/ and https://regexr.com/)
Suleiman Mohamud: https://github.com/SuleRas
Link:
