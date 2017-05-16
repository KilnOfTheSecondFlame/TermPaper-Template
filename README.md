# Description
A LaTeX project template for term papers.

# Introduction
Over the course of the last year, I was finding myself using LaTeX more and more collaboratively. Preparing the whole shebang always took the longest time. Forking this repo should give you a base file that compiles.

# Travis CI
As sprinkles I added a Travis configuration file, for commit testing. Due to the fact we have to download the whole texlive, the build usually takes about 15min. I played around with caching, but did not manage to skip the download and install step. Mind the fact, I'm no Travis power user at all. If you have some suggestion, just shoot it my way.

# Building
Due to the fact that I specified Biber as the backend for BibLaTeX compiling the .tex file takes more steps. 
In TexStudio just define a "User Command" in 'Configure TeXstudio'>Build and Copy&Paste this string: txs:///pdflatex | txs:///biber | txs:///pdflatex