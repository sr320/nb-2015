Wayback to just-MBD

Prior to bisulfite sequencing we did do a couple if MBD enrichment libraries to describe DNA methylation in oysters. Results even were snuck into [this perspective](http://journal.frontiersin.org/article/10.3389/fphys.2011.00116/abstract).

![mbd](http://www.frontiersin.org/files/Articles/19155/fphys-02-00116-HTML/image_m/fphys-02-00116-g001.jpg)

While I am sure there are genome tracks around, I am ending up #doingitagain.

In short I took the raw Solid reads, align to `Crassostrea_gigas.GCA_000297895.1.26.dna.genome` in CLC, exported bam, converted to bedgraph, converted to tdf.  

---

In long:
The raw files
![raw](http://eagle.fish.washington.edu/cnidarian/skitch/Nightingales_-_Google_Fusion_Tables_1B2B4B37.png)

1) Imported into CLC v8.0.1

```
          Discard read names = Yes
          Discard quality scores = No
          Original resource = /Users/sr320/data-genomic/tentacle/solid0078_20110412_FRAG_BC_WHITE_WHITE_F3_SB_METH/solid0078_20110412_FRAG_BC_WHITE_WHITE_F3_QV_SB_MOTH.qual
          Original resource = /Users/sr320/data-genomic/tentacle/solid0078_20110412_FRAG_BC_WHITE_WHITE_F3_SB_METH/solid0078_20110412_FRAG_BC_WHITE_WHITE_F3_SB_MOTH.csfasta
```

(yes the core called them MOTH)

2) Reads were mapped

![mapped](http://eagle.fish.washington.edu/cnidarian/skitch/CLC_Genomics_Workbench_8_0_1_-_Evaluation_1B2B4C2A.png)

3) Exported as BAM.

4) Converted to bedgraph

```
!/Applications/bioinfo/bedtools2/bin/genomeCoverageBed \
-bg \
-ibam /Users/sr320/data-genomic/tentacle/solid0078_moth.bam \
-g /Volumes/web/halfshell/qdod3/Cg.GCA_000297895.1.25.dna_sm.toplevel.genome \
> /Users/sr320/data-genomic/tentacle/MBD-meth.bedgraph          
```

5) Converted to toTDF

![tdf](http://eagle.fish.washington.edu/cnidarian/skitch/Screenshot_6_12_15__10_22_AM_1B2B4CF5.png)
     
          
---

Rinse and repeat with unmethylated fraction (UNMOTH) and import tdf into IGV!