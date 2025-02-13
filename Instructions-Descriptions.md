# Instructions & Descriptions
This Markdown file provides descriptions of the reasons behind code implementations in various branches, including the main branch. For sections of code that require manual setup, this document will offer precise instructions on what to do.

## Main Branch
**Standard APA style**:The code allows for the APA style to be used both with numeric in-text citations and the standard version.

**Instructions**:
1. In the `APA-Custom-Template.tex` file, comment out the biblatex package on line 40 and use the biblatex package on line 42 instead.
2. In the `APA-custom-Template.bbx` file, comment out line 2 and use line 3 instead.

## Customising `biblatex.def` File
Building the project requires a `.def` file. The purpose of this branch is to use the default (source) `biblatex.def` but modify it by integrating the contents of `APA-Custom-Template.def`. This is a temporary measure until I can decide which sections I require for my custom `.def` file. Once decided, I will load this custom `.def` in the `.tex` file and use it instead.

**Instructions**:
1. **Replace the Modified `biblatex.def`**: Locate the modified `biblatex.def` in your installation path and replace it with the original version.
2. **For MikTeX Users**:
   - Navigate to your user-specific MikTeX installation directory:
     - On Windows, this is typically found in:
       ```
       C:\Users\[Your Username]\AppData\Local\Programs\MiKTeX\tex\latex\biblatex\biblatex.def
       ```
   - Here, `[Your Username]` represents your actual Windows username.
   - Copy the original `biblatex.def` from your source or backup location to this path.
   - Ensure you have administrative privileges to write to this directory or run your text editor as an administrator.

Remember, modifying system files like `biblatex.def` can affect other LaTeX documents you work on, so backup your current `biblatex.def` before making changes.