---
layout: post
title: "Improve Latex compilation time"
date: 2018-05-21 15:46 +0200
categories: tips latex
---

# Short answer
Convert all graphic files from `png` to **`pdf`**, the compilation time can be *20 times* faster.

# Testing
Heavy graphics is the bottle neck of Latex compilation, so I make experiments to see which type of graphics affects the performance the most. I have a latex project with structure

~~~
.
+-- jpg
|  +-- img_*.jpg
+-- png
|  +-- img_*.png
+-- jpgpdf
|  +-- img_*.pdf
+-- pngpdf
|  +-- img_*.pdf
+-- doc.tex
~~~

where `jpg`, `png`, `jpgpdf`, and `pngpdf` are folders of 1000 images in corresponding extentions. `jpgpdf` contains pdf file converted from `jpg`, and so does `pngpdf`. The latex file `doc.tex` is

~~~
\documentclass{article}

\usepackage{graphicx}
\usepackage{float}
\usepackage{subfig}
\usepackage{pgffor}

\begin{document}
    \foreach \n in {1,...,1000}{
     \begin{figure}[H]
         \includegraphics[width=0.5\linewidth]{pngpdf/img_\n}
         \caption{\n}
     \end{figure}
    }
\end{document}
~~~
So, by changing the `includegraphics` argument, I could test the compilation time of different formats.

# Results

| Experiement | Size of 1 file | Compilation time | Output .pdf size |
|---------|---------|---------|---------|
| jpg	| 165K | 9.6 sec | 165M |
| png	| 80K | 1 min 32 sec | 56.1 M |
| jpgpdf | 183K | 2 sec | 173.8 M |
| pngpdf | 80K | 1.5 sec | 59.2 M |

So the final conclusion for graphic file is **`PDF with PNG > PDF with JPG > JPG > PNG`**

# Other approaches
1. Use `\include` and `\includeonly`
2. Use `draftmode`

# Tips
Use `ImageMagic` to convert with simple command `convert image.png image.pdf`