A template for theses
=====================

This LaTeX code comes from 
[my dissertation](https://ediss.sub.uni-hamburg.de/volltexte/2020/10455/pdf/Dissertation.pdf)
and I like the style, so I make it available for adoption.  Use
everything in here freely as you want, pick & choose.

This code is based on LuaTeX and biblatex, which makes everything so
much nicer to use (proper font support! unicode support! easy
customization of bibliography styles!).

You need to run `lualatex` to compile the tex files and `biber` to
generate the bibliography.

The bibliography style slightly differs from my dissertation and is
more in line with the ACL style.

The Makefile
------------

The Makefile automatically builds the latex code using `latexmk`.  It
records missing files and tries to generate them.  This means that you
can have a file `image.svg` include it with
`\includegraphics{image.pdf}` and the Makefile will automatically call
inkscape to convert the SVG to PDF.

Please don't treat the Makefile as some magic, it only helps you in
the long run if you understand what's going on.
