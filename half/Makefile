TEX_SRC = $(wildcard *.tex)

all: main.pdf

%.pdf: %.tex $(TEX_SRC) rustlistings.sty
	pdflatex --interaction=nonstopmode --halt-on-error $<
	pdflatex --interaction=nonstopmode --halt-on-error $<

.PHONY: all
