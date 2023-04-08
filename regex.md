# Regex Matching an Email

## Summary

This tutorial will go over a regex that is used to match an email. In this tutorial we will break down the regex and explain each character and concept of it to give a detailed explanation on the components and how they work.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

### Anchors

The anchors of a regex are the first and last elements of the expression without including the `/` since a regex is a literaly and the `/` character helps us determine that it is a regex. This means that the anchors `^` and `$` are both considered to be the anchors of the regex.

### Quantifiers

Quantifiers in a regex will set the limits of the string that your regex matches. This is stated by either a `*` `+` `?` or a set of curly brackets with numbers in them. `*` means matching the pattern zero or more times, `+` means one of more times, `?` means zero or one time. `{n}` means matches n number of times, `{n, }` means matches at least n times, and `{n, x}` means matches from n to x number of times.

### Character Classes

Character classes in a regex defines what characters can occur in the input string that can fulfill a match to our regex. In our above regex the character classes are determined with `\d` which matches a single character that is a digit ranging from 0 to 9.

### Grouping and Capturing

The two groups used for this regex expression are: `([a-z0-9_\.-]+)` and `([a-z\.]{2,6})`. The first expression is used to match the user's email name before the @ symbol while the second expression is used to match to the email service being used after the @ symbol (gmail, yahoo, etc).

### Bracket Expressions

Bracket expressions are anything that are inside of the `[]`. These are used to outline what characters we want to include in our regex such as `[a-z]` meaning we include any character from a through z.

### Greedy and Lazy Match

Since this regex include a `+` after the first 2 bracket expressions then it is considered and Greedy match. This means that it will match as many occurrences of the pattern as described. In ours we only use `+` meaning it will check if it matches the pattern one or more times.

## Author

My name is Alexander Weiss, I am a Front-end focused developer currently getting my certification at Penn LPS. Here is my GitHub profile if you have any questions: https://github.com/alexander1262
