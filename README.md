# Template files for submissions to the Annual Conference of the Cognitive Science Society
# with thanks to Roger Levy for perparing and organizing the most recent version of these files.

This repository contains new LaTeX template files
for submissions to the Annual Conference of the Cognitive Science
Society, to be used starting with the 2019 conference:

The simplest way to download and use these templates is to click on
the green **Clone or download** button at the right-hand side of this
page above all the file names, and choose **Download ZIP**.
Alternatively, you can use [Git](https://git-scm.com) to clone this repository
yourself.

TWO IMPORTANT NOTES:

1) DOUBLE-BLIND REVIEWING

As in 2019, 2020, and 2021, for the 2022 conference, 6-page paper submissions will be reviewed
double-blind, so submissions must be anonymized.  The template files
you will find in this repository have been updated from the template
files from previous years reflecting this change to anonymized paper
submissions.

** The policy for double-blind reviews will be strictly enforced in 2022.
Please ensure your submissions are anonymized before submission.  **

2)  CC-BY LICENSING

An online proceedings will be published by the Cognitive Science Society. 
At the time of final (camera-ready) submission authors will be required to 
agree to release of their proceedings contribution under a CC-BY license. 
This means that authors allow free reuse of their work provided the original 
authors are attributed. Please see the submissions website for more details.  

## Preparing an anonymized submission

If you are using the Word template, simply replace the **How to Make a
Proceedings Paper Submission** title with the title of your submitted
paper, and then replace the formatting instructions

If you are using the LaTeX template, make sure that the
`\cogscifinalcopy` command is commented out.  

In either case, remember that you need to leave at least 2.75 inches
between the top of the first page and the abstract & text of your
paper.  Since the top margin needs to be 1 inch on all pages, this
means that there needs to be at least 1.75 inches of space on page 1
in which nothing but your paper title and **Anonymous CogSci
submission** appears.  Additionally, please remember not to include
acknowledgments in the final version of your paper.

## Preparing the de-anonymized final version of your accepted paper

Uncomment the `\cogscifinalcopy` command and
recompile.  The file `cogsci_template_final_version_deanonymized.pdf`
provides an example of author list & affiliation formatting.

In the final version of the paper, the title, author, abstract, and
text of the paper must fit within six pages.  Unlimited additional
pages can be used for acknowledgments and references.  In the final
version of the paper for the proceedings (but not the initial
anonymized submission), be sure to include any acknowledgments that
may be appropriate.

Once again, make sure that you adhere to the general formatting
instructions, including that there are at least 2.75 inches between
the top of page 1 and the start of the abstract and text.

## Bibliography System

This template uses **BibLaTeX with Biber backend** and follows **APA 7th edition**
style guidelines. This is an upgrade from the older BibTeX/natbib system with
APA 6th edition.

**For LaTeX users:**
- Bibliography entries go in `CogSci_Template.bib`
- The template is configured to use `\cite{}`, `\citet{}`, and `\citep{}` commands
- Compile with: `pdflatex` → `biber` → `pdflatex` → `pdflatex`
- Or use `latexmk -pdf` to handle the compilation automatically

