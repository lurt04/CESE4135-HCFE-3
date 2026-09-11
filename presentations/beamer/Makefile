MAIN = presentation

.PHONY: all clean $(MAIN).pdf

all: $(MAIN).pdf

$(MAIN).pdf:
	pdflatex -interaction=nonstopmode $(MAIN).tex
	bibtex $(MAIN)
	pdflatex -interaction=nonstopmode $(MAIN).tex
	pdflatex -interaction=nonstopmode $(MAIN).tex

clean:
	rm -f $(MAIN).aux $(MAIN).bbl $(MAIN).blg $(MAIN).log $(MAIN).nav \
	      $(MAIN).out $(MAIN).snm $(MAIN).toc $(MAIN).run.xml \
	      $(MAIN)-blx.bib $(MAIN).fls $(MAIN).fdb_latexmk
