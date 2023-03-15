# Latex Syntax for elegent note taking 

### Ref: https://www.overleaf.com/learn/latex/

### Document types
```

article for articles in scientific journals, presentations, short reports, program documentation, invitations, ...

proc a class for proceedings based on the article class.

minimal is as small as it can get. It only sets a page size and a base font. It is mainly used for debugging purposes.

report for longer reports containing several chapters, small books, thesis, ...

book for real books

slides for slides. The class uses big sans serif letters.

memoir for changing sensibly the output of the document. It is based on the book class, but you can create any kind of document with it (1)

letter For writing letters.

beamer For writing presentations

```

### Boiler plate 

```
\documentclass{article}
\usepackage{ulem}

\title{}
\author{}
\date{\today}

\begin{document}
	\section{}

\end{document}


```


### formating

```
These format only a little bit of text at a time. Because they only affect a small
amount of text, these commands are a single command that receives the text
in curly braces ({ and }) afterwards. Some important examples we will use are
below. To show what they do, the actual command is used on the text in curly
braces.

• \textbf{Text to write in bold}

• \textit{Text to write in italics}

• \underline{Text to underline}

• \sout{Text to strike out} You will need to use the ulem package (see
Section 6.3)

• \textsc{} writes text in all capital letters


```

### Centering Text
```
\begin{center}

\end{center}


\begin{align*}

.\end{align*}
```

### Right/Left Alignment

```
\begin{flushright}
\end{flushright}

\begin{flushleft}}
\end{flushleft}

```

### indentation

```
\hspace{\parindent}
```


### Text Sizes 
```
tiny
scriptsize
footnotesize
small 
normalsize
large
Large
LARGE
huge
```

### Quotes 

```
For quotes in latex, use backticks

`this is a quote`
```

### Lists 
```

Lists are easy to create:

\begin{itemize}
  \item List entries start with the \verb|\item| command.
  \item Individual entries are indicated with a black dot, a so-called bullet.
  \item The text in the entries may be of any length.
\end{itemize}

\begin{enumerate}
  \item List entries start with the \verb|\item| command.
  \item Individual entries are indicated with a number system
  \item The text in the entries may be of any length.
\end{enumerate}

\begin{description}
  \item[word] List entries start with the \verb|\item| command.
  \item[word] Individual entries are indicated with a emphasized first word 
  \item[\huge{word}] The text in the entries may be of any length.
\end{description}

```


### Sections and Subsections
```
\section{title} These are the larger sections. They have a single number and
the title. “More Stuff” is a section.

\subsection{title} These are the smaller sections within the section most 
recently declared in the .tex file. They have two numbers separated by a
period (.). “Sections and Subsections” is a subsection of “More Stuff.”

```

### Packages

```
Like in any programming language, other people have made things that can
improve our coding lives. Many of these packages already come with a standard
LaTeX install (Miktex for Windows and TexLive for Linux), and other ones can
be downloaded and placed in the same directory as the .tex file. To use the
package in a document, the command \usepackage{packageName} must appear
after the \documentclass command. Some packages have special parameters
that appear in brackets before the package name. Some common packages to
include are:

• \usepackage{amsmath}, \usepackage{amsfonts}, and \usepackage{amssymb}
form the set of AMS (American Mathematics Society) packages that the
TexMaker IDE always suggests. With these three packages, almost every
math symbol is available.

• \usepackage[margin=XX]{geometry} can cheat the margins when you want
to save trees or specify particular guidelines. Replace XX with a floatingpoint number followed by a unit of measurement such as ‘in’ or ‘cm’ (no
space between the number and unit).

• \usepackage{graphicx} allows graphics to be rendered in the document.
It is a necessary evil in LaTeX.

• \usepackage{epsfig} allows PostScript images to be rendered in the document. It is a slightly less evil in LaTeX since the bounding boxes can be computed for you.

• \usepackage[normalem]{ulem} allows some other emphasis in-line formatting commands such as \sout.

```

### Instering graphics

```
\usepackage{graphicx}
\graphicspath{ {/path/to/image} }
\includegraphics[scale=1.5]{image.png}
```


