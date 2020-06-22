.PHONY: all

all: thesis.pdf

thesis.pdf: thesis.bbl 	\
			icthesis.sty \
			thesis.tex 	\
			abstract.tex \
			acknowledgements.tex \
			chapters/introduction.tex \
			chapters/technology.tex \
			chapters/technology/front-end.tex \
			chapters/technology/redis.tex \
			chapters/technology/postgres.tex \
			chapters/technology/back-end.tex \
			chapters/technology/docker.tex \
			chapters/technology/kubernetes.tex \
			chapters/technology/azure.tex \
			chapters/design.tex \
			chapters/solution.tex \
			chapters/conclusion.tex
	pdflatex thesis.tex

thesis.bbl: thesis.bib 
	pdflatex thesis.tex
	bibtex thesis
	pdflatex thesis.tex
