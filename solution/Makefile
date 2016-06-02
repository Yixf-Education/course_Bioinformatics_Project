PDFC = xelatex
BIBC = bibtex
READER = evince

TARGET = experiment.pdf
OUTGROWTH = *.out *.log *.aux *.toc *.lof *.lot *.lol *.bbl *.blg
SOURCE = experiment.tex
BSOURCE = experiment

$(TARGET): $(SOURCE)
	$(PDFC)	$(SOURCE)
	$(BIBC)	$(BSOURCE)
	$(PDFC)	$(SOURCE)
	$(PDFC)	$(SOURCE)

read:
	$(READER) $(TARGET)

clean:
	-rm $(OUTGROWTH)

cleanall:
	-rm $(OUTGROWTH) $(TARGET)

.PHONY:read clean cleanall
