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

* `+`
This quantifier is used to match one or more charecters in the algorithm and placed to the left of the (+) and need to match at least once with any charecter.

* `*`
This quantifier lets the search know that it has to match 0 times or more.

* `?`
This quantifier does the same as (*) and is optional but when impemented it makes the quantifier lazy making it match as few times as possible unlike the default which does the opposite making it considered greedy (matching as much as possible).

(Lazy and Greedy will be explained in its own section below).

* `{7,9}`
This algorithm is set to have the charecters seven to nine charecters long.

* `abc/cba`
This is a match between abc and cba only.

### Grouping Constructs
* `(abc){3}`
We use this when we want to have a group od selective patternes and use parentheses and also include numeric counters alongside it

an example is "abcabcabc", the first group is "abc" and if we use {3} is will repeat it 3 time leading to "abcabcabc"

### Bracket Expressions
Bracket Expressions is a regular expression that is surrounded by square brackets and is used to match a single character or collating element and is then complemented

and example is [a-z]

### Character Classes
Charecter classes are used to match charecters specifically between a range of what is given 

* `\w`
This is used to match with any word charecter that is lowercase without accent marks, for example [y-r5-9_].

* `\W`
This matches any charecter that isn't a word charecter for example [Y-Ry-r5-9_]

* `\d`
This matches any digitized charecters like 5-9

* `\D`
This searches for non-digitized Charecters

* `\p`
This matches a charecter with a specific unicode 

* `[A-Z]`
This creates a range for the search criteria between two charecters

* `'`
This symbol accepts any input

### The OR Operator
* `|`
This operator acts to be a boolean OR and makes a match of expressions before or after the | and is utilized in a group or a whole expression, this causes the search string to look for a match for what follows and precedes the |.

### Flags
Flags are used tp change the interpretation of the expression and are also used after the slosing forward slash

* `i`
This ignores the case

* `g`
"g" is a modifier that preforms a match the finds all matches instead of stopping after the first inital search for case sensitive matches ("g" and "i" are combined in the modifier).

* `m`
This is the multiline flag that is used to enable to match the start and a end a line instead of the whole string 

* `s`
"s" is a global search for the whitespace in a sting 

### Greedy and Lazy Match

* `Greedy`
greedy is a quantifier the uses the search algorithm to match as many patterns as possible and is also the longest sting match

* `Lazy`
Lazy is also a quantifier and is the shortest match that matches the fewest patterns possible

### Boundaries

Boundaries are used to match a position at the "word boundary" and are sperated into 3 positions

* Before the inital charecter in the string 
* After the last charecter in the sting
* Between two charecter in the string 

### Back-references
Back-Refrences are matches with the same text matched by a capturing group and can be used like this (<([A-Z][A-Z0-9]*)\b[^>]*>.*?</\1>).

The Back-Refrence \1 is the first capturing group and the same text is matched by the first group
### Look-ahead and Look-behind

The LA-LB or "lookaround" are zero-length assertionn they match charecters and give up matches to only send the result whether or not if they match, they basically say if they can match or not

## Author

This is the first tutorial i have made for my GitHub, more work can be found here
* `https://github.com/JacobG2510`
