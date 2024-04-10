# Whitepaper
This year we're producing a robot code whitepaper, this repository contains the markdown source for the whitepaper. The whitepaper is written in markdown and converted to PDF using pandoc.

The process for conversion is stolen from https://miki725.com/2019/10/15/markdown-to-pdf-ieee.html

# How to build
You'll need to have pandoc installed on your system. You can install it with `apt install pandoc` on ubuntu. Additionally, you'll need `pandoc-citeproc` and `texlive` installed.

To build the whitepaper run
```
pandoc \
    --from=markdown \
    --to=latex \
    --template=template.latex \
    --output=whitepaper.pdf \
    paper.md
```