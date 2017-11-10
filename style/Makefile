.DEFAULT_GOAL := pp

pp: $(PDF) 
$(PDF): $(MD)
	pp -pdf -import=style/pp-macros/all.pp source/*.md | pandoc -s -o $@ $(TEXTEMPLATE) --include-in-header=style/style.tex $(TEXFLAGS) 2>output/pdf.log
	if [[ "$OSTYPE" == "darwin" ]]; then open $@; else xdg-open $@;fi

