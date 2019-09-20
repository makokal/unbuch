A simple pandoc setup to compile a book from markdown sources into html pages and pdf based on pandoc and python filters.

Features:

* Tufte-inspired layout with sidenotes
* Latex formulas via katex plugin
* Environments
* HTML and PDF output

# Example

Check out [fairmlbook.org](https://fairmlbook.org) for a real example.

# Getting started

1. Install [pandoc](https://pandoc.org/) v2.2 or higher and [pandoc-citeproc](https://github.com/jgm/pandoc-citeproc)
2. Make sure you have python 2.7 installed with [pandocfilters](https://github.com/jgm/pandocfilters) package
3. Make sure you have `libbrsvg` installed. For Mac `brew install librsvg`, Ubuntu `apt install librsvg2-bin`
4. Clone the repository
5. Customize your book by setting up variables in `Makefile`.
6. Type `make` to build both pdf and html files.
  - To build html only, type `make html`.
  - To build pdf only, type `make pdf`.

Find the compiled results in `publish/` directory.

# Dependencies

- `pandoc` v2.2 or higher
- `python` 2.7 with `pandocfilters` installed

The workflow was developed and tested with:
- pandoc v2.2, python 2.7, Ubuntu 18.04 LTS

# Special files and folders

* `assets` -- Put all files linked to from the sources here
* `css` -- All css files
* `filters` -- Pandoc filters
* `sources` -- This is where the source files live. Go here to edit.
* `templates` -- Pandoc template files
* `publish` -- Contains compiled pages and pdfs ready for publishing. DO NOT EDIT.

# Credits

The setup is based on:

* [tufte-pandoc-css](https://github.com/jez/tufte-pandoc-css)
* [tufte-css](https://github.com/edwardtufte/tufte-css)
* [pandoc-sidenote](https://github.com/jez/pandoc-sidenote)

# Current issues

See `Issues` tab for current issues and ways of contributing to the project.

Thank you.
