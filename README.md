# CompareM

<b>[This project is in active development and not currently recommended for public use.]</b>

LinkM is a small wrapper around [BamM](http://minillinim.github.io/BamM/) for associating 16S reads with assembled contigs. Emphasis has been placed on linking 16S fragments with contigs binned into putative population genomes. It works as follows:

* all pairs where one or both reads derived from a 16S sequence are identified
* these <i>16S pairs</i> are mapped onto assembled contigs
* report which 16S pairs were mapped to assembled contigs
 * optionally, a set of population genomes (i.e., bins) can be provided for identifying 16S pairs associated with a specific genome

LinkM was developed as 16S sequence often fail to assemble. As a result, it is common to obtain population genomes either without a 16S sequences or with only a partial 16S sequence. The 16S pairs associated with a population genome can be used to perform a <i>de novo</i> assembly with just these pairs, or used as short fragments and parsimoniously placed in an existing 16S tree. We have also observed that in many cases the 16S pairs will link a contig within a population genome to a partially assembled 16S fragment which was too short to be properly binned.

## Install

The simplest way to install this package is through pip:
> sudo pip install linkm

LinkM relies on several other software packages:

* [BamM](http://minillinim.github.io/BamM/)
* [bwa](http://bio-bwa.sourceforge.net/)

## Cite

If you find this package useful, please cite this git repository (https://github.com/dparks1134/LinkM)

## Copyright

Copyright © 2015 Donovan Parks. See LICENSE for further details.
