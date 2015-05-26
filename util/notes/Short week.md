#Stranded, sex, and arms a flailing 

Normally I would not consider a _week in review_ post, but so little progress was made (better than nothing) I thought I would give it a shot. Monday and Tuesday was in Oregon giving a seminar "[Genomics on the Half Shell: Environmental Epigenetics, Open Science, and the Oyster](https://github.com/sr320/talk-osu-2015)". (Yes, I will use that as an excuse).

On the epigenetics and ocean acidification front I think we have a way forward. In short the following will get 32% mapping.

```
!/Users/Shared/Apps/bsmap-2.74/bsmap \
-a 20150506_trimmed_2212_lane2_CTTGTA_L002_R1_001.fastq.gz \
-d /Users/Shared/data/oyster.v9_90.fa \
-o tmp-4.sam \
-n 1 \
-L 30 \
-p 8 \
 -v 5
```

A hurdle overcome in this effort included getting rid of more artifact sequence. [Sam cleaned up a file](http://onsnetwork.org/kubu4/2015/05/06/bioinformatics-trimmomaticfastqc-on-c-gigas-larvae-oa-ngs-data/) to get us some straight lines then I invoked the `-L` to get rid of the "G rise".  

---
![trim](http://eagle.fish.washington.edu/cnidarian/skitch/Bioinformatics_–_Trimmomatic_FASTQC_on_C_gigas_Larvae_OA_NGS_Data___Sam_s_Notebook_1B01001D.png)

---

The second big issue was understanding (Thanks to Mac!) that I needed to pay attention to the mapping strand information 


    -n  [0,1]   set mapping strand information. default: 0
    -n 0: only map to 2 forward strands, i.e. BSW(++) and BSC(-+), 
                   for PE sequencing, map read#1 to ++ and -+, read#2 to +- and --.  
    -n 1: map SE or PE reads to all 4 strands, i.e. ++, +-, -+, -- 


 
With that and flexing the `-v`, we can get mapping that can then be analyzed. Will wait on pulling the trigger until we hear from the NSF on going for a full proposal. In the mean time I would still like to know what is going on in those first 30 bp.
 
 
---

 While working on a chapter I came across the diversion of trying to identify the gene sequences that were analogous to the Dheilly sex specific genes.
 
 see 
 
Dheilly, Nolwenn M.; Lelong, Christophe; Huvet, Arnaud; Kellner, Kristell; Dubos, Marie-Pierre; Riviere, Guillaume; Boudry, Pierre; Favrel, Pascal (2012): Gametogenesis in the Pacific Oyster Crassostrea gigas: A Microarrays-Based Analysis Identifies Sex and Stage Specific Genes. File_S1.xls. PLOS ONE.
10.1371/journal.pone.0036353.s001. Retrieved 14:28, May 08, 2015 (GMT).


In NCBI I was able to get the details of the array platform

![geo](http://eagle.fish.washington.edu/cnidarian/skitch/GEO_Accession_viewer_1B010440.png)


This file was loaded up to the beta version of SQLShare (http://sqlshare.uw.edu/).

![array](http://eagle.fish.washington.edu/cnidarian/skitch/SQLShare_-_View_Query_1B0104C8.png)

And with a few joins...

```
SELECT * FROM [sr320@washington.edu].[Dheilly-File_S1_1]s
  left join 
  
[sr320@washington.edu].[Dheilly-array-design]array
  on 
  s.[Genbank Acc]=array.GB_ACC
  left join 
  [sr320@washington.edu].[table_Roberts_Sigenae6_transcriptome.tab]six
  on 
  array.ContigName=six.Column1​
 
   ```
   
   and a little more work I can get a fasta for Blast purposes. 
   
   see  also
   <https://github.com/sr320/chapter-mollusc-genomics/blob/master/ipynb/Dheilly-sex-specific.ipynb>
   
   Though in a little of hindsight maybe a better approach would be to use the probe sequences and see how they match up with the Ensembl version of the oyster genome.
   
   ---
   
   And to prove I did not completely _waste_ the week I am considering how to addresss our reviews for the "Up in Arms" paper. In another means to assess full transcriptome I have generated some data by comparing `Phel` to `Patiria`
   
 ![pat](http://eagle.fish.washington.edu/cnidarian/skitch/Transcriptome-Comparison_1B01067A.png).
 
 Still need to take this forward from...
 <https://github.com/sr320/eimd-sswd/blob/master/Transcriptome-Comparison.ipynb>
 
 

 
                   
                                                       
