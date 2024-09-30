
# Regex Tutorial: Matching Hexadecimal Colour Codes

Hexadecimal colour codes are widely used in web development to represent colours. This tutorial will explain a regex pattern used to validate hexadecimal colour codes, breaking down each component and describing how it works.

## Summary

In this tutorial, we'll break down the following regex pattern:

```
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
```

This regex is used to match both 3-digit and 6-digit hexadecimal colour codes. We'll walk through each component of the regex and explain how it validates colour codes commonly seen in HTML and CSS.

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

- `^`: The caret (`^`) asserts the position at the start of the string.
- `$`: The dollar sign (`$`) asserts the position at the end of the string. This ensures that the regex matches the full string, from start to finish.

### Quantifiers

- `{6}`: Matches exactly six occurrences of the preceding character set (i.e., `[a-f0-9]`).
- `{3}`: Matches exactly three occurrences of the preceding character set.

### OR Operator

- `|`: The pipe (`|`) is used as an OR operator, meaning the regex will match either the 6-digit format or the 3-digit shorthand for hexadecimal colour codes.

### Character Classes

- `[a-f0-9]`: This matches any character in the range `a-f` or `0-9`, which corresponds to valid hexadecimal digits.

### Flags

There are no flags used in this regex, but flags like `i` for case-insensitivity could be applied if needed.

### Grouping and Capturing

- `([a-f0-9]{6}|[a-f0-9]{3})`: Parentheses group multiple parts of the regex together. This section captures either six or three hexadecimal characters for colour codes.

### Bracket Expressions

- Bracket expressions like `[a-f0-9]` allow for matching any single character within the specified range.

### Greedy and Lazy Match

This regex does not use greedy or lazy quantifiers (`?`, `+?`, `*?`), but the `?` in `#?` makes the `#` optional, meaning it will match with or without the `#` symbol.

### Boundaries

Boundaries in this regex are set by the `^` and `$` anchors, which ensure that the regex matches only the entire string.

### Back-references

This regex does not use back-references.

### Look-ahead and Look-behind

There are no look-ahead or look-behind assertions in this regex.

## Author

This tutorial was written by [Cameron Beattie](https://github.com/Cbeattie97)

[Visit Cameron's GitHub profile](https://github.com/Cbeattie97)
