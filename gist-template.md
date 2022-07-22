# Title (Regular Expressions (RegEx))

Hello, below i have my Regex tutorial. I talk about key concepts, how it used and for what purposes we developers use regular expressions. Thank you.

## Summary

A regular expression are patterns used to match character combinations in string. The pattern can be used for text search and text replace operations.

How does it work?
Its a sequence of characters that forms a search pattern.
When the data is search it can be used to search patterns to match what you are looking for.
A regular expression can be very simple but also very complicated in the search pattern require to meet all requirements. 

A example we see is when signing up for accounts. If email not valid input will notify that email is not valid. When email is valid there won’t be pop up saying to enter valid email. This is the same for other categories of inputs like phone number and etc.

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
A anchor means a string that begins or ends. The two Character are ^ and $. The ^ anchor means a string a string that begins with that characters after it.
The $ anchor signifies a string that comes that ends with character at the end.

### Quantifiers
Quantifiers specify how many characters must be in expression for a match to be found. They set limits and usually include minimum and maximum characters	
*-Matches the pattern zero or more times
+-Matches the pattern one or more times
?-Matches the pattern zero or one time
{}-Curly brackets can provide three different ways to set limits for a match:
	{ n }-Matches the pattern exactly n number of times
	{ n, }-Matches the pattern at least n numbers of times
	{ n, x }-Matches the pattern from a minimum of n number of times to a maximum of x number of time

### Grouping Constructs
Regular expressions become more complicated so checking that strings to determine different requirements. A method called grouping constructs. To group a section of a regex using these () is known as a subexpression.

### Bracket Expressions
A bracket expressions is a regular expressions enclosed by []. It use to match the character in the list. The breakdown of the expressions [a-z], [0-9], [_-]. The String will be able to have any lower case letter between a-z. If we want to include a Uppercase you have to use a different expression like ‘[A-Z] because it is case sensitive. The string can contain any 
number with the [0-9] expression. The [_-] contains an underscore or hyphen. 
* [a-z]  equals abcd…etc.
* [0-9] equals 01…..789

### Character Classes
Character classes defines set of  characters> it specify the characters that will successfully match a single a character from a 

Ex:[aeiou] equals “a”, “e”, “I”, “o” or “u”.


### The OR Operator
The OR operator can be used to match characters to the left or right of the expression. 
Ex: the (m|M) will match either t or T from the input string. 
Ex: The regex four | 4 acce[ts strings “four” or “4”

### Flags
A regex must be wrapped in slash characterss. When you are  using flags this regex being wrapped in slash becomes and exception. 
There are only 6 of the in Javascript.
i - the search is case-insensitive: no difference between A and a  
g - with the flag the search looks for all matches, without it only the first match is returned.
m - multiline mode  
s - enables "dotall" mode that allows a dot . to matchg newline character \n
u - enables full uncide support. t enables correct processing of surrogate pairs.
y - searching the exact position in the text

### Character Escapes

The backslash in a regular expression precedes a literal character. You also escape certain letters that represent common character classes

Ex: Regex(
	"Are you there, Saul?, asked Laus.”, // source

	"(here|there).+(\w+).+(said|asked)(\s)(\w+)\." ); // regular expression
"there, Saul?, asked Laus.”

## Author

Hello I am Saul Ventura, Full Stack Web Developer from Dallas, Texas. 









