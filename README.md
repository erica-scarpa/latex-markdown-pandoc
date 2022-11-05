# LaTeX, markdwon, pandoc

Some LaTeX templates

## LaTeX templates for bibliographies

<center><img src="/img/bibliography.png" alt="drawing"/></center>
<center><img src="/img/annotated-bibliography.png" alt="drawing"/></center>

A simple file which can be used to generate a single bibliography file through `\nocite{*}`. The `.bib` file must be in the same folder as the `.tex`: replace `test-bib` in the `\bibliography{test-bib}` string with the filename of your bibliography. You must run XeLaTeX.

## markdown pandoc

`pandoc -s test.md --bibliography=bibliography.bib --csl=your-citation-stylesheet.csl --citeproc --pdf-engine=xelatex -o test.pdf`

Citation styles sheets are available on the [CSL GitHub repository](https://github.com/citation-style-language/styles) and must be included in the same folder. 