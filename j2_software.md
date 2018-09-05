---
layout: page
title: Software
permalink: /software/
---

Most of my software can be found at my [github page](https://github.com/nicolaprezza). Below you can find  a list of my main projects.

<br>

### eBWTclust: positional clustering of the Burrows-Wheeler Transform ###
----

[eBWTclust](https://github.com/nicolaprezza/eBWTclust) finds clusters corresponding to the same genome position in the eBWT of a set of DNA reads of two individuals and, by analyzing these clusters, it finds SNPs between the two individuals (reference-free, alignment-free).

The paper describing the theory behind the tool (eBWT positional clustering) can be found here: https://arxiv.org/abs/1805.01876


### The run-length Compressed Burrows-Wheeler transform index (r-index) ###
----
The [r-index](https://github.com/nicolaprezza/r-index) is the first full-text index of size O(r), r being the number of BWT runs of the input text (of size n), supporting near-optimal locate of pattern occurrences. The r-index employs a novel suffix array sampling of size 2r; in classical FM-indexes, this sampling would result in a locate time of Omega(n/r) per occurrence. The r-index, on the other hand, reduces this time to O(log(n/r)).

### DYNAMIC: Dynamic succinct and compressed data structures ###
----
[DYNAMIC](https://github.com/xxsds/DYNAMIC) is a C++ library offering space- and time-efficient implementations of some basic succinct/compressed dynamic data structures such as succinct dynamic partial sums, bitvectors, strings. 

### ERNE: The Extended Randomized Numerical alignEr ###
----
This tool, developed in collaboration with the university of Udine and the [Institute of Applied Genomics](http://www.appliedgenomics.org/en/), includes: 

- A DNA short-reads aligner.
- A bisulfite-treated short-reads aligner for methylation analysis.
- A read filtering tool.
- A methylation calling tool.

ERNE is based on a novel succinct hash data structure combining the concepts of Burrows-Wheeler transform and Hamming-Aware hash functions. 
