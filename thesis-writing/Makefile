DEPS =  \
                ref.bib \
                intro.tex \
                algo1.tex \
                conclusion.tex \
                myversion.tex \
                proposed.tex \
                litrev.tex \
                prelim.tex \
                methodeval.tex

myversion.pdf : $(DEPS)
	pdflatex myversion
	bibtex myversion
	pdflatex myversion
	pdflatex myversion


myversion.zip : ReadMe.txt Makefile $(DEPS)
	zip myversion.zip ReadMe.txt Makefile $(DEPS)


clean:
	rm -fr myversion.snm myversion.aux myversion.bbl myversion.nav myversion.ind myversion.log myversion.out myversion.toc myversion.ent myversion.pdf myversion.blg
