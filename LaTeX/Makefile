PROJECT=main
TEX=pdflatex
BIBTEX=bibtex
MKINDEX=makeindex
MKGLOSSARY=makeglossaries
BUILDTEX=$(TEX) $(PROJECT).tex

all:
	$(BUILDTEX)
	$(BIBTEX) $(PROJECT)
	$(MKINDEX) $(PROJECT)
	$(MKGLOSSARY) $(PROJECT)
	$(BUILDTEX)
	$(BUILDTEX)

index:
	$(MKINDEX) $(PROJECT)

glossaire:
	$(MKGLOSSARY) $(PROJECT)

bib:
	$(BIBTEX) $(PROJECT)

pdf:
	 $(BUILDTEX)

clean-all:
	rm -f *.dvi *.log *.bak *.aux *.bbl *.blg *.idx *.ps *.eps *.pdf *.toc *.out *~

clean:
	rm -f *.log *.bak *.aux *.bbl *.blg *.idx *.toc *.out *~
