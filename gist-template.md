# RegEx Tutorial

Regular expressions, commonly referred to as regex, are versatile tools used to find patterns within strings. They offer a compact and adaptable method for recognizing and altering text. Throughout this tutorial, we'll explore different parts of regex to grasp how they work and how to use them effectively.

## Summary

The regex we'll be focusing on is: ^https?://(www\.)?example\.com$

This regex is a pattern for matching URLs that start with "http://" or "https://", followed by an optional "www." subdomain, and ending with "example.com". Throughout this tutorial, we will dissect this regex and explain each component in detail.

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
Anchors in regex specify the position in the string where the match must occur. The ^ and $ symbols used in the regex ^https?://(www\.)?example\.com$ are anchors. The ^ asserts the start of the string, ensuring that the URL starts with "http://" or "https://". The $ asserts the end of the string, ensuring that the URL ends with "example.com".

### Quantifiers
Quantifiers specify the number of occurrences of the preceding element in the regex pattern. In the regex ^https?://(www\.)?example\.com$, ? is a quantifier meaning "zero or one occurrence". It applies to the character s, allowing "http://" or "https://".

### Grouping Constructs
Grouping constructs, denoted by parentheses (), allow you to group multiple tokens together. In the regex ^https?://(www\.)?example\.com$, (www\.)? is a group that captures the optional "www." subdomain.

### Bracket Expressions
Bracket expressions, denoted by square brackets [], specify a set of characters to match. There are no bracket expressions in this regex, but they're commonly used for matching specific characters or ranges.

### Character Classes
Character classes allow matching any one of a set of characters. They are denoted by square brackets []. In the regex ^https?://(www\.)?example\.com$, there are no character classes, but they're frequently used for matching a range of characters like digits or alphabets.

### The OR Operator
The OR operator | allows you to match either of two alternatives. In the regex ^https?://(www\.)?example\.com$, it's not explicitly used, but the optional "www." subdomain serves a similar purpose.

### Flags
Flags are options that affect how the regex engine processes the pattern. Common flags include case-insensitive matching, global matching, and multiline matching. In this regex, there are no flags used.

### Character Escapes
Character escapes allow you to match characters with special meaning in regex. In the regex ^https?://(www\.)?example\.com$, \. is a character escape used to match a literal period, since . in regex typically matches any character.

## Author
This tutorial is written by Cameron Bursch, a passionate junior developer interested in simplifying complex concepts for those interested in learning about regular expressions. Feel free to check out more tutorials and projects on my GitHub profile. 
https://github.com/cbursch13
