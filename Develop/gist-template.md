# Regex Pseudo

My this week is to create a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does.

## Summary

This regex is a homemade version of an email validation tool. While I understand that regex may not be the most ideal way, and certainly not the only, it was something that I enjoyed working on. This could be used in a number of scenarios, but the most applicable for me is through the use of inquier prompts. 

In our cirriculum, there has been a few assignments that have required us to gather input from an end user through inquier prompts. Without understanding what regex was, or how to use it, I now find that this would be very usefull in validating the user input. I

Let us take a look a the regex expression we will be evaluating below:

```js
/^\S[^\n\r][a-zA-Z0-9\.]+@+\S[^\n\r][a-zA-Z]+[.]+[a-z]+/;
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)

## Regex Components

### Anchors

```js
^
```

The only anchor used in this Regex is the carrot symbol.

### Quantifiers

```js
+
```

The only quantifier used in this Regex is the plus symbol...

### OR Operator

No OR operator was used in the creation of this Regex...

### Character Classes

```js
[^\n\r]
[a-zA-Z0-9\.]
[^\n\r]
[a-zA-Z]
[.]
[a-z]
```

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
