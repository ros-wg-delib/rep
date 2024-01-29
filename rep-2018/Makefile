images = react-sequence react-fallback sequence-memory fallback-memory parallel inverter force_success force_failure

# all png files
all: $(images:=.png)

%.png: %.pdf
	convert -density 300 $< $@

%.pdf: %.tex
	lualatex $<

clean:
	rm -f *.aux *.log *.pdf *.png *.fls *.fdb_latexmk *.synctex.gz
