.PHONY: all
all: OpenSecEd-paper.pdf OpenSecEd-slides.pdf

SRC=		preamble.tex
SRC+=		abstract.tex content.tex

OpenSecEd-paper.pdf: paper.pdf
paper.pdf: paper.tex ${SRC}

OpenSecEd-slides.pdf: slides.pdf
slides.pdf: slides.tex ${SRC}

OpenSecEd-paper.pdf OpenSecEd-slides.pdf:
	ln -sf $^ $@


.PHONY: clean
clean:
	${RM} OpenSecEd-paper.pdf
	${RM} OpenSecEd-slides.pdf


INCLUDE_MAKEFILES=../makefiles
include ${INCLUDE_MAKEFILES}/tex.mk
