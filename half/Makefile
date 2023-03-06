TEX_SRC = $(wildcard *.tex)

all: main.pdf

%.pdf: %.tex $(TEX_SRC)
	pdflatex --interaction=nonstopmode --halt-on-error $<

.PHONY: all
