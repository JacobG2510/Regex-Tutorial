# Regex Tutorial

Regex tutorial on how to use the HTML sting and their individual functions when used in coding.

## Summary

The regex is used to identify a pattern in a string search algorithm through a function kown as (find) or (find and replace).

The HTML Tag contains < and > to represent both the opening and closing tag such as or

....etc, Every opening tag has to have a closing tag or it will not run
An example of the code is /^<([a-z]+)([^<]+)(?:>(.)</\1>|\s+/>)$/

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
The components for the Regex are /^<([a-z]+)([^<]+)(?:>(.)</\1>|\s+/>)$/

### Anchors
We use anchors to define the search were the parameters begin and end.

Anything after ^ and before $ (symbols caret and dollar) are part of the search definition and the characters the follow after the caret(^) is identified by the position in the search.

The caret shows the beginning of the string where we have the algorithm to match the character and the dollar identifies the end of the string in the algorithm, this helps the system running the search parameter identify < and > charecters and anything between

(abc123 in the middle is just an example)

### Quantifiers
Quantifiers are used in the regex to find where our token string is matched to a pre-set mumber.

+ This quantifier is used to match one or more charecters in the algorithm and placed to the left of the (+) and need to match at least once with any charecter.

* This quantifier lets the search know that it has to match 0 times or more.

? This quantifier does the same as (*) and is optional but when impemented it makes the quantifier lazy making it match as few times as possible unlike the default which does the opposite making it considered greedy (matching as much as possible).

(Lazy and Greedy will be explained in its own section below).

{7,9} This algorithm is set to have the charecters seven to nine charecters long.

abc/cba This is a match between abc and cba only.

### Grouping Constructs
(abc){3} We use this when we want to have a group od selective patternes and use parentheses and also include numeric counters alongside it
an example is "abcabcabc", the first group is "abc" and if we use {3} is will repeat it 3 time leading to "abcabcabc"

### Bracket Expressions
Bracket Expressions is a regular expression that is surrounded by square brackets and is used to match a single character or collating element and is then complemented

and example is [a-z]

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
