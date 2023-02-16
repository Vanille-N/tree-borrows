SOURCES = $(wildcard *.tex)
FIGURES = $(SOURCES:.tex=.pdf)

all: $(FIGURES)

%.pdf: %.tex
	pdflatex $<
