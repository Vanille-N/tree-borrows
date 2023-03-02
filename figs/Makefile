SRC_RAW = $(wildcard *.raw)
SRC_TEX = $(wildcard *.tex)
FIGURES = $(SRC_TEX:.tex=.pdf) $(SRC_RAW:.raw=.pdf)

all: $(FIGURES)

%.pdf: %.tex
	pdflatex $<

%.tex: %.raw
	cat template.header \
		'$<' \
		template.footer \
		> '$@'
