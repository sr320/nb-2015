#Towards the canonical oyster DNA methylation genome browser

Seems like I have gotten close (see [here](https://github.com/sr320/qdod/wiki/Genome-Feature-Tracks#crassostrea-gigas-high-throughput-bisulfite-sequencing-male-gamete)) but do not have a canonical IGV session that has all of our DNA methylation data. The goal here is to generate (and publish so I do not lose it).

All data is publicly available at 

<http://owl.fish.washington.edu/halfshell/index.php?dir=2015-05-comgenbro%2F>

Metadata

FileID   |   Description  | Links
-----------|--------------------|-------------
Crassostrea_gigas.GCA_000297895.1.26.gtf | gtf  |  [ftp](ftp://ftp.ensemblgenomes.org/pub/current/metazoa/gtf/crassostrea_gigas/)
MBD-Gill-meth | MBD enriched DNA library alignment  | [paper](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3249382/figure/F1/), [info](https://www.google.com/fusiontables/embedviz?viz=CARD&q=select+*+from+13IxnqIZ_2Xpz_HE-3YcnU_egASYz9ZlA0PYIDGLN+where+col2+%3D+'C_gigas'+and+col1+%3D+'2011-04-19+00%3A00%3A00'&tmplt=2&cpr=2)
MBD-Gill-unmeth | Unmethylated complement to  MBD-Gill-meth, alignment  |  [info](https://www.google.com/fusiontables/embedviz?viz=CARD&q=select+*+from+13IxnqIZ_2Xpz_HE-3YcnU_egASYz9ZlA0PYIDGLN+where+col2+%3D+'C_gigas'+and+col1+%3D+'2011-04-19+00%3A00%3A00'&tmplt=2&cpr=2)
BiGill_CpG_methylation | gill methylation 5x (hi output) | [paper](https://peerj.com/articles/215)
BiGill_exon_clc_rpkm | Corresponding exon-specific gene expression |  [paper](https://peerj.com/articles/215)
BiGo_CpG_methylation | male gamete methylation 5x  (hi output)  | [paper](http://journal.frontiersin.org/Journal/10.3389/fphys.2014.00224/abstract)
M1 | male gamete methylation 5x  | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
M3 | male gamete methylation 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T1D3 | 72hpf larvae from `M1` methylation 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T1D5 | 120hpf larvae from `M1` methylation 5x  | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T3D3 | 72hpf larvae from `M3`  methylation 5x  | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
T3D5 | 120hpf larvae from `M3` methylation 5x | [preprint](http://biorxiv.org/content/early/2015/03/13/012831)
2M_sig | Heat stress DMRs (array), `ind.#2` | [notebook](http://onsnetwork.org/halfshell/2015/02/20/differential-methylation-in-the-kitchen/), [draft](https://www.authorea.com/users/3858/articles/18000/_show_article)
4M_sig | Heat stress DMRs (array), `ind.#4` | [notebook](http://onsnetwork.org/halfshell/2015/02/20/differential-methylation-in-the-kitchen/), [draft](https://www.authorea.com/users/3858/articles/18000/_show_article)
6M_sig | Heat stress DMRs (array), `ind.#6` | [notebook](http://onsnetwork.org/halfshell/2015/02/20/differential-methylation-in-the-kitchen/), [draft](https://www.authorea.com/users/3858/articles/18000/_show_article)
2M.bedgraph.tdf | RNA-seq from `ind.#2` above - pretreament | [notebook](http://onsnetwork.org/halfshell/2015/02/26/heating-up-the-beds/), [draft](https://www.authorea.com/users/3858/articles/18000/_show_article)
4M.bedgraph.tdf | RNA-seq from `ind.#4` above - pretreament | [notebook](http://onsnetwork.org/halfshell/2015/02/26/heating-up-the-beds/), [draft](https://www.authorea.com/users/3858/articles/18000/_show_article)
6M.bedgraph.tdf | RNA-seq from `ind.#6` above - pretreament | [notebook](http://onsnetwork.org/halfshell/2015/02/26/heating-up-the-beds/), [draft](https://www.authorea.com/users/3858/articles/18000/_show_article)
2M-HS.bedgraph.tdf | RNA-seq from `ind.#2` above - post-heatshock | [notebook](http://onsnetwork.org/halfshell/2015/02/26/heating-up-the-beds/), [draft](https://www.authorea.com/users/3858/articles/18000/_show_article)
4M-HS.bedgraph.tdf | RNA-seq from `ind.#4` above - post-heatshock | [notebook](http://onsnetwork.org/halfshell/2015/02/26/heating-up-the-beds/), [draft](https://www.authorea.com/users/3858/articles/18000/_show_article)
6M-HS.bedgraph.tdf | RNA-seq from `ind.#6` above - post-heatshock | [notebook](http://onsnetwork.org/halfshell/2015/02/26/heating-up-the-beds/), [draft](https://www.authorea.com/users/3858/articles/18000/_show_article)
mgaveryDMRs_112212.gff | EE2 exposure DMRs (array) - three oysters | [draft](https://docs.google.com/document/d/1JaXBgDP_BECybpc4RKxhRPYqiaH9Mj2hMvo68tlt-n4/edit)

---

anyone should be able to render this in IGV with this `session file`:

http://owl.fish.washington.edu/halfshell/2015-05-comgenbro/igv_session.xml

Tracks that still need to be added are larvae exposed to pesticide then a review of all _C. gigas_ genomic datasets to make sure nothing was overlooked. 

    