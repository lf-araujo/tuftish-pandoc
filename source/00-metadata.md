---
title: Tuftish-pandoc Book/Handout Style
author: lf-araujo
date: !today
bibliography: source/Link para library.bib
csl: style/chicago-fullnote-bibliography.csl
suppress-bibliography: yes
link-citations: true
lang: pt-br
papersize: a4
mainfont: Fira Sans
monofont: Fira Mono
monofontoptions: Scale=0.7
colorlinks: yes
linkcolor: Mahogany
citecolor: Mahogany
urlcolor: Mahogany
documentclass: memoir 
classoption: oneside 
link-citations: true
toc: yes 
header-includes: |
	\usepackage{graphicx}
	\setkeys{Gin}{width=\linewidth,totalheight=\textheight,keepaspectratio}
	\setlength{\baselineskip}{14pt}
	\setlength{\normalbaselineskip}{14pt}
	\settrims{0pt}{0pt}
	\settypeblocksize{49\baselineskip}{107mm}{*}
	\setlrmargins{24.8mm}{*}{*}
	\setulmargins{27.4mm}{*}{*}
	\setheadfoot{\baselineskip}{\baselineskip}
	\setheaderspaces{*}{2\baselineskip}{*}
	\setmarginnotes{8.2mm}{49.4mm}{\onelineskip}
	\checkandfixthelayout
	\RequirePackage{ragged2e}
	\AtBeginDocument{\RaggedRight}
	\setmpjustification{\RaggedLeft}{\RaggedRight}
	\setlength{\RaggedRightParindent}{1.0pc}
	\setlength{\parindent}{1pc}
	\setlength{\parskip}{0pt}
	\newcommand\loosesc[1]{ {\addfontfeature{LetterSpace=8}#1}}
	\makepagestyle{tufte}
	\makeoddhead{tufte}{}{}{\loosesc{\rightmark}\quad\thepage}
	\makeevenhead{tufte}{\thepage\quad\loosesc{\leftmark}}{}{}
	\makeevenfoot{tufte}{}{}{}
	\makeoddfoot{tufte}{}{}{}
	\makepsmarks{tufte}{
	\createmark{chapter}{left}{nonumber}{}{}
	\createmark{section}{right}{nonumber}{}{}
	\createplainmark{toc}{both}{\contentsname}
	\createplainmark{lof}{both}{\listfigurename}
	\createplainmark{lot}{both}{\listtablename}
	\createplainmark{bib}{both}{\bibname}
	\createplainmark{index}{both}{\indexname}
	\createplainmark{glossary}{both}{\glossaryname}}
	\setlength{\headwidth}{\textwidth}
	\addtolength{\headwidth}{\marginparsep}
	\addtolength{\headwidth}{\marginparwidth}
	\makerunningwidth{tufte}{\headwidth}
	\makeheadposition{tufte}{flushright}{flushleft}{}{}
	\renewcommand{\footnotesize}{\fontsize{8pt}{10pt}\selectfont}
	\renewcommand{\foottextfont}{\footnotesize}
	\footmarkstyle{{#1. }}
	\setlength{\footmarkwidth}{0em}
	\setlength{\footmarksep}{-\footmarkwidth}
	\footnotesinmargin
	\setsidecaps{\marginparsep}{\marginparwidth}
	\sidecapmargin{outer}
	\setsidecappos{t}
	\renewcommand*{\sidecapstyle}{%
	\captionnamefont{\foottextfont\scshape}
	\ifscapmargleft
	\captionstyle{\RaggedLeft\footnotesize\foottextfont}%
	\else
	\captionstyle{\RaggedRight\footnotesize\foottextfont}%
	\fi}
	\newlength{\fullwidthlen}
	\setlength{\fullwidthlen}{\marginparwidth}
	\addtolength{\fullwidthlen}{\marginparsep}
	\newenvironment{fullwidth}{%
	\begin{adjustwidth}{}{-\fullwidthlen}}{%
	\end{adjustwidth}  }
	\newcommand{\fullwbegin}{\smallskip\begin{fullwidth}}
	\newcommand{\fullwend}{\end{fullwidth}\smallskip}
---


