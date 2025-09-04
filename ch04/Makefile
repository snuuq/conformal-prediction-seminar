# ===== Cross-platform Makefile for LaTeX =====
LATEXMK = latexmk -pdf -interaction=nonstopmode -file-line-error

# 중간 산출물 패턴 (junk)
JUNK_FILES = *.aux *.log *.out *.toc *.lof *.lot *.fls *.fdb_latexmk *.synctex.gz \
             *.bbl *.blg *.bcf *.run.xml *-blx.bib *.nav *.snm *.vrb *.xdv *.dvi \
             *.ps *.thm *.ilg *.idx *.ind *.acn *.acr *.alg *.glg *.glo *.gls* \
             *.ist *.xdy *.auxlock *.tmp *.lox

# ===== Phony targets =====
.PHONY: all clean distclean beamer main

# ===== PDF 빌드 =====
beamer: beamer.pdf
main: main.pdf

%.pdf: %.tex
	@echo "Building $< ..."
	$(LATEXMK) $<

# 기본 메시지
all:
	@echo "Usage: make <name>  # builds <name>.tex -> <name>.pdf"

# ===== OS 판별 후 clean =====
ifeq ($(OS),Windows_NT)
# Windows
DEL_CMD = del /f /q
NULL_DEV = 2>nul
else
# Linux / Mac
DEL_CMD = rm -f
NULL_DEV =
endif

# Clean: 중간 파일만 삭제
clean:
	@echo "Cleaning intermediate files..."
	-$(LATEXMK) -c
	-$(DEL_CMD) $(JUNK_FILES) $(NULL_DEV)

# Distclean: PDF 포함 모두 삭제
distclean:
	@echo "Cleaning all generated files..."
	-$(LATEXMK) -C
	-$(DEL_CMD) $(JUNK_FILES) $(NULL_DEV)
	-$(DEL_CMD) *.pdf $(NULL_DEV)
