TEX_SRC = $(wildcard *.tex)

all: main.pdf

%.pdf: %.tex $(TEX_SRC)
	latexmk $<

.PHONY: all
