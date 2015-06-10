#Towards the canonical oyster DNA methylation genome browser

Seems like I have gotten close (see [here](https://github.com/sr320/qdod/wiki/Genome-Feature-Tracks#crassostrea-gigas-high-throughput-bisulfite-sequencing-male-gamete)) but do not have a canonical IGV session that has all of our DNA methylation data. The goal here is to generate (and publish so I do not lose it).

First we need to start with the genome itself - and lets have a single working directory ...

    /Users/sr320/data-genomic/tentacle/comgenbro

And mirrored publicly at <http://owl.fish.washington.edu/halfshell/index.php?dir=2015-05-comgenbro%2F>

Metadata

FileID   |   Description  | Source  
-----------|--------------------|-------------
Crassostrea_gigas.GCA_000297895.1.26.gtf | gtf  |  [ftp](ftp://ftp.ensemblgenomes.org/pub/current/metazoa/gtf/crassostrea_gigas/)
MBD-Gill-meth | MBD enriched DNA library  | [paper](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3249382/figure/F1/), [info](https://www.google.com/fusiontables/embedviz?viz=CARD&q=select+*+from+13IxnqIZ_2Xpz_HE-3YcnU_egASYz9ZlA0PYIDGLN+where+col2+%3D+'C_gigas'+and+col1+%3D+'2011-04-19+00%3A00%3A00'&tmplt=2&cpr=2)
MBD-Gill-unmeth | Unmethylated complement to  MBD-Gill-meth  |  [info](https://www.google.com/fusiontables/embedviz?viz=CARD&q=select+*+from+13IxnqIZ_2Xpz_HE-3YcnU_egASYz9ZlA0PYIDGLN+where+col2+%3D+'C_gigas'+and+col1+%3D+'2011-04-19+00%3A00%3A00'&tmplt=2&cpr=2)
BiGill_CpG_methylation | gill methylation 5x | [paper](https://peerj.com/articles/215)
BiGill_exon_clc_rpkm | Corresponding exon-specific gene expression |  [paper](https://peerj.com/articles/215)
BiGo_CpG_methylation | male gamete methylation 5x  | [paper](http://journal.frontiersin.org/Journal/10.3389/fphys.2014.00224/abstract)
M1 | male gamete methylation 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
M3 | male gamete methylation 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T1D3 | 72hpf larvae from `M1` 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T1D5 | 120hpf larvae from `M1` 5x  | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T3D3 | 72hpf larvae from `M3` 5x  | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T3D5 | 120hpf larvae from `M3` 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
&probes& | probe location on xxx array | file location (canonical)


http://onsnetwork.org/halfshell/2015/02/20/differential-methylation-in-the-kitchen/

    