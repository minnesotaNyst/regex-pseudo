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

- / -> we use the forward slash to denote the starte of a regular expression.
- ^ -> We use the carrot symbol to tell the expression that it needs to match the beginning of a string, or the beginning of a line
- \S -> We use the backslash paire with a capital S to indicate that the string cannot begin with whitespace. This includes spaces or tabs.
- [] -> This is a character set which defines what the string should match when there is definition between the brackets.
- [^] -> When the character set (brackets) starts with a ^, it will negate the set (this means that the expression cannot pass validations if it matches whatever is inside of the brackets).
- [^\n\r] -> Using the backslash with n and r means that the string cannot begin with a new line feed for a returned line. This further adds to the expression component that does not allow spaces or tabs.
- [a-zA-Z0-9\.] -> This component tells us that the string can start with a character (upper or lower case) and a number. One will notice that the component ends with a backslash and a period (.); which means that if there is a period in the body of the email address that the expression can ignore it. In other words, periods are allowed.
- +@+ -> The next component we use is an @ symbol paired with the + quantifier. The plus quantifier looks for a match for one or more of the preceeding token (in this case, the @ symbol).
- [^\n\r] -> Here we reuse the component that does not allow spaces or tabs to start the domain portion of the email address.
- [a-zA-Z] -> Next, we reuse part of the initial body component that allows characters (upper or lower case) to fill out the domain of the email address. This can be easily modified if there are email domains that include numbers, but they are rare.
- +[.] -> This component is using the plus quantifier that we saw before to tell the expression that we want a period after the domain portion of the email. Esentially, we are looking for the '.com' and validating that the period comes before...
- +[a-z]+ -> Before the actual component that is going to validate that the address ends with lowercase only. We need to end this with a plus quantifier to tell the expression that it needs to match one or more of the preceding token.
- / -> Lastly, we end the expression with another forward slash. This closes the expression.

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

Today, as a motivated and goal oriented individual I embrace challenges, strive to help others learn and develop, work collaboratively with teams, and push myself to further develop my current skill set with an expectation to succeed. I thrive in high paced environments where teams are setup for success. You can check out the rest of my profile at: https://github.com/minnesotaNyst
