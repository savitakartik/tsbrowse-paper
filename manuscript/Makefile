
all: paper.pdf

paper.pdf: paper.tex reference.bib
	pdflatex -shell-escape paper.tex
	bibtex paper
	pdflatex paper.tex
	pdflatex paper.tex
clean:
	rm -f *.pdf *.aux *.bbl *.out

