---
layout: post
title: "Install LaTeX for thesis at Uni Münster"
description: ""
category: howto
tags: [LaTeX, Scientific work]
alias: /post/32669801602/install-latex-for-thesis-at-uni-munster
---
{% include JB/setup %}
1. Download MacTex from [here](http://ftp.join.uni-muenster.de/pub/software/CTAN/systems/mac/mactex/MacTeX.pkg) (I linked the Uni Münster Mirror directly since this is a Uni Münster specific guide)
2. Run the installer
3. Install non-free fonts that you will need for the Uni Münster template as follows:
  1. Download the installer from [here](http://www.tug.org/fonts/getnonfreefonts/install-getnonfreefonts)
  2. `cd` into the directory where you downloaded the file to (you will need to open your Terminal for this): `cd ~/Downloads`
  3. Run the installer from the terminal: `sudo texlua install-getnonfreefonts`
  4. Install all fonts (because why not): `getnonfreefonts --all`
4. Install slashbox as follows:
  1. Download it [here](http://mirror.ctan.org/macros/latex/contrib/slashbox.zip)
  2. Copy it to `/usr/local/texlive/texmf-local/tex/latex/`
5. Download the actual styles from [here](http://sourceforge.net/projects/wiwwutexstyles/)
6. Copy them to `/usr/local/texlive/texmf-local/tex/latex/`
7. Run `texhash`
8. You are all done