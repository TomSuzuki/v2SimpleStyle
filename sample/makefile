SHELL   = /bin/sh

RM = cmd.exe /C del	# for windows
# RM = rm -f	# for Linux

FILE   = sample# 引数から読み込ませる？
TEX     = $(FILE).tex
XDV     = $(FILE).xdv

all:
	make tex

tex:
	xelatex -no-pdf $(TEX)
	pbibtex $(FILE)
	xelatex -no-pdf $(TEX)
	xelatex -no-pdf $(TEX)
	xelatex -no-pdf $(TEX)
	xdvipdfmx.exe $(XDV)
	make clean

clean:
	-$(RM) *.aux *.dvi *.idx *.ilg *.ind *.log *.nav *.out *.snm *.xdv *.toc *~ *.bbl *.blg *.vrb
