#Short week, little progress

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

```
-n  [0,1]   set mapping strand information. default: 0
                   -n 0: only map to 2 forward strands, i.e. BSW(++) and BSC(-+), 
                   for PE sequencing, map read#1 to ++ and -+, read#2 to +- and --.
                   
                   -n 1: map SE or PE reads to all 4 strands, i.e. ++, +-, -+, -- 
 ```
 
 With that and flexing the `-v`, we can get mapping that can then be analyzed. Will wait on pulling the trigger until we hear from the NSF on going for a full proposal. In the mean time I would still like to know what is going on in those first 30 bp.
 
---

 
 
 
 
                   
                                                       
