# L 4 LaTeX

A 2 -day Workshop on Introduction to LaTeX on 05 February 2022 organized by *Poetry of Reality*

## Day 1

Please find the source code and PDF of presentation from [here](Day 1/presentation) and the sample document from [here](Day 1/test_doc).

### Installation of Texlive in GNU/Linux based systems (eg:- Ubuntu)

1. Installation using terminal:

     For full Texlive installation [~3 GB download]:

    `sudo apt install texlive-full`

   For basic installation:

   `sudo apt install texlive texlive-latex-recommended texlive-latex-extra texlive-science`

2. Install Texstudio for editing LateX files.

    `sudo apt install texstudio`

3. For package installation, search class or style file using Terminal first and install necessary package.

   `apt search geometry`

    From listed packages, install necessary one.

4. Package installation using `tlmgr`. We can also use `tlmgr` for installing packages.

    `tlmgr install geometry`

### MikTeX installation in Windows.

- Please follow the following link for detailed information on [MikTeX installation](https://miktex.org/howto/install-miktex)

- Download Installation file from [here](https://miktex.org/download)

- Download Texstudio from [here](https://www.texstudio.org/)

### A sample Document

Please save the following content in a file with name `document.tex`. Open in Texstudio and use `Build & View` button  (or press F5) to comple and view the PDF file.

```
    \documentclass[a4paper, 12pt]{article}

    \begin{document}

    This my first \LaTeX document!.

    \end{document}

```

### Some references

1. [Overleaf learn LaTeX in 30 minutes](https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes)

2. [LaTeX Primer](https://www.tug.org/twg/mactex/tutorials/ltxprimer-1.0.pdf)

## Day 2
