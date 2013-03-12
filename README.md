pdfx-ext
========

Updated and extended version of LaTeX package pdfx by River Valley. According to the LPPPL, this new version has to have a new name to avoid confusion.

It mostly focuses on PDF/A-1b compliance and eventually including a reference list in the XMP metadata.

The original package was distributed under the LaTeX Project Public License; this is too.

Basic install instructions:
- put *.xmp, pdfx-ext.sty and glyphtounicode-cmr-tex in a directory pdfx-ext in $TEXMF/tex/latex
- update the TeX package catalog

Usage instructions:
- create a <project>.xmpdata file containing the metadata
- copy the .icm file in your project directory
- run pdfLaTeX as usual.
