
.PHONY: all
all: ../inst/bowtie2

../inst/bowtie2:
	cd bowtie2; \
	make -f Makefile; \
	cd ..; \
	echo “Make of bowtie2 DONE”
	mkdir ../inst
	mv bowtie2/bowtie2 ../inst
#	mv bowtie2/bowtie2-align ../inst
	mv bowtie2/bowtie2-build ../inst
	mv bowtie2/bowtie2-inspect ../inst
	mv bowtie2/bowtie2-build-s ../inst
	mv bowtie2/bowtie2-build-l ../inst
	mv bowtie2/bowtie2-align-s ../inst
	mv bowtie2/bowtie2-align-l ../inst
	mv bowtie2/bowtie2-inspect-s ../inst
	mv bowtie2/bowtie2-inspect-l ../inst
	echo “Copy of bowtie2 binaries DONE”

.PHONY: clean
clean:
	rm -f bowtie2/*.o
	rm -f ../inst/bowtie2 ../inst/bowtie2-build ../inst/bowtie2-inspect ../inst/
