# RegEx Tutorial (Hex Value)

Welcome to my gist breaking down a specific regular expression. Regular Expression, or RegEx for short, are used by combining special characters to create a specific search pattern.
<p>An example of a RegEx used for a username:</p>
<pre><code>/^[a-z0-9_-]{3,16}$/</pre></code>
The RegEx we are going to look at is for matching a Hex Value. Below is a table of contents explaining the many components of the RegEx we are going to be looking at. Without further ado, let's jump right into it!

## Summary

With this particular RegEx, we will be looking at the Anchors, Quantifiers, Grouping Constructs, Brackets Expressions, the OR Operator.

<p>Matching a Hex Value:</p>
<pre><code>/^#?([a-f0-9]{6}|[a-f0-9]{3})$/</pre></code>

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

Anchors are used to signify the beginning and ending of a string you are trying to search for.

<p>Common Anchors:</p>

<pre><code>^ and $</pre></code>

Within our Hex Value example, we can see that the ^ and the $ are placed at both ends of the RegEx to signify the beginning and ending of the string we are trying to search for.

<pre><code>/^#?([a-f0-9]{6}|[a-f0-9]{3})$/</pre></code>

Beginning of the RegEx
<pre><code>/^....</pre></code>

End of the RegEx
<pre><code>....$/</pre></code>

### Quantifiers

Quantifiers are used to set limits on the string we are searching for. Quantifiers can be used on the RegEx as a whole or be placed within subexpressions. Quantifiers are expressed using '{ }' with values inside the brackets. 

This specific quantifier is looking for a string with EXACTLY 6 characters
<pre><code>[a-f0-9]{6}</pre></code>

This specific quantifier is looking for a string with EXACTLY 3 characters
<pre><code>[a-f0-9]{3}</pre></code>

### Bracket Expressions

Bracket expressions are used within the '[]' to narrow down what we want to find in our search. Within the bracket expression, we can have multiple search parameters for our RegEx.

Within a Hex Value, there is a specific range of character that we can have.

<pre><code>[a-f0-9]</pre></code>

This RegEx is looking for letters between 'a-f' and numbers from '0-9'.

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
