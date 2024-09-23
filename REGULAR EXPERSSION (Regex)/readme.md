# Regular Expressions (Regex)
Regular expressions, commonly known as regex, are sequences of characters that form search patterns. They are often used for string matching, search, and text processing tasks such as validation and extraction.

Table of Contents
Basic Syntax
Common Regex Patterns
Examples
Finding Patterns
Matching Specific Formats
Usage in Python

## Basic Syntax
`. (Dot)`: Matches any character except a newline.

`^`: Anchors the regex at the start of a string.

`$`: Anchors the regex at the end of a string.

`[] (Character Set)`: Matches any single character within the square brackets.

`|`: Acts as an OR operator between patterns.

`\`: Escapes a special character.

`+`: Matches one or more of the preceding element.

`*`: Matches zero or more of the preceding element.

`?`: Matches zero or one of the preceding element.

`{n}`: Matches exactly n occurrences of the preceding element.

`{n,m}`: Matches between n and m occurrences.

## Common Regex Patterns

`\d`: Matches any digit (0-9).

`\D`: Matches any non-digit character.

`\w`: Matches any word character (alphanumeric + underscore).

`\W`: Matches any non-word character.

`\s`: Matches any whitespace character (spaces, tabs).

`\S`: Matches any non-whitespace character.

### Examples

## Finding Patterns

Match a single digit: \d

Pattern: \d

String: I have 2 apples and 3 bananas

Matches: 2, 3

Match an email address:

Pattern: \w+@\w+\.\w{2,3}

String: Contact me at example@mail.com

Matches: example@mail.com

Match a phone number: (123) 456-7890

Pattern: \(\d{3}\)\s\d{3}-\d{4}

String: My phone number is (123) 456-7890.

Matches: (123) 456-7890

Matching Specific Formats

Match a date in dd/mm/yyyy format:

Pattern: \d{2}/\d{2}/\d{4}

String: Today's date is 23/09/2024.

Matches: 23/09/2024

Match a valid URL:

Pattern: https?://(www\.)?\w+\.\w+

String: Visit https://www.example.com or http://example.org

Matches: https://www.example.com, http://example.org

