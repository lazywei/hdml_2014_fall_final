SRC = kernel.tex
PDF = kernel.pdf
AUX = kernel.aux
TEXC := xelatex
TEXC_OPTS += -shell-escape

.PHONY: clean install

all: $(PDF)

$(AUX):
	$(TEXC) $(TEXC_OPTS) $(SRC)

$(PDF): $(AUX) $(SRC)
	$(TEXC) $(TEXC_OPTS) $(SRC)

clean:
	@rm -f $(PDF)
