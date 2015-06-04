SRC = example-1.tex
PDF = example-1.pdf
AUX = example-1.aux
TEXC := xelatex
TEXC_OPTS += -shell-escape

.PHONY: clean

all: $(PDF)

$(AUX):
	$(TEXC) $(TEXC_OPTS) $(SRC)

$(PDF): $(AUX) $(SRC)
	$(TEXC) $(TEXC_OPTS) $(SRC)

clean:
	@rm -f $(PDF)

