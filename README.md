# Epal2nal.pl
pal2nal.pl  (v13)

Usage:  pal2nal.pl  pep.aln  nuc.fasta  [nuc.fasta...]  [options]


    pep.aln:    protein alignment either in CLUSTAL or FASTA format

    nuc.fasta:  DNA sequences (single multi-fasta or separated files)

    Options:  -h            Show help 

              -output (clustal|paml|fasta|codon)
                            Output format; default = clustal

              -blockonly    Show only user specified blocks
                            '#' under CLUSTAL alignment (see example)

              -nogap        remove columns with gaps and inframe stop codons

              -nomismatch   remove mismatched codons (mismatch between
                            pep and cDNA) from the output

              -codontable (universal|vmitochondria|chl)
                            Codon table
                              - universal (default)
                              - vmitochondria -> vertebrate mitochondrial
			      - chl -> chloroplast

              -html         HTML output (only for the web server)

              -nostderr     No STDERR messages (only for the web server)


    - sequence order in pep.aln and nuc.fasta should be the same.

    - IDs in pep.aln are used in the output.
