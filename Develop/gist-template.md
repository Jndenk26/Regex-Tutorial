# Matching an Email

This tutorial will explain the following Regex: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.

## Summary

Regex is short for regular expression, which is defined as a sequence of characters that defines a search pattern.  This can be used to locate patterns within a string.  This tutorial will explain the components of matching an email through regex.  

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

The anchors used in the above mentioned Regex include ^ and $.  ^ indicated the beginning of the string, whereas the $ denotes the end of the string. 

### Quantifiers

In this regex the + operator is the first quantifier used.  This will connect the email username to the email platform, e.g gmail.  The second + operator will add the ".com"  The second qualifier used is the {2,6}.  This will allow a match range of between 2-6 characters for the character set [a-z/.]. 

### Character Classes

d/ is the character class for this Regex, and only allows single digit matches.  

### Grouping and Capturing

Capturing Group # 1 is ([a-z0-9_\.-]+).  This matches the email user name.  Capturing Group # 2 is ([\da-z\.-]+).  This matches the email platform.  Capturing Group # 3 ([a-z\.]{2,6}) captures the ".com".

### Bracket Expressions

Bracket Expressions # 1 includes [a-z0-9_\.-] which matches any case-sensitive letter from a-z, any character 0-9, and the following characters: "_", "-", and ".".  Bracket Expression # 2 includes [\da-z\.-] and matches a single digit from 0-9, any case sensitive letter a-z and the following characters: "-" and ".".  Bracket Expression # 3 includes [a-z\.] and matches any case sensitive character a-z, and ".". 

### Greedy and Lazy Match

This Regex includes the following greedy match: + quantifier.  This is greedy because there is no limit to the number of matches possible.  The other greedy quantifier in this Regex is {}, because it will allow unlimited matching of ranges between 2-6 characters.

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
