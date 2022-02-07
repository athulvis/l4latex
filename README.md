# L 4 LaTeX

A 2 -day Workshop on Introduction to LaTeX on 05 February 2022 organized by **Poetry of Reality**

## Day 1

Please find the source code and PDF of presentation from [here](https://github.com/athulvis/l4latex/tree/main/Day%201/presentation) and the sample document from [here](https://github.com/athulvis/l4latex/tree/main/Day%201/test_doc).

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

Presented by Manosh T M

Source code of sample documents can be found in [Day 2](https://github.com/athulvis/l4latex/tree/main/Day%202) folder.

- Sample article - [Link](https://github.com/athulvis/l4latex/tree/main/Day%202/My_article)

- Sample book - [Link](https://github.com/athulvis/l4latex/tree/main/Day%202/BOOK)

- Sample report - [Link](https://github.com/athulvis/l4latex/tree/main/Day%202/My_report)

- Sample presentation - [Link](https://github.com/athulvis/l4latex/tree/main/Day%202/ppt)

### Sample Codes

#### Different types of documents

- Article

```
\documentclass[11pt,a4]{article}

```
- Book

```
\documentclass[11pt,a4]{book}
```
- Report

```
\documentclass[11pt,a4]{report}
```
- Presentation

```
\documentclass[11pt]{beamer}
```

#### Import Necessary packages

Necessary packages for creating a scientific document are given below:

| Package Name | Purpose |
| ------------ | ------- |
| graphicx | Adding images |
| amsmath | Mathematical equations |
| amssymb | Mathematical symbols |
| inputenc | Different input encodings like Unicode |
| fontenc | Font encodings |
| geometry | Change page structure |
| hyperref | Hyperlink |

#### Add title and author

Add below in preamble (before `\begin{document}`

```
\title{add title}
\author{ Author name}
\date{\today}
```
Also use `\maketitle` after `\begin{document}`.

#### Add Abstract

```

\begin{abstract}

Add abstract text.

\end{abstract}
```

#### Add section and subsection

- Seciton
```
\section{section title} for section name with number.

\section*{section title} for section name without number.
```
- Subsection
```
\subsection{subsection title} for subsection name with number.

\subsection*{subsection title} for subsection name without number.
```

#### Equation

```
\begin{equation}
\frac{\partial y}{\partial t}=\oint\alpha\beta\sqrt{x^2+y^2} dx
\label{My_eq}
\end{equation}
```
#### Images

```
\begin{figure}[h]
    \centering
    \includegraphics[width=5cm]{images/fig1}
    \caption{My first image}
    \label{fig:1}
\end{figure}
```
#### Table

```
\begin{table}[h]
    \begin{center}
        \begin{tabular}{|c|c|r|c|}
            \hline
            \rule[-1ex]{0pt}{2.5ex} Name & Place & Age & Remarks \\
            \hline
            \rule[-1ex]{0pt}{2.5ex} Appu & EKM & 12 &  \\
            \hline
            \rule[-1ex]{0pt}{2.5ex} Ammu & TVM & 13 &  \\
            \hline
            \rule[-1ex]{0pt}{2.5ex} Hari & USA &12  &  \\
            \hline
            \rule[-1ex]{0pt}{2.5ex} Basi & JAP  & 7 &  \\
            \hline
            \rule[-1ex]{0pt}{2.5ex} Athul & PLUTO & 20 &  \\
            \hline
        \end{tabular}
    \end{center}
\caption{My table}
\label{tab:1}
\end{table}
```

#### Bulleted items

```
\begin{itemize}

    \item text 1
    \item text 2

\end{itemize}
```

Use `\enumerate` for numbered items.

#### Bibliography

- Save the bibtex files in some file (eg: ref) with `.bib` extension.

A bibtex example is given below:

```
@article{PhysRevLett.128.057702,
  title = {Scattering between Minivalleys in Twisted Double Bilayer Graphene},
  author = {Tomi\ifmmode \acute{c}\else \'{c}\fi{}, Petar and Rickhaus, Peter and Garcia-Ruiz, Aitor and Zheng, Giulia and Portol\'es, El\'{\i}as and Fal'ko, Vladimir and Watanabe, Kenji and Taniguchi, Takashi and Ensslin, Klaus and Ihn, Thomas and de Vries, Folkert K.},
  journal = {Phys. Rev. Lett.},
  volume = {128},
  issue = {5},
  pages = {057702},
  numpages = {7},
  year = {2022},
  month = {Feb},
  publisher = {American Physical Society},
  doi = {10.1103/PhysRevLett.128.057702},
  url = {https://link.aps.org/doi/10.1103/PhysRevLett.128.057702}
}
```
- Add below text to main latex document in the end section.

```
\bibliographystyle{plain}
\bibliography{ref}
```

#### Create Presentation

Using texstudio template, a beamer presentation can be created easily.

- Add `beamer` in documentclass
- Use desired theme
- Add frames inside `\begin{document}`. Example is given below.

```
\begin{frame}
    \frametitle{Intro}

    Slide text

\end{frame}

```

