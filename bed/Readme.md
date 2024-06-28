# BED - Browser Extensible Data

Bed is a format to denote chromosomal regions which has a [formal specification](https://github.com/samtools/hts-specs/blob/master/BEDv1.pdf) since 2021. Here is an example of a benign bed file with four columns:

    chr1    0  100  region1
    chr1  100  200  region2

There is a lot that can go wrong here. The coordinates might be invalid, the line endings may differ, some implementations may expect sorted fields or require tabs as separators.

This directory contains the following files:

* emptyfile.bed: it's empty Jim
* coords.bed: a file with various invalid coordinates
* eof.bed: according to the spec a line has to end with with a newline. In extension this file is empty.
