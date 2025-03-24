# Instructions & Descriptions
This Markdown file provides descriptions of the reasons behind code implementations in various branches, including the main branch. For sections of code that require manual setup, this document will offer precise instructions on what to do.

## Main Branch
**Standard APA style**: The code allows for the APA style to be used with `numeric` in-text citations and the `author-year` version. To use `author-year` in-text citations please follow the instructions below.

**Instructions**:

For MikTeX users:
1. In the `BibBreeze.tex` file, set the `citestyle` of the `biblatex` package to `BibBreeze-authoryear`.
2. In the `BibBreeze.bbx` file, set the `numeric` of `RequireBibliographyStyle` as `BibBreeze-authoryear`.

## Customising-BibLaTeX's.def-file branch
Building the project requires a `.def` file. The purpose of this branch is to create my own custom `.def` file based on my needs. However, for now I am using a modified version of the default `biblatex.def` (for MikTeX users) renamed to `BibBreeze.def`. This is a temporary measure until I can decide which sections I require for my own custom `BibBreeze.def` file.
