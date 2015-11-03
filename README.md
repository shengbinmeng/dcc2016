Academic paper for DCC 2016.

Files:
- dccpaper.cls: LaTeX class file
- IEEEbib.bst: BiBTeX style file with bibliography style definitions
- dcc2016.tex: the paper in LaTeX
- refs.bib: file of bibliographic references
- Figures/：folder for image files
- Makefile: provides for automatic LaTeX compilation and PDF generation

It is recommended to use the included Makefile to produce the PDF document to
submit to the conference:

  - "make": runs LaTeX and BiBTeX to produce the file dcc_paper.dvi.
            Multiple runs are conducted as needed to resolve cross references.
  - "make pdf": produces a format-compliant PDF, dcc_paper.pdf, for
                submission. dvips and ps2pdf are used to completely embed and
                subset all fonts.

The Makefile should work on any modern Unix system with dvips and ps2pdf
installed. Windows users will either need to compile by hand or install
Cygwin (http://cygwin.com/).
