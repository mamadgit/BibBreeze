# BibBreeze: A Referencing Package that Automates Bibliography Reconstruction

## Note
For information regarding the details and purpose of the branches of this repository, please read the `Instructions-Descriptions.md` markdown file. Also, to see the output and capabilities of this package please look at the `BibBreeze.pdf` as an example.

## Introduction
This LaTeX package, called `BibBreeze` written using `LaTeX3`, is a referencing package that automates bibliography reconstruction, eliminating manual effort in reference handling. It reorders disorganized fields for bibliography entries, fills in missing fields, and produces polished, referencing style-compliant bibliographies—optimized for researchers, academics, and writers. Currently, the package's referencing style is designed for APA (with both `numeric` and `author-year` in-text citations) with more styles (Harvard, Chicago, AMA, etc.) to come.
## Key Features

- **Advanced Automation**: Leverage algorithms that parse through bibliography data from `.bib` files, to automate the handling of incomplete or misstructured entries:
  - Recognises embedded entry fields, such as a `booktitle` field in conference proceedings entry that may combine the conference title, location, and date, and distributes them into their proper structure.
  - Differentiates between subtypes of entries sharing a single BibTeX key (e.g., `@inproceedings`), such as presented conference proceedings versus those published in books or journals.
  - Embeds actionable prompts directly in the bibliography output, providing instructions for manual edits when automated fixes aren’t sufficient.
- **Designed for Academic Use**: Also tailored for journals requiring APA referencing with `numeric` in-text citation, offering a time-saving solution for academic writing.
  - **Note:** Users wishing to use the standard APA style (`author-year` in-text citation) can do so with a simple modification, as explained in the `BibBreeze.tex` file or in the `Instructions-Descriptions.md` file.
- **Seamless Integration**: Works effortlessly with LaTeX projects using BibLaTeX.

- **Full APA 7th Edition Compliance**: Accurately implements all guidelines of the APA 7th edition for various entry types such as articles, books, conference proceedings (presented, published in journals or books), and theses (PhD and masters).
  
## Why This Template?
- Other widely used referencing packages, such as BibLaTeX's default APA style and Springer Nature's universal referencing package, lack this level of automation. For example:
  - They may overdeliver by printing unnecessary fields, such as a paragraph-long `note` field.
  - They are unable to recognise embedded fields.
  - They cannot distinguish between subtypes of an entry sharing the same BibTeX key.
  - They do not prompt users with instructions when critical fields are missing.
    
- **Strict APA 7th Edition Compliance**: Adheres to the strict guidelines of the APA 7th edition, down to correct order and punctuation. To the observations and tests of this developer, other packages have notable flaws in this regard, such as:
  - Missing "&" for two or more authors in the Springer Nature's package.
  - Printing duplicate "http" prefixes in URLs or DOIs in BibLaTeX's default APA style.
  - Including unnecessary fields by APA standards such as paragraph-long notes in both APA packages (BibLaTeX's default and Springer Nature), leading to non-compliant output.
- **Superior Solution for Referencing**: By addressing these automation and compliance issues, the `BibBreeze` package provides a superior solution for accurate referencing, reducing manual effort and ensuring consistency across academic writing.

## Installation and Setup
1. Clone this repository: https://github.com/mamadgit/BibBreeze.git
2. Include the template in your LaTeX project:
- Add the provided `.bbx` and `.dbx` files to your project directory.
- Configure BibLaTeX to use this style in your `.tex` file (according to the `.tex` provided).
3. Compile your document using a LaTeX editor (e.g., Overleaf, TeXShop) with BibLaTeX enabled.

## Contributing and Feedback
This project is open to contributions! If you have suggestions, bug reports, or feature requests, please open an issue or submit a pull request. Feel free to star this repository if you find it useful!
