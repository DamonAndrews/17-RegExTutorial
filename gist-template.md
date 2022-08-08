# RegEx Read Me

This is a Read Me describing the componenets of matching an Email address.

## Summary

See the below Table of Contents in order to access descriptions for each component of the Regex: Matching an Email. One may find this tool very useful for applications like Node or MongoDB as it provides validation to ensure that emails are inputted with correct formatting.

Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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

Computers & programs don't do what we want them to do, they do what we tell them to do.  In the case of regular expressions, we want to be able to validate that information is inputted in a correct and accurate fashion. The first step is to indicate where in fact the string begins and ends. While there are multi-line options, an email address will simply be one line. The (^) (without parenthesis) character indicates the beginning of a string, and for single line validation a (`$)`will indicate where the string should end. Hence the term anchors; these symbols anchor a beginning and end point.

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
