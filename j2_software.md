---
layout: page
title: Software
permalink: /software/
---

Most of my software can be found at my [github page](https://github.com/nicolaprezza). Below you can find  a list of my main projects.

<br>

----
### ebwt2snp ###

[ebwt2snp](https://github.com/nicolaprezza/ebwt2snp-v2) is a tool implementing a novel algorithm for finding SNPs/INDELs in a set of reads by processing just the Burrows-Wheeler transform (BWT) of the input. The tool is based on the observations that, in the BWT, SNPs and INDELs are clustered since they share the same context. The tool also implements a novel succinct suffix-array navigation algorithm. Publications:

- Nicola Prezza, Nadia Pisanti, Marinella Sciortino, and Giovanna Rosone, 2019. **SNPs detection by eBWT positional clustering**. Algorithms for Molecular Biology, 14(1), p.3.

- Nicola Prezza, Nadia Pisanti, Marinella Sciortino, and Giovanna Rosone, 2018. **Detecting mutations by eBWT**. In 18th International Workshop on Algorithms in Bioinformatics, (WABI 2018). Vol. 113, pp. 1-15. Schloss Dagstuhl-Leibniz-Zentrum fur Informatik GmbH, Dagstuhl Publishing.

- Nicola Prezza and Giovanna Rosone, 2019. **Space-Efficient Computation of the LCP Array from the Burrows-Wheeler Transform**. arXiv preprint arXiv:1901.05226

----
### r-index ###

The [r-index](https://github.com/nicolaprezza/r-index) is the first full-text index of size O(r), r being the number of BWT runs of the input text (of size n), supporting near-optimal locate of pattern occurrences. The r-index employs a novel suffix array sampling of size 2r; in classical FM-indexes, this sampling would result in a locate time of Omega(n/r) per occurrence. The r-index, on the other hand, reduces this time to O(log(n/r)).

----
### DYNAMIC ###

[DYNAMIC](https://github.com/xxsds/DYNAMIC) is a C++ library offering space- and time-efficient implementations of some basic succinct/compressed dynamic data structures such as succinct dynamic partial sums, bitvectors, strings. 

----
### ERNE 2 ###

This tool, developed in collaboration with the university of Udine and the [Institute of Applied Genomics](http://www.appliedgenomics.org/en/), includes: 

- A DNA short-reads aligner.
- A bisulfite-treated short-reads aligner for methylation analysis.
- A read filtering tool.
- A methylation calling tool.

ERNE is based on a novel succinct hash data structure combining the concepts of Burrows-Wheeler transform and Hamming-Aware hash functions. 
