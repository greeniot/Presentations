# LaTeX Makefile
TEX = pdflatex
FILE = presentation
DEPENDENCIES = $(FILE).tex \
	beamerthemegreeniot.sty

all: $(FILE).pdf

$(FILE).pdf: $(DEPENDENCIES)
	$(TEX) $(FILE).tex
	$(BIB) $(FILE).aux
	$(TEX) $(FILE).tex
	$(TEX) $(FILE).tex

.PHONY: clean

clean:
	rm -f *.aux *.blg *.out *.toc *.bbl *.log *.abstract