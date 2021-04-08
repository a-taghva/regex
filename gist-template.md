# Regex Tutorial

Matching a Hex Value: 
<pre>/^#?([a-f0-9]{6}|[a-f0-9]{3})$/</pre>


## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.
<pre>/^#?([a-f0-9]{6}|[a-f0-9]{3})$/</pre>

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
<pre>/<span style="color: red">^</span>#?([a-f0-9]{6}|[a-f0-9]{3})<span style="color: red">$</span>/</pre>
`^` and `$` are called "anchors" in regex.<br />
The caret `^` matches at the beginning of the text, and the dollar `$` – at the end.

The pattern `^#` means string starts with `#`<br />
We can see if it ends with a charcter, number or underscore by using `\w$`<br />

<span style="color: red"></span>

### Quantifiers
<pre>/^#?([a-f0-9]<span style="color: red">{6}</span>|[a-f0-9]<span style="color: red">{3}</span>)$/</pre>
`Quantity {n}`

#### The exact count {3}
`\d{3}` is same as `\d\d\d`
it look for 3 digits


#### The range {3,6}
`\d{3,6}` matches 3-6 times.
`\d{3,}` matches 3 or more digits.
<pre>/^#?([a-f0-9]{6}|[a-f0-9]{3})$/</pre>

### OR Operator
<pre>/^#?([a-f0-9]{6}<span style="color: red">|</span>[a-f0-9]{3})$/</pre>
square brackets are similar to OR Operator, for instance gr[ae]y is either gray or grey

`gr(a|e)y` matches <u>gray</u> or <u>grey</u><br />
`gra|ey` means <u>gra</u> or <u>ey</u>

### Character Classes
A character class is a special notation that matches any symbol from a certain set.<br />
for example:<br />
  - `\d`: digits[0-9]<br />
  - `\w`: either a letter of Latin alphabet or a digit or underscore.<br />
  - `\s`: includes tabs `\t`, newlines `\n` and some other rare characters, `\v`, `\f` and `\r`<br />

### Flags

### Grouping and Capturing

### Bracket Expressions


### Greedy and Lazy Match


## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
