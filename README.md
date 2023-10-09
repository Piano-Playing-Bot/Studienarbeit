# LaTeX-Code für die Studienarbeit

## Generelle Notizen

-   Im Ordner `img/` lassen sich alle Bilder, die in der Arbeit verwendet werden, finden
-   Die Datei ["Allgemeine Hinweise für das wissenschaftliche Arbeiten"](hinweise-wissenschaftliche-arbeiten.md) fasst wichtige Hinweise und Best-Practices zum wissenschaftlichen Arbeiten zusammen
-   Die Datei [bibliography.bib](bibliography.bib) enthält alle Quellen für die Arbeit
-   Die einzelnen `.tex`-Dateien stellen die jeweiligen Kapitel der Studienarbeit dar. Die [master.tex](master.tex) Datei stellt dabei den Entry-Point für das LaTex-Projekt
-   [master.pdf](master.pdf) ist die resultierende PDF-Datei, nach Bau des LaTeX-Projekts

## LaTeX-Installation

### Prerequisites

First, you need a working LaTeX installation. Please find an appropriate one for your operating system, e. g.

-   Windows, Mac, Linux: [TexLive](http://www.tug.org/texlive/) (included in most Linux distributions)
-   Windows: [MikTex](http://www.miktex.org)
-   Mac: [MacTex](http://www.tug.org/mactex/index.html)

Next, you need a LaTeX Editor. Any text editor (e.g. vi/vim, atom, sublime etc.) will do the job. However, there are some LaTeX editors which support writing LaTeX-domuments specifically:

-   [TexStudio](http://www.texstudio.org) (platform independent)
-   [VSCode](https://code.visualstudio.com/) (platform independent) with the [LaTeX Workshop Extension](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)
-   [TexShop](http://pages.uoregon.edu/koch/texshop/) (Mac only)

## Explanation of the LaTeX template

In the LaTeX directory, the file **`master.tex`** is the LaTeX root file which can be compiled directly. All other `.tex`-files are incuded there.

The template files are commented in detail. Moreover, there is an instruction document **`anleitung.tex`** (in German) which explains the basic usage of the template.

Read the comments in all the `.tex`-files carefully, since you'll likely need to modify configurations and content, e.g. for disabling unused parts like the _List of Algorithms_ etc. The file **`config.tex`** includes relevant packages and provides a great portion of configuration settings. Nearly every property or characteristic can be configured/modified/addee here, beginning from page layout, header and footer, citation style etc. _If needed read the LaTeX package documentations at [CTAN](http://www.ctan.org)!_

Adapt in the `.tex`-files, in particular in `master.tex` and `config.tex`, especially all parts which are marked with **`@stud`**.

Citation examples are included in the file **`bibliography.bib`** -- articles, books, online references, etc.

Acronyms will be maintained in file **`acronyms.tex`**.

The acronyms list will then be generated automatically from this file upon compilation with LaTeX. Also lists of figures, tables, coding sections, algorithms will be generated automaticvally during LaTeX compilation if these items are properly captioned in the running text of your thesis -- see LaTeX instructions for details.

The GitHub bundle contains sample chapter and appendix files which may be adapted or extended. Additional chapter and appendix files can be provided and included in the `master.tex` file.

If you want to use a logo of your company replace the graphics file **`firmenlogo.jpg`** in folder `./img` by the logo of your company. Adjust the size of the logo by setting the scale factor of the image in **`titlepage.tex`**.
