# Title (Match an Email - Regex Tutorial)
In this tutorial I will be explaining and informing the reader how read and understand the match an email regex. The purpose of this tutorial is to show the many uses an email regex has to save time and code when it comes to validating emails. 


## Summary
A regular expression can also be expressed as a sequence of specific characters that define a pattern. Depending on the pattern of the sequence will determine the function of the actual regex. Regex itself has a foundation that is interchangeable depending on what the use of the validators are, such as; numbers, letters, various symbols, and many similar characters or spaces that are commonly used. 

This is a matching an email regex example
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
* Anchors are the individual characters that are in the regex. There are two kinds of anchors (^ and $). The ^ refers to the beginning of a string and the $ refers to the end of a string. Such as the email match regex we can see there is a ^ at the front and $ at the end. 
here> /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ < here
* Another example could be:
^Hello world
^Hey I'm talking to you
^Hello neighbor
^Hello how are you matching strings that start with Hello
you$               matching strings that end with you
^Hello world$      matching strings to exact string
or simply put we can look for a string itself such as
hello


### Quantifiers
These are characters in the regex that show how many times a character or entry must be shown in the input to match the regex. 
Examples of Quanitifers are as follows:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
* `+` - matches a string that has beginning followed by one or more of the last character
* `?` - matches a string that has beginning followed by zero or one of the last character
* `{}` -  matches a string that has the beginning followed by how ever many the number in the brackets of the last character in the string
* `()*` - matches a string that has any beginning characters followed by zero or more copies of the string within the brackets
As we see in the email regex we have 2'+' 3'()' and 1'{}'. 
The + shows that the email should be continuous or end from the last characters within the brackets.
The () shows that the email must match to a certain parameter that exists.
The {} show that there should be at least 2 to 6 characters within that entry at the end. 

### OR Operator
OR Operators match on a choice of regex: if you put the character(s) representing the operator between any two characters in the regex, the result matches the combination of the strings that those two characters match.


* `[]` - matches a string that has any characters within the squeare brackets

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
In the email we see that there are 3 cases of brackets. The cases are used to show that each case has the pieces within it but are not capturing those individually and instead as a whole. 

### Character Classes
Character Classes tell the regex to match only one out serveral characters; digits, words, or whitespace

Examples of Character Classes are as follows:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

* `\d` - matches a single character that is a digit
* `.` - matches any character
* the capital case for any aformentioned characters will inverse the match
In the email we see that there is a case to match a single character that is a digit. This refers to a single digit that could be placed in the position of the @ symbol. There are also 4 cases of '.' as well. This matches any other characters that are not specifically defined within the regex. 

### Flags
Flags are optional,we can add it to make it search for things in different ways. Each flag is defined by a single alphabet letter, and has multiple purposes in modifying the expression's search.
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
As we see there are no flags in the email regex.

### Grouping and Capturing
Grouping combines a pattern or string so it is matched in a complete section
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
Examples of Grouping are as follows:
* `()` - parentheses creates a capture group
In the email regex there are three specific capture groups. One for the email, one for the corresponding organization and one for the type of organization. 

### Bracket Expressions
Bracket Expressions `[]` match any single character within the brackets if the first character is in the brackets its a `^` then it is any chracter not in the list, and is unspecified whether it matches or not. 

Examples of Bracket Expressions are as follows: 
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
* `[]` - matching any single character within the brackets
We can see there are three cases of the brackets being used. In this case it is looking for the patterns for characters that start from a to z or 0 to 9. With acception to any other character that is added as well. 

### Greedy and Lazy Match
Greedy and/or Lazy Matching are quantifiers that expand the match as far as possible through the text. 
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
In the email regex there is no matchers. 


### Boundaries
Boundaries are the places between characters.
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
There are no boundaries for the email regex

### Back-references
When using Grouping which is saved in memory for later use. Backreferencing is the name of using these matches. 
Backreferencing is the reference of a captured match by a captured group.
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
There are no back references in the email regex.

### Look-ahead and Look-behind
Is only used when you want to look for a specific character that is followed by or preceded by the regex.
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
There are no look-aheads in the email regex.

## Author
Feel free to checkout my other repositories on my github provided below. 

[GitHub Profile](https://github.com/kaohzina)
