# 17-Computer-Science-Regex-Tutorial
Computer Science for JavaScript Regex Tutorial

This gist was created to help explain the purpose and uses of what is known as a "regular expression". Simply put, a regular expression, or "regex", is a series of special characters that make up a specific search pattern. When coding, you can use a regular expression to fine-tune what kind of statement your program is set to look for in a particular instance. This is helpful when setting up a specific criteria for login credentials, or for identifying the format of a webpage URL. These characters can be literal characters (such as a specific letter or number), or they can be "meta-characters" (such as "/d" which refers to any number from 0-9 ).

## Summary

The regex I will be outlying in this gist will be one that you can use to match an email address, such as the following:

```

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

```

I will discuss each section of the search sequence and what the parameters mean. This might look confusing, but each part of the expression specifies a match condition.

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

The anchors of a regex specify where it begins and where it ends. This is done using the ^ character at the start of the expression, and the $ character at the end of it.

### Quantifiers

Quantifiers are characters that you can use to identify groups of metacharacters:

- the asterisk * searches for a match of 0 or more characters
- the plus sign + searches for a match of 1 or more characters
- the question mark ? searchese for a match between 0 and 1 character
- using curly brackets {} lets you search for a match within a certain range of characters. You can write this either as {min, max} or as {n}, with n specifying a number range.

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
