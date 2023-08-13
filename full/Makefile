TEX_SRC = $(wildcard *.tex)

all: main.pdf

%.pdf: %.tex $(TEX_SRC) rustlistings.sty coqlistings.sty Makefile
	pdflatex --interaction=nonstopmode --halt-on-error $<
	bibtex main.aux
	pdflatex --interaction=nonstopmode --halt-on-error $<
	pdflatex --interaction=nonstopmode --halt-on-error $<

.PHONY: all
