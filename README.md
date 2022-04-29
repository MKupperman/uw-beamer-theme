# Oregon State University Beamer Theme

## Description

Authors: Michael Kupperman

_A custom Beamer theme for the University of Washington._

Derived largely from [Jeremy Lilly's Oregon State University Beamer Theme](https://github.com/jeremy-lilly/osu-beamer-theme).

## Usage

To use, place all five `.sty` files and the `uw_theme_images` directory into your working directory and add

`\usetheme{UW}`

to the preamble of your main Beamer presentation `.tex` file.

### User Defined Macros

This theme allows the user to define the following macros that are used throughout the document:

- `title`
- `subtitle`
- `author`
- `department`
- `institute`
- `titlegrapic`

For example:

```latex
\title[Short Title]{Long Title}
\subtitle{Subtitle}
\author{Jane Doe\inst{1} \and John Doe\inst{2}}
\department{Applied Mathematics}
\institute{
    \inst{1}Very Fancy University \\
    \inst{2}Another Fancy University
}
\titlegraphic{\includegraphics[scale=0.05]{images/placeholder.png}}
```

**Note:** Not all these must be defined. The user may define whichever they like, and the document will change appearance accordingly.

## Compilation

This theme uses UW's official font UniSans, and as such should be complied with **LuaLaTeX** or **XeLaTeX**. The font package is included in this repository.
When compiled on most LaTeX IDEs the command on line 1 on main.tex will override the default compiler choice in favor of LuaLaTeX.

However, if you do wish to compile with **pdfLaTeX**, you may do so and obtain the default romanized font for the header text layers. Simply remove line 1 from `main.tex`.

## Helpful Resources

- [An Introduction to Beamer](https://www.overleaf.com/learn/latex/Beamer_Presentations:_A_Tutorial_for_Beginners_(Part_1)%E2%80%94Getting_Started)
- [Beamer Documentation](http://tug.ctan.org/macros/latex/contrib/beamer/doc/beameruserguide.pdf)
- [Beamer Structure Guide](http://www.cpt.univ-mrs.fr/~masson/latex/Beamer-appearance-cheat-sheet.pdf)
