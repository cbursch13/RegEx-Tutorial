# RegEx Tutorial

Regular expressions, often abbreviated as regex, are essential tools for string manipulation in programming. They allow developers to search for specific patterns within text, making tasks like data validation, text parsing, and pattern matching much more manageable.

## Summary

In this tutorial, we'll be focusing on a particular regex pattern: ^https?://(www\.)?example\.com$

This regex is designed to match URLs that begin with "http://" or "https://", followed by an optional "www." subdomain, and ending with "example.com". Throughout our exploration, we'll dissect this regex piece by piece, explaining each component in detail.

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
Anchors, represented by the symbols ^ and $ in our regex pattern, specify the position within the string where a match must occur. The ^ symbol asserts the start of the string, ensuring that our URL starts with "http://" or "https://". Similarly, the $ symbol asserts the end of the string, guaranteeing that our URL ends with "example.com".

### Quantifiers
Quantifiers determine the number of occurrences of the preceding element in the regex pattern. In our regex ^https?://(www.)?example.com$, the ? quantifier means "zero or one occurrence", applied to the character 's', allowing for both "http://" and "https://".

### Grouping Constructs
Grouping constructs, denoted by parentheses (), allow us to group multiple tokens together. In our regex ^https?://(www.)?example.com$, the group (www.)? captures the optional "www." subdomain, providing flexibility in matching URLs with or without this prefix.

### Bracket Expressions
Bracket expressions, enclosed within square brackets [], specify a set of characters to match. Although not utilized in our regex pattern, they are commonly employed for matching specific characters or character ranges.

### Character Classes
Character classes, denoted by square brackets [], enable matching any one of a set of characters. While absent in our regex ^https?://(www.)?example.com$, they are frequently used for matching ranges of characters such as digits or alphabets

### The OR Operator
The OR operator | allows us to match either of two alternatives. Although not explicitly used in our regex pattern, the optional "www." subdomain serves a similar purpose, providing flexibility in matching URLs with or without this prefix.

### Flags
Flags are options that affect how the regex engine processes the pattern. Common flags include case-insensitive matching, global matching, and multiline matching. In this regex, there are no flags used.

### Character Escapes
Character escapes allow you to match characters with special meaning in regex. In the regex ^https?://(www\.)?example\.com$, \. is a character escape used to match a literal period, since . in regex typically matches any character.

## Author
This tutorial was crafted by Cameron Bursch, a passionate junior developer dedicated to simplifying complex concepts for aspiring learners. For more insightful tutorials and exciting projects, be sure to explore my GitHub profile at [cbursch13](https://github.com/cbursch13).
