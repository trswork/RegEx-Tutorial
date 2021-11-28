## RegEx Tutorial

A regex, which is short for regular expression, is a sequence of characters that defines a specific search pattern. They are also frequently used to validate input.

## Summary

I will be describing the regex for matching an email and how each is used in this particular expression. 
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
Anchors match a position within a string, not a character.

Examples
^ Beginning(anchor). Matches the beginning of the string.
 $ End. Matches the end of the string.

### Quantifiers
Quantifiers are used to indicate that the preceding token must be matched a certain number of times.

Examples
+ Quantifier. Match 1 or more of the preceding token
{2,6} Quantifier. Match between 2 and 6 of the preceding token.

### OR Operator
OR Operator can use the | operator (logical OR) to match characters or expression of either the left or right of the | operator.

Not used in the email example above

### Character Classes
Character classes are used to match a character from a specific set. 

Examples
 a-z Range. Matches a character in the range "a" to "z". Case sensitive
 0-9 Range. Matches a character in the range "0" to "9"
 _ Character. Matches a "_" character
 \. Escaped Character. Matches a "." character
 - Character. Matches a "-" character


### Flags
Flags can change how the expression is interpreted. They also follow the closing forward slash of the expression.

Example
/ Flag. Used to close the expression. /g is used for a global flag

### Grouping and Capturing
Groupings allow you to combine a sequence of tokens to operate on them together. 

Capturing groups are a way to treat multiple characters as a single unit. To create this place the characters to be grouped inside a set of parentheses.  

Example
(Capturing group #1. Groups multiple tokens together and creates a capture group for extracting a substring or using a backreference.
 [character set. Match any character in the set
 a-z Range. Matches a character in the range "a" to "z". Case sensitive
 0-9 Range. Matches a character in the range "0" to "9"
 _ Character. Matches a "_" character
 \. Escaped Character. Matches a "." character
 - Character. Matches a "-" character
])
### Bracket Expressions
A bracket expression is either a matching list expression or a non-matching list expression. Consists of one or more expressions(ordinary characters, collating elements, equivalence classes, or character classes).

Example
[character set. Match any character in the set
 a-z Range. Matches a character in the range "a" to "z". Case sensitive
 0-9 Range. Matches a character in the range "0" to "9"
 _ Character. Matches a "_" character
 \. Escaped Character. Matches a "." character
 - Character. Matches a "-" character
]

### Greedy and Lazy Match
Greedy Match means the regex engine matches as many characters as possible.

Lazy Match means the regex engine matches the shortest possible string. 

Not used in the email example above

### Boundaries
Boundaries refer to a position between \w and \W, or at the beginning or end of a string if it begins or ends with a word character.

Not used in the email example above

### Back-references
Back-References refer to a previously matched group and looks for exactly the same text again.

Not used in the email example above

### Look-ahead and Look-behind
The lookahead asserts that what immediately follows the current position is one or more word characters, and captures these characters to Group 1. 

Lookbehind has the same effect, but works backwards. It tells the regex engine to temporarily step backwards in the string, to check if the text inside the lookbehind can be matched there.

Not used in the email example above

## Author

My name is Tenee Rodriguez. I am currently based in Charlotte NC. I am attending UNCC's Coding Bootcamp with the intent of completing this course in January of 2022. Coding is a new field for me. I've spent the last 6 years in the Insurance field. I have experience with both personal and commercial insurance.

https://github.com/trswork