pdfx-ext
========

Updated and extended version of LaTeX package [pdfx](http://ctan.org/pkg/pdfx) by River Valley. According to the LPPPL, this new version has to have a new name to avoid confusion.

It mostly focuses on PDF/A-1b compliance and eventually including a reference list in the XMP metadata.

The original package was distributed under the LaTeX Project Public License; this is too.

Goals
-----
I had a few ideas for this package:
 * [x] support all constructs of the original package (including Subject, which wasn't implemented before)
 * [ ] comply with the PDF/A standard (which has its quircks, like allowing at most one dc:creator in PDF/A-1)
 * [x] allow the author's URI to be embedded as dcterms:creator
 * [x] embed a subset of the PRISM vocabulary in XMP in the PDF/A prescribed way (partially complete)
 * [ ] embed (subsets of) the FaBiO and CiTO ontologies in XMP in the PDF/A prescribed way
 * [ ] use XMP to embed a layout style-independent and machine readable reference list
 * [ ] provide a construct (macro, or a program) to convert BibTeX to PRISM+CiTO statements in XMP
 * [ ] be a reference implementation for connecting PDF documents created from LaTeX to the Semantic Web/Web of Data :)

Instructions
------------
Basic install instructions:
- put *.xmp, pdfx-ext.sty and glyphtounicode-cmr-tex in a directory pdfx-ext in $TEXMF/tex/latex
- update the TeX package catalog

Usage instructions:
- create a <project>.xmpdata file containing the metadata
- copy the .icm file in your project directory
- add \usepackage{pdfx-ext} to the preamble of your LaTeX document
- run pdfLaTeX as usual.
