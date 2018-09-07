# Flux beamer

Flux is a modern style beamer presentation. It is based on simple design patterns and flat colors.

Available as template on [Overleaf](https://www.overleaf.com/latex/templates/flux-beamer/vhzbnhyymddd#). 

> Disclaimer: This theme is mainly optimized for personal needs and shared without guarantees.

## Demos

![alt text](https://github.com/pvanberg/flux-beamer/blob/master/demo.png)

## Themes

Flux provides five differents color palettes. (asphalt, blue, red, green, gray)

![alt text](https://github.com/pvanberg/flux-beamer/blob/master/demo_themes.png)

## Minimal Working Example

```
\documentclass[9pt]{beamer}
\usepackage[sfdefault]{roboto}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usepackage{styles/fluxmacros} 	% Define where theme files are located. 
\usefolder{styles}
\usetheme[style=asphalt]{flux} % Available styles: asphalt, blue, red, green, gray 

\title{Flux beamer template}
\subtitle{Modern theme v0.1}
\author{John Doe}
\institute{Institute, location}
\date{\today}
\titlegraphic{assets/overleaf.png}

\begin{document}

\titlepage 

\begin{frame}
 \frametitle{Table of contents}
 \tableofcontents
\end{frame}

\end{document}
```

## Compilation

Due to the use of bibliography and tikz figures, the compilation sequence must follow:

```
pdflatex demo.tex
biber demo.tex
pdflatex demo.tex
pdflatex demo.tex
```

