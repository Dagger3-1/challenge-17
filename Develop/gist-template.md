# Title (Challenge-17-Computer Science for JavaScript: Regex Tutorial)

Regular Expressions, commonly known as Regex, are sequences of characters that form search patterns. Regex is a powerful tool for manipulating and analyzing text, and it is widely used in programming, data processing, and text editing. This tutorial aims to provide a comprehensive guide to understanding and using regex, covering various components and their functionalities.

## Summary

In this tutorial, we will explore the fundamental components of regular expressions, including anchors, quantifiers, grouping constructs, bracket expressions, character classes, the OR operator, flags, and character escapes. Each section will provide a detailed explanation of these components and how they can be used to construct complex regex patterns.

Here is a regex pattern we will be breaking down:

 /^(Mr|Ms|Mrs)\.\s[A-Z][a-z]*$/

This regex pattern matches titles such as "Mr.", "Ms.", "Mrs." followed by a space and a capitalized name.

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
Anchors are used to specify the position of a match in relation to the string. The two main anchors are:

^ asserts the position at the start of a string.

$ asserts the position at the end of a string. Example: ^Hello matches "Hello" only at the start of a string.

### Quantifiers
Quantifiers define how many instances of a character, group, or character class must be present in the input for a match to be found. The main quantifiers are:

* matches 0 or more times.

+ matches 1 or more times.

? matches 0 or 1 time.

{n} matches exactly n times.

{n,} matches n or more times.

{n,m} matches between n and m times. Example: \d{2,4} matches between 2 and 4 digits.

### Grouping Constructs

Grouping constructs allow for the organization and retrieval of matched substrings. The main constructs are:

() creates a capturing group.

(?:) creates a non-capturing group. Example: (cat|dog) matches either "cat" or "dog".

### Bracket Expressions

Bracket expressions, or character classes, match any one of the enclosed characters. For example:

[abc] matches "a", "b", or "c".

[a-z] matches any lowercase letter.

[^a-z] matches any character except a lowercase letter. Example: [A-Za-z] matches any uppercase or lowercase letter.

### Character Classes
Character classes provide a way to match specific sets of characters. Common character classes include:

\d matches any digit (equivalent to [0-9]).

\w matches any word character (equivalent to [A-Za-z0-9_]).

\s matches any whitespace character. Example: \d+\s\w+ matches one or more digits followed by whitespace and one or more word characters.

### The OR Operator
The OR operator (|) allows for matching one pattern or another. For example:

(cat|dog) matches either "cat" or "dog". Example: Mr|Ms|Mrs matches "Mr", "Ms", or "Mrs".

### Flags
Flags modify the behavior of the regex pattern. Common flags include:

i for case-insensitive matching.

g for global matching.

m for multiline matching. Example: /hello/i matches "Hello" and "hello".

### Character Escapes
Character escapes are used to match special characters or to specify non-printable characters. Common escapes include:

\. matches a literal dot.

\\ matches a literal backslash.

\n matches a newline character. Example: \d+\.\d{2} matches a number with exactly two decimal places.

## Author
This tutorial was created by Jonathan. Github:https://github.com/Dagger3-1

