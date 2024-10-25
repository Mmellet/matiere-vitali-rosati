serve:
	ls * | entr make fab
       
fab:
	pandoc texte.md --top-level-division=part --citeproc --csl=theses-de-sorbonne-universite.csl -o texte.tex |  make pdf

pdf:
	lualatex --shell-escape -interaction nonstopmode livre.tex
	lualatex --shell-escape -interaction nonstopmode livre.tex

