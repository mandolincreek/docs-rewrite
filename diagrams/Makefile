ARCH_SRC = \
	   arch \
	   arch-audio \
	   arch-voice \
	   arch-skills \
	   arch-enclosure \

ARCH_PNG = $(addsuffix .png,$(ARCH_SRC))

PDF = arch.pdf

all: $(PDF)

arch.pdf: $(ARCH_PNG)
	convert $^ $@

%.png: %.dot
	dot -Tpng <"$<" >"$@"
