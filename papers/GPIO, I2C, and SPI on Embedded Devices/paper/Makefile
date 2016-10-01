# LaTeX Makefile
TEX = pdflatex
BIB = biber
FILE = paper
DEPENDENCIES = $(FILE).tex \
	$(FILE).bib

all: $(FILE).pdf

$(FILE).pdf: $(DEPENDENCIES)
	$(TEX) -shell-escape $(FILE).tex
	$(BIB) $(FILE)
	$(TEX) -shell-escape $(FILE).tex
	$(TEX) -shell-escape $(FILE).tex

.PHONY: clean

clean:
	rm -f *.aux *.blg *.out *.toc *.bbl *.log *.abstract
