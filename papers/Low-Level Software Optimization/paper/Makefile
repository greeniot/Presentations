# LaTeX Makefile
TEX = pdflatex
FILE = paper
DEPENDENCIES = $(FILE).tex

all: $(FILE).pdf

$(FILE).pdf: $(DEPENDENCIES)
	$(TEX) $(FILE).tex
	$(TEX) $(FILE).tex

.PHONY: clean

clean:
	rm -f *.aux *.blg *.out *.toc *.bbl *.log *.abstract