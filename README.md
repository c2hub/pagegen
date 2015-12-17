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
