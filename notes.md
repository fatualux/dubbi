# Notes

## Python

- Dictionaries
- Docstrings
- Return of a function
    - ***print***
        - **Commas**:
            - Best for simple, quick print statements where you don't need complex formatting.
            - Handles different types automatically.
        - **String Concatenation with +**:
            - Useful when you need to build a string dynamically, but you must ensure all parts are strings.
            - Requires manual conversion of non-string types.
        - **f-strings**:
            - Ideal for more complex or dynamic string formatting.
            - Automatically handles different types and allows inline expressions.

- **DO NOT to modify** global variables with `global` inside a local/enclosing scope; this is prone to produce issues.

- **Global constants ** should be named in **uppercase**.