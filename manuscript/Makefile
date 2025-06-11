
all: paper.pdf supplement.pdf

paper.pdf: paper.tex reference.bib
	pdflatex -shell-escape paper.tex
	bibtex paper
	pdflatex paper.tex
	pdflatex paper.tex

supplement.pdf: supplement.tex reference.bib
	pdflatex -shell-escape supplement.tex
	bibtex supplement
	pdflatex supplement.tex
	pdflatex supplement.tex

clean:
	rm -f *.pdf *.aux *.bbl *.out

