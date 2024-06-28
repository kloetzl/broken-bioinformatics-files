# FASTA

FastA is the simplest file format that deserves the name, however already a lot of things can go wrong. Consider the following benign example.

    >SequenceName comment more stuff
    ACGTAACCCCGGTACGATCGGGATCTTTGACTGATCAAAAATAATTAAGCGTTAN
    GATCAAAAATAATTAAGCGTTANACGTAACCCCGGTACGATCGGGATCTTTGACT

Historically sequences were short and thus fasta files included a line break every 70 chars so they would be easier to read on a terminal. However, that makes parsing a file correctly (and quickly) difficult.

This directory includes the following invalid files:

* emptyfile.fa: an empty file
* emptysequence.fa: one sequence doesn't contain any characters
* emptysequence2.fa: same but followed by another sequence
* eofincomment.fa: the file ends in a comment
* eofincomment2.fa: same
* eofincomment3.fa: the file ends after a whitespace
* eofinname.fa: the file ends in the sequence name
* snpgenie.fa: empty sequence name
* spaceinseq.fa: the sequence shouldn't contain whitespace
