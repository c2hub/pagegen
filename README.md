# pagegen
A C2 utility for generating c2hub webpages from template.

To use this tool, you will need to make two following files

1. pagelist.txt

contains a list of filenames to be "built" with pagegen.
No extension or .half extension should be used.

2. template.txt

contains a template, optimally html template, but should work with anything.
The place where you wish content to be placed should be marked with "%s".
Example of a template.txt:

    Hello, my name is %s, what is yours?

It is really just about the presence of %s;

## V2.0 Plans
In V2, pagegen will be more a preprocessor than just mass copy paster. This
will be new syntax for content:

    [p] This is a paragraph
    it can span many
    many lines
    [a href="website.com"] this is a link

It will also be possible to make elements inside elements:

    [p] this is a paragraph with a [a href="website.com", link] inside.

Nested elements spanning on multiple lines too?

    [div]
    [div][p] thing in a div
    [div][a] link in a div
