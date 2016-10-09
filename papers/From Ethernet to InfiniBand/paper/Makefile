# LaTeX Makefile
TEX = pdflatex
BIB = bibtex
FILE = paper
DEPENDENCIES = $(FILE).tex \
	$(FILE).bib

all: $(FILE).pdf

$(FILE).pdf: $(DEPENDENCIES)
	$(TEX) $(FILE).tex
	$(BIB) $(FILE).aux
	$(TEX) $(FILE).tex
	$(TEX) $(FILE).tex

.PHONY: clean

clean:
	rm -f *.aux *.blg *.out *.toc *.bbl *.log *.abstract