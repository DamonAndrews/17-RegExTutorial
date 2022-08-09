# RegEx Read Me

This is a Read Me describing the componenets of matching an Email address.

## Summary

See the below Table of Contents in order to access descriptions for each component of the Regex: Matching an Email. One may find this tool very useful for applications like Node or MongoDB as it provides validation to ensure that emails are inputted with correct formatting.

Matching an Email: `/^([a-z0-9_\.-]+) @ ([\da-z\.-]+)\. ([a-z\.]{2,6})$/`

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

Computers & programs don't do what we want them to do, they do what we tell them to do.  In the case of regular expressions, we want to be able to validate that information is inputted in a correct and accurate fashion. The first step is to indicate where in fact the string we are validating begins and ends. While there are multi-line options, an email address will simply be one line. The (^) (without parenthesis) character indicates the beginning of a string, and for single line validation a (`$)`will indicate where the string should end. Hence the term anchors; these symbols anchor a beginning and end point.

### Quantifiers

Quantifiers further help us validate the data by representing the amount of times characters (or character classes or groups) should be present in the given string. The quantifier present in the match and email string is (+).  This is one of the many quantifiers available, and it means to match one or more times for the elements listed before it. For matching an email this would mean that `([a-z0-9_\.-]` are elements that must be matched, and they can be matched one or more times. By default quantifiers are greedy, which will be explained in the greedy and lazy match section.

### OR Operator

The logical or OR operator allows validation for two types of characters. For example, a lowercase or uppercase version of a letter. The letter "C" for example could be validated for either lower or uppercase using the or character ( | ) as follows, c|C.

### Character Classes

This can be thought of as a way to grop characters without requiring a specific order to the characters. In matching an email with the above string, we see ( [ and ] ) to indicate character classes. We also see the use of (  \d ) to indicate a "digit" character class. It means any digit 0-9, so it is essentially the equivalent of the 0-9 used in the first section of the validator.

### Flags

Flags are anohter key componenets of regular expressions. Often we may want to replace data in a string in addition to validating it. A flag is a way to do that, as they are used to search and replace text. There are 6 total flags available in JavaScript. These range from specifying case sensitivity to positioning within text.

### Grouping and Capturing

Grouping allows us create blocks of patterns. For example in our validation, the folowing grouping is applied to the username portion of the email: `([a-z0-9_\.-]+)`. The parentheses on each end indicate that this is a group, as it is all a single portion of the email address, the username. A capturing group is used for each section of the email validation, one for the username, one for the domain name, and finally one for the top-level domain at the end of the string.

### Bracket Expressions

Using the example from above for username validation we can examine the bracket expressions used. The expression is: `[a-z0-9_\.-]` Inside these brackets the characters are specified that are acceptable for our vaildation. In this example, we can accept alphabetical characters a-z (in lowercase), digits 0-9,a nd the following characters: _ . \ -  , all of which are listed explicitly inside the brackets.

### Greedy and Lazy Match

As mentioned previously in the quantifiers section, quantifiers can be either greedy or lazy, but are lazy by default.

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

Damon Andrews is an at-your-service Web Developer seeking a full time role to put his skill and creativity to good use. You can find more of his work here: https://github.com/DamonAndrews.


Thank you.
