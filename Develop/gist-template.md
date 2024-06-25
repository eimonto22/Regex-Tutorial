# Matching an Email Address tutorial

In this tutorial I will be describing a tutorial on email addresses matching with the use of regular expressions.

## Summary

Email matching using regular expressions (regex) involves creating a pattern that can accurately identify email addresses within text.

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
This is the part of the email address before the "@" symbol. It can contain: Uppercase and lowercase letters (a-z, A-Z)Digits (0-9)Special characters such as dot (.), underscore (_), percent (%), plus (+), and hyphen (-). The @symbol is a fixed character in every email address. Following to the domain portion, this is the part of the email address after the "@" symbol. It can contain: Domain labels separated by dots (.) Each domain label can contain letters, digits, and hyphens, but not start or end with a hyphen.

### Anchors
Anchors are special characters in regular expressions that assert the position of a match within a string, rather than matching any actual characters. They are particularly useful in email matching to ensure that the entire string being checked conforms to the email format. Caret (^): Asserts the position at the start of a string.
Dollar Sign ($): Asserts the position at the end of a string.
### Quantifiers
Quantifiers in regular expressions specify how many instances of a character, group, or character class must be present in the input for a match to occur. They are crucial for defining the constraints on different parts of an email address in regex. 
Common Quantifiers:
*: Matches 0 or more occurrences of the preceding element.
+: Matches 1 or more occurrences of the preceding element.
?: Matches 0 or 1 occurrence of the preceding element.
{n}: Matches exactly n occurrences of the preceding element.
{n,}: Matches n or more occurrences of the preceding element.
{n,m}: Matches between n and m occurrences of the preceding element.
### OR Operator
The OR operator in regular expressions is represented by the pipe symbol (|). It allows you to specify multiple alternative patterns that can match. When used in email matching, it can help to accommodate variations in email address formats or to match specific patterns within the broader email format.
### Character Classes
This is an example of simple character classes that can be used for an email and what regex will match against.
[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$ 
### Flags
lags in regular expressions modify the behavior of the regex engine, allowing for more flexible matching. When matching email addresses, flags can be used to control case sensitivity, multi-line mode, and more.
### Grouping and Capturing
Grouping and capturing in regular expressions allow you to extract specific parts of a match. In the context of email matching, groups can help isolate the local part, domain, and top-level domain (TLD) of an email address.
Grouping: Parentheses () are used to group parts of a regex pattern.
Capturing: Groups not only group the pattern but also capture the matched content, which can then be accessed and used.
### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

## Author
My name is Eddie Montoya and I hope I was able to make a bried yet informational tutorial for Regex Email Matching. (https://github.com/eimonto22/Regex-Tutorial)
