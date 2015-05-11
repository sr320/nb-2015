Primers 

A quick tutorial to check out primers on NCBI to see what the product size should be and how specific they are. 

```
Resource: Patil et al. 2005 Primer Name- CCGS4F  Primer Sequence- TATTCGTTGGAGACTTTATAACCCT  Resource: Patil et al. 2005
Primer Name- CCGS4R     Primer Sequence- AAGGCTTAGAATTGCAAGGTCTATA Resource: Patil et al. 2005

Primer Name- TPHI16S-1F    Primer Sequence- CTGAGTTTTTAATTGAAGTT TAGTTGGG Resource: Quinteiro et al. 2011
Primer Name- TPHI16S-2R    Primer Sequence- CCCTGCGGTAGC TTTTGCT Resource: Quinteiro et al. 2011
```

Old school way is just take the primer with NNNs in the middle and blast.
`TATTCGTTGGAGACTTTATAACCCTNNNNNNNNNNNNNNNNNNNNNAAGGCTTAGAATTGCAAGGTCTATA`


![submit](http://eagle.fish.washington.edu/cnidarian/skitch/Nucleotide_BLAST__Search_nucleotide_databases_using_a_nucleotide_query_1AF3CA29.png)

You will get an output as such....


![bl1](http://eagle.fish.washington.edu/cnidarian/skitch/Banners_and_Alerts_and_NCBI_Blast_Nucleotide_Sequence__71_letters__1AF3C831.png)

Scroll down to the alignments....

![bl2](http://eagle.fish.washington.edu/cnidarian/skitch/Banners_and_Alerts_and_NCBI_Blast_Nucleotide_Sequence__71_letters__1AF3C856.png)

And look at the coordinates....

![align](http://eagle.fish.washington.edu/cnidarian/skitch/Banners_and_Alerts_and_NCBI_Blast_Nucleotide_Sequence__71_letters__1AF3C8E3.png)

So the primers lay down between bp 400 and 61 on the given sequence, thus `400-61=339` and the band size should be about 339 bp.

---

You could also just use the Primer-Blast feature.

![pb](http://eagle.fish.washington.edu/cnidarian/skitch/Banners_and_Alerts_and_Primer_designing_tool_1AF3C89B.png)



![pb2](http://eagle.fish.washington.edu/cnidarian/skitch/Banners_and_Alerts_and_Primer-Blast_results_1AF3C96A.png)

**Bonus!** It does the math for you!