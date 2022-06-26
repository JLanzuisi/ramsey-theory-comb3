FILE = main

all: render addheader

render: $(FILE).rmd
	render.R $(FILE).rmd

addheader: $(FILE).tex
	sed -i '1i % % % % % % % % % % % % % % % % % % % % % % % % % % % % % %' $(FILE).tex
	sed -i '2i % This TeX file is auto-generated from an rmarkdown source.' $(FILE).tex
	sed -i '3i % % % % % % % % % % % % % % % % % % % % % % % % % % % % % %' $(FILE).tex
	sed -i '4i %' $(FILE).tex
