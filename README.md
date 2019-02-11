# STL5 Phylogenetics

## Intro

Phylogenetic tree construction of STL5 for HI Nat Micro Viral Complementation.

## Software Utilized
* [ClustalX-2.1](http://www.clustal.org/)
* [RAxML-8.2.12](https://cme.h-its.org/exelixis/web/software/raxml/index.html)

## Multiple Sequence Alignment

Retrieved the following ORF2 sequences from [GenBank](https://www.ncbi.nlm.nih.gov/genbank/):
* strain Y - ASB51409.1
* TF18 - AFB18034.1
* STL4 - AFT63044.1
* STL3 - AFT63043.1
* BSRI1 - AGL34956.1
* STL1 - AFT63039.1
* STL2 - AFT63042.1
* MAV1 - AWB15474.1
* MAV2 - AWB14570.1
* PAstV2 - ADP21511.1

2. Aligned sequences with ClustalX using default parameters.

## ML Tree Construction

`raxmlHPC-PTHREADS-AVX2 
-f a 
-m PROTGAMMABLOSUM62 
-p 8937 
-x 2819 
N 1000 
-s AstV_sequences.fasta 
-n AstVMLTree 
-o PAstV2_ADP21511.1 
-T 20`
