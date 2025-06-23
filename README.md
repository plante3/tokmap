# tokmap

tokmap: iterate over a token list expandably, without dropping spaces or braced groups.

Usage: `\tokmap <command> { <tokens> }` applies command over the token list tokens.
Space tokens, left and right braces are replaced with the marker tokens `\tokmap@space`,
`\tokmap@bgroup`, and `\tokmap@egroup` respectively (who are `\ifx`-equal to themselves
exclusively). For convenience, command may contain multiple tokens.
It is assumed that `{` and `}` are the only characters with category codes 1
(beginning of group) and 2 (end of group) respectively.
Expandable.

This package may be used in LaTeX by `\usepackage{tokmap}`, or
in plain TeX and other formats by `\input{tokmap}`.

See the [visualtoks](https://ctan.org/pkg/visualtoks) package for an example application.

Copyright (C) 2025 plante
Version 1.0
This package is released under the LaTeX Project Public License (LPPL) 1.3c.
