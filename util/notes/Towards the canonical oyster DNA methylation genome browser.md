#Towards the canonical oyster DNA methylation genome browser

Seems like I have gotten close (see [here](https://github.com/sr320/qdod/wiki/Genome-Feature-Tracks#crassostrea-gigas-high-throughput-bisulfite-sequencing-male-gamete)) but do not have a canonical IGV session that has all of our DNA methylation data. The goal here is to generate (and publish on figshare so I do not lose it).

First we need to start with the genome itself - and lets have a single working directory ...

    /Users/sr320/data-genomic/tentacle/comgenbro

And mirrored at <http://owl.fish.washington.edu/halfshell/index.php?dir=2015-05-comgenbro%2F>

Metadata

FileID   |   Description  | Source  
-----------|--------------------|-------------
Crassostrea_gigas.GCA_000297895.1.26.gtf | gtf  |  [ftp](ftp://ftp.ensemblgenomes.org/pub/current/metazoa/gtf/crassostrea_gigas/)
BiGill_CpG_methylation | gill methylation 5x | [paper](https://peerj.com/articles/215)
BiGill_exon_clc_rpkm | Exon-specific gene expression values (RPKM) from RNA-seq analysis corresponding to `BiGill CpG` oyster |  [paper](https://peerj.com/articles/215)
BiGo_CpG_methylation | male gamete methylation 5x  | [paper](http://journal.frontiersin.org/Journal/10.3389/fphys.2014.00224/abstract)
M1 | male gamete methylation 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
M3 | male gamete methylation 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T1D3 | 72hpf larvae from `M1` 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T1D5 | 120hpf larvae from `M1` 5x  | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T3D3 | 72hpf larvae from `M3` 5x  | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T3D5 | 120hpf larvae from `M3` 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)


http://onsnetwork.org/halfshell/2015/02/20/differential-methylation-in-the-kitchen/

    