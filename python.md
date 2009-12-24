Indentation
-----------

Use tabs for indentation, and spaces for alignment.

For the sake of this section, tabs will be represented with arrows (--->).

For example, a dictionary may be declared as such:

    errors = {
    --->'not_found':            'The record was not found.',
    --->'invalid_id':           'The record ID is invalid.',
    --->'undefined_or_unknown': 'The record was undefined or unknown.',
    }

When nesting non-trivial dictionaries, lists and tuples, put each item on its own line, with the first immediately following the opening brace, and all others lining up with it:

    dictionary = {
    --->'1': 'one',
    --->'2': ('two', 'dos'),
    --->'5': {'cinco': 'five',
    --->      '6-1':   '5'},
    }

Spacing
-------

One space:

  - before and after operators
  - before, but not after, function calls
  - not before, but after, commas, colons and semicolons

Parens have no spaces around them.

Example:

    for i in [(2 ** n) for n in range(1, 6)]:
        ...

Use blank lines to break up blocks of code. In general, there will be about 5 lines of code in a block. Don’t use more than one blank line in a row.

Identifier Names
----------------

Use meaningful names. Avoid single-letter variables, except as counters in loops. Try to avoid using abbreviations; if you do, make sure that the same abbreviation is used everywhere.

Constants: `UPPERCASE_WITH_UNDERSCORES`

Classes: `UpperCamelCase`

Functions/methods: `lowercase_with_underscores`

Variables: `lowerCamelCase`

Functions/Methods
-----------------

Try to avoid functions over 50 lines. If you find yourself writing a long function, you should probably extract out parts to separate functions.

Comments
--------

Comments should be indented to the same level as the code to which they refer, and always on their own line.

If used to comment out code, there should be no space between the comment and the code. If used as documentation, leave one space between.

    def foo(a, b):    
        # first, get the product of a and b.
        c = a * b
        
        # now call a function
        callFunc(c)
        
        # this code is no longer needed
        #oldFunc(a, b)
        #c -= b
        
        return c

