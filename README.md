# Multiple Sequence Alignment with Suffix Tree

This project is aimed at improving a part of [HAlign2.0](https://github.com/malabz/HAlign), which could align multiple nucleotide sequences fast and accurately.

## Usage

```
java -jar halign-stmsa.jar [-h] [-o outfile] [-t thread] [-r] [-s] infile
```

```
positional argument: 
  infile   nucleotide sequences in fasta format

optional arguments: 
  -h       show this help message and exit
  -o       target file
  -t       multi-thread
  -r       realign the endings for better results
  -s       output alignments without sequence identifiers, i.e. in plain txt format but with sequence order retained
```

## Chang Log

* 15-10-2020

  add argument [-r] to re-align the beginning and ending parts of the result generated by suffix-tree msa for a better partial alignment

* 28-07-2020

  pairwise-alignment scoring rules adjusted

* 11-07-2020
  
  optimizations

* 16-12-2019

  refactoring and a new feature added

* 15-12-2019

  `SuffixTree.java` rewritten to improve the performance
 
* 20-10-2019

  initialisation

## Build

- JDK 11
- Maven
