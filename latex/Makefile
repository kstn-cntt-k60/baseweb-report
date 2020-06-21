.PHONY: all

all: thesis.pdf

thesis.pdf: thesis.bbl 	\
			icthesis.sty \
			thesis.tex 	\
			abstract.tex \
			acknowledgements.tex \
			chapters/introduction.tex \
			chapters/technology.tex \
			chapters/design.tex
	pdflatex thesis.tex

thesis.bbl: thesis.bib 
	pdflatex thesis.tex
	bibtex thesis
	pdflatex thesis.tex
