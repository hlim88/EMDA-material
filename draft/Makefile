FILE=emda

all: $(FILE).pdf

view: $(FILE).pdf display

.PHONY: clean

clean:
	rm -rf *~ *.idx *.lot *.toc *.lof *.aux *.blg *.out *.bbl *.log *.pdf

display:
	open $(FILE).pdf

$(FILE).pdf: $(FILE).tex
	pdflatex $(FILE)
	pdflatex $(FILE)
	bibtex $(FILE)
	pdflatex $(FILE)
	pdflatex $(FILE)
