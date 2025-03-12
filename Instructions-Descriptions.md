# Instructions & Descriptions
This Markdown file provides descriptions of the reasons behind code implementations in various branches, including the main branch. For sections of code that require manual setup, this document will offer precise instructions on what to do.

## Main Branch
**Standard APA style**: The code allows for the APA style to be used with `numeric` in-text citations and the a`author-year` version.

**Instructions**:

For MikTeX users:
1. Locate the default `authoryear.cbx` in your installation path and replace it with the modified `authoryear.cbx` presented on this repository.
   - On Windows, this is typically found in:
       ```
       C:\Users\[Your Username]\AppData\Local\Programs\MiKTeX\tex\latex\biblatex\biblatex.def
       ```
       Here, `[Your Username]` represents your actual Windows username.
     
   - Or if you'd prefer another method:
     Copy the contents of `APA-Custom-Template.cbx` into the default `authoryear.cbx` right after line 8 (`\newbool{cbx:parens}`).
2. In the `APA-Custom-Template.tex` file, comment out the biblatex package on line 40 and use the biblatex package on line 42 instead.
3. In the `APA-custom-Template.bbx` file, comment out line 2 and use line 3 instead.

## Customising-BibLaTeX's.def-file branch
Building the project requires a `.def` file. The purpose of this branch is to use the default (source) `biblatex.def` but modify it by integrating the contents of `APA-Custom-Template.def`. This is a temporary measure until I can decide which sections I require for my `APA-Custom-Template.def` file. Once decided, I will load the `APA-Custom-Template.def` in the `.tex` file and use it instead.

**Instructions**:

For MikTeX users:

Locate the default `biblatex.def` in your installation path and replace it with the modified `biblatex.def` presented on this repository.
- On Windows, this is typically found in:
       ```
       C:\Users\[Your Username]\AppData\Local\Programs\MiKTeX\tex\latex\biblatex\biblatex.def
       ```
  Here, `[Your Username]` represents your actual Windows username.
- Before replacing, copy the default `biblatex.def` from your source or backup location to this path.
- Ensure you have administrative privileges to write to this directory or run your text editor as an administrator.
     
Or if you'd prefer another method:

Copy the contents of `APA-Custom-Template.def` **from line 5 to line 16**. Locate the original `biblatex.def` in your installation path and add the copied content to the macro `DeclareDriverSourccemap` on **line 1339**.
Remember, modifying system files like `biblatex.def` can affect other LaTeX documents you work on, so backup your current `biblatex.def` before making changes.

## Detailed-Explanation-of-Code branch
In this branch a detailed explanation of the main algorithms that make this APA referencing package unique has been explained. Furthermore, the key innovations have been listed.
