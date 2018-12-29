# Dossiers
CODE := $(shell pwd)



all: img poly proper

# Générations des images
FIGSRC = $(wildcard sources/*.ipe )

FIGOBJ = $(FIGSRC:.ipe=.pdf)

img: $(FIGOBJ)

sources/%.pdf: sources/%.ipe
	ipetoipe -pdf $<


# Cinquième

comp:
	pdflatex relaxation-2017-2018.tex
	pdflatex relaxation-2017-2018.tex


# nettoyage			
proper:
	rm -f *.log *.toc *.aux *.nav *.snm *.out *.bbl *.blg *.dvi
	rm -f *.backup *~
