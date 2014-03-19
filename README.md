4x5-Font
========

A 4x5 font for small displays.

`4x5-font.js` contains a javascript object describing the font.
Key/Value pairs are character/mapping pairs. Mapping is list of rows (4 bits).

Works in Python (remove `var`):

    python3
    >>> char_map = ...
    >>> char = 'A'
    >>> for row in char_map(char_map[char]):
    ...     print(bin(row))
    ...
    0b0100
    0b1010
    0b1110
    0b1010
    0b1010

That's an uppercase 'A':

     *
    * *
    ***
    * *
    * *
