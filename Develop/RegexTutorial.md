# Regex Tutorial Matching Email

This tutorial explains the use of the matching an email regex (regular expressions). Which is as follows:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

The matching email regex is used to validate emails.This tutorial will give you a walkthrough of each regex component and how it applies to matching an email.

## Summary

Regex (regular expressions), refer to encoded text strings designed to match patterns in other strings. Regular expressions are helpful when you need to find a string of characters that matches a certain type of pattern. These patterns can be simple, where they match an exact string, or they can be more complex, where they match strings that contain a set of rules.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Author](#author)

## Regex Components

### Anchors
Anchors do not match any character. Instead, they match a position before or after characters. The anchors included in this regex are the `^` and `$`, they are shown at the beginning and end of the line of the code below.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 
               
The `^` symbol signifies that the string of the regex will match with the beginning of the text.

The `$` symbol signifies that the string of the regex will match with the end of the text
 
### Quantifiers
Quantifiers match a number of instances of a character, group, or character class in a string. The quantifiers in this regex component are the `+` and the `{2,6}` in this expression below: 
 
 `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 
        
 Quantifiers indicate the certain amount of characters the regex will match. 
 
 The `+` quantifier will match  1 or more characters. 
 
 The `*` quantifier will match 0 or more characters.
 
 The `?` quantifier will match 0 or 1 character.
 
 The `{n}` quantifier will match `n` character(s).
 
 The `{a,b}` quantifier will match an expression that is at least `a` character(s) but no more than `b` character(s).

### Character Classes
A character class allows you to match any symbol from a certain character set. A character class is also called a character set. Character Classes are the most basic expressions used in regex after a character match. It can match a character from a specific set. To see the use of the character classes on the regex for matching an email, see below: 
 
 `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 
 
- `[a-z0-9_\.-]+` : This is stating that the string has to have at least 1 or more letter from a to z or have one or more digits between 0 and 9, or an underscore_ or dot . using the literal expression. or a hyphen "-".
- `[\da-z\.-]+` : This will match a string that has digits from 0-9 because it is using \d or a letter from a to z because it is using a to z. The search pattern can be repeated because it uses the quantifier + at the end of the character class. 
- `[a-z\.]{2,6}` : This is referring to match a letter from a to z because it is using a-z or a dot. The matching pattern for this section must have 2 or at least 6 occurrences. 

### Grouping and Capturing
Capturing groups are a way to treat multiple characters as a single unit. They are created by placing the characters to be grouped inside a set of parentheses. Paranthesis are used for grouping in the regex below. 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 

In this particular regex, grouping is used to separate meta characters from its literal characters. The following groups from our regex are below.

- `([a-z0-9_\.-]+)`
- `([\da-z\.-]+)`
- `([a-z\.]{2,6})`

### Bracket Expressions
Lastly, our regex contains a bracket expressions from the regex below. These are expressions enclosed in the square brackets.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 

There are three within our code:
- `[a-z0-9_\.-]`
- `[\da-z\.-]`
- `[a-z\.]`

So, for example, in `[a-z0-9_\.-]`, this character will be matched by any lowercase letters from a-z, any digits from 0-9, or a period.

## Author
Skyler Crawford <br>
Github Profile: https://github.com/Ricochet227