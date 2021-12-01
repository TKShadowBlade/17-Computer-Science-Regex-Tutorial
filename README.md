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

The anchors of a regex specify where it begins and where it ends. This is done using the ^ character at the start of the expression, and the $ character at the end of it. You will also 

### Quantifiers

Quantifiers are characters that you can use to identify groups of metacharacters:

- the asterisk * searches for a match of 0 or more characters
- the plus sign + searches for a match of 1 or more characters
- the question mark ? searchese for a match between 0 and 1 character
- using curly brackets {} lets you search for a match within a certain range of characters. You can write this either as {min, max} or as {n}, with n specifying a number range.

### Grouping Constructs

You can use parentheses () as a way to group subexpressions together. Doing so will allow you to search for a set of characters in a group.

- Example: (po)* will search for zero or more instances of the character group "po".

### Bracket Expressions

Brackets identify an exact character or set of characters to match when searching. Any individual character inside brackets will be matched, as well as any set of characters. These are referred to as "character classes".

- Example:

```

[abcd]

```

- This expression will match the letters "a" and "c" in the word "catch".

If you include the ^ character inside of your brackets at the start, this will specify characters NOT to be matched. This is also known as a negated character class.

- Example:

```

[^abcd]

```

- This will match any character that is NOT a, b, c, or d.

You can also specify character sets/ranges using a hyphen ("abcd" is the same as "a-d").

### The OR Operator

The OR Operator is another name for the " | " character. you can use this in search groups such as what was discussed above, if you wish to alternate between characters in a search group.

- Example: "(s|t)he" will search for groupings that contain "s" OR "t", followed by "h", followed by "e". 

### Flags

Flags are additional modifiers that affect the search. There are six of these flags that are used in Javascript, such as:

- 'g' is used to return ALL instances of a search parameter
- 'i' is used to specify that a search parameter is case insensitive
- 'm' is used for multiline searches, and it affects how the '^' and '$' anchors function.

### Character Escapes

The backslash '\' is used to do what is called "escaping characters". This is for when you want to search for a literal character, not use it as a search modifier.

- Example: The dot '.' is typically used to specify a search for any character. However, you can search for a literal dot if you write it as such:
```
/\./
```


## Author

I am an up-and-coming web developer with a taste for learning and improving my skillset. I am a perpetual work in progress, and am always looking for new ways to grow my knowledge base. If you want to get a better look at what projects I'm working on, you can visit my Github profile at the link below:

- [Anthony K. Github Profile] (https://github.com/TKShadowBlade)
