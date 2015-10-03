#Open Data and Reproducibility with Repos

While we can certainly improve on our efforts to make our work open and reproducible, we have published a series of products over the last few years that have had associated code/data repositories that have accompanied the narratives (aka manuscripts). I will try to recap said efforts here as a means to show others different options, as well as point out ways we can improve going forward.

---

#Case 1 
>Gavery MR, Roberts SB. (2013) Predominant intragenic methylation is associated with gene expression characteristics in a bivalve mollusc. PeerJ 1:e215 <https://dx.doi.org/10.7717/peerj.215>

This was one of our early efforts where we provided the ability to view genomic feature tracks in Integrative Genomics Viewer and the SQLShare query used to derive the methylation feature track from the original methratio output.


<img src="http://eagle.fish.washington.edu/cnidarian/skitch/Predominant_intragenic_methylation_is_associated_with_gene_expression_characteristics_in_a_bivalve_mollusc__PeerJ__1BBEED09.png" alt="Predominant_intragenic_methylation_is_associated_with_gene_expression_characteristics_in_a_bivalve_mollusc__PeerJ__1BBEED09.png"/>

---

![pic](http://eagle.fish.washington.edu/cnidarian/skitch/Crassostrea_gigas_high-throughput_bisulfite_sequencing__gill_tissue__1BBEEDD3.png) <http://figshare.com/articles/Crassostrea_gigas_high_throughput_bisulfite_sequencing_gill_tissue_/749728>

We also linked out to a webpage with more instructions <http://oystergen.es/bigill>


---
#Case 2

>Garcia-Vedrenne AE, Groner M, Page-Karjian A, Siegmund G-F, Singhal S, Sziklay J and Roberts SB. (2013) Development of Genomic Resources for a thraustochytrid Pathogen and Investigation of Temperature Influences on Gene Expression PLoS ONE 8(9): e74196. [doi:10.1371/journal.pone.0074196](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0074196)

In this particular case we cited the figshare repository in the paper itself.

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/PLOS_ONE__Development_of_Genomic_Resources_for_a_thraustochytrid_Pathogen_and_Investigation_of_Temperature_Influences_on_Gene_Expression_1BBEEEB4.png" alt="PLOS_ONE__Development_of_Genomic_Resources_for_a_thraustochytrid_Pathogen_and_Investigation_of_Temperature_Influences_on_Gene_Expression_1BBEEEB4.png"/>


![qpx](http://eagle.fish.washington.edu/cnidarian/skitch/QPX_Genome_Browser_Feature_Tracks_1BBEF2DB.png) <http://figshare.com/articles/QPX_Genome_Browser_Feature_Tracks/701214>

---

#Case 3

>Olson CE and Roberts SB. (2014). Genome-wide profiling of DNA methylation and gene expression in Crassostrea gigas male gametes Frontiers in Physiology. 5:224. doi: [10.3389/fphys.2014.0022](http://journal.frontiersin.org/article/10.3389/fphys.2014.00224/abstract)

This is an edge case where figshare was used for supplemental analysis, though a tiny bit of R code is part of the repo.

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/Frontiers___Genome-wide_profiling_of_DNA_methylation_and_gene_expression_in_Crassostrea_gigas_male_gametes___Invertebrate_Physiology_1BBEF472.png" alt="Frontiers___Genome-wide_profiling_of_DNA_methylation_and_gene_expression_in_Crassostrea_gigas_male_gametes___Invertebrate_Physiology_1BBEF472.png"/>



![olson](http://eagle.fish.washington.edu/cnidarian/skitch/Crassostrea_gigas_male_gonad_transcriptome_data_comparison_1BBEF4ED.png) <http://figshare.com/articles/Crassostrea_gigas_male_gonad_transcriptional_data_comparison/1004464>



----

#Case 4

>Timmins-Schiffman E, Coffey WD, Hua W, Nunn BL, Dickinson GH and Roberts SB. (2014). Shotgun proteomics reveals physiological response to ocean acidification in Crassostrea gigas BMC Genomics 2014, 15:951 doi:[10.1186/1471-2164-15-951](http://www.biomedcentral.com/1471-2164/15/951)

With this paper we added data to a PANAGAEA for the first time per request. The citations to figshare doubled here (2), where one is a simply a PDF that (in theory) could be used to reproduce the proteomics data results in SQLShare. This is complex as it is a combination of links and SQL commands. A unique problem here is that SQLShare is moving servers, so this breaks. The second figshare citation is the full size pathway analalysis figures that allow people to interact with the data better. This paper is prime for some form of interactiveness.

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/BMC_Genomics___Full_text___Shotgun_proteomics_reveals_physiological_response_to_ocean_acidification_in_Crassostrea_gigas_1BBEF69E.png" alt="BMC_Genomics___Full_text___Shotgun_proteomics_reveals_physiological_response_to_ocean_acidification_in_Crassostrea_gigas_1BBEF69E.png"/>

![pan](http://eagle.fish.washington.edu/cnidarian/skitch/Timmins-Schiffman__E_et_al___2014___Shotgun_proteomics_reveals_physiological_response_to_ocean_acidification_in_Crassostrea_gigas_1BBEF6C2.png) <http://doi.pangaea.de/10.1594/PANGAEA.837671>



<img src="http://eagle.fish.washington.edu/cnidarian/skitch/BMC_Genomics___Full_text___Shotgun_proteomics_reveals_physiological_response_to_ocean_acidification_in_Crassostrea_gigas_1BBEF5D2.png" alt="BMC_Genomics___Full_text___Shotgun_proteomics_reveals_physiological_response_to_ocean_acidification_in_Crassostrea_gigas_1BBEF5D2.png"/>



<img src="http://eagle.fish.washington.edu/cnidarian/skitch/SQLShare_workflow_for_proteomics_analysis_1BBEF64E.png" alt="SQLShare_workflow_for_proteomics_analysis_1BBEF64E.png"/>
<http://figshare.com/articles/SQLShare_workflow_for_proteomics_analysis/894323>

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/iPath2_supplemental_information_1BBEF672.png" alt="iPath2_supplemental_information_1BBEF672.png"/>
<http://figshare.com/articles/iPath2_supplemental_information/899908>

---

#Case 5

>Fuess LE, Eisenlord ME, Closek CJ, Tracy AM, Mauntz R, Gignoux-Wolfsohn S, Moritsch MM, Yoshioka R, Burge CA, Harvell CD, Friedman CS, Hewson I, Hershberger PK, Roberts SB (2015) Up in Arms: Immune and Nervous System Response To Sea Star Wasting Disease PLoS ONE doi:[10.1371/journal.pone.0133053](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0133053)

Here is where things start getting a little better...

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/PLOS_ONE__Up_in_Arms__Immune_and_Nervous_System_Response_to_Sea_Star_Wasting_Disease_1BBEF736.png" alt="PLOS_ONE__Up_in_Arms__Immune_and_Nervous_System_Response_to_Sea_Star_Wasting_Disease_1BBEF736.png"/>

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/PLOS_ONE__Up_in_Arms__Immune_and_Nervous_System_Response_to_Sea_Star_Wasting_Disease_1BBEF78F.png" alt="PLOS_ONE__Up_in_Arms__Immune_and_Nervous_System_Response_to_Sea_Star_Wasting_Disease_1BBEF78F.png"/>

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/eimd-sswd_v1_0__Supplemental_Jupyter_notebooks_and_data_1BBEF7FB.png" alt="eimd-sswd_v1_0__Supplemental_Jupyter_notebooks_and_data_1BBEF7FB.png"/>
<http://figshare.com/articles/eimd_sswd_v1_0_Supplemental_Jupyter_notebooks_and_data/1441384>


<img src="http://eagle.fish.washington.edu/cnidarian/skitch/sr320_eimd-sswd_1BBEF81A.png" alt="sr320_eimd-sswd_1BBEF81A.png"/>
<https://github.com/sr320/eimd-sswd>


---

#Case 6

>Heare JE, Blake B, Davis JP, Vadopalas B, Roberts SB. (2014) Evidence of Ostrea lurida (Carpenter 1894) population structure in Puget Sound, WA. PeerJ PrePrints 2:e704v1 <http://dx.doi.org/10.7287/peerj.preprints.704>

Now we are into "preprints" (and we will continue to be into them). For this particular paper, data was analyzed with R, using a GitHub repo, and doi'd with Zenodo.

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/Evidence_of_Ostrea_lurida__Carpenter_1864__population_structure_in_Puget_Sound__WA__PeerJ_PrePrints__1BC01888.png" alt="Evidence_of_Ostrea_lurida__Carpenter_1864__population_structure_in_Puget_Sound__WA__PeerJ_PrePrints__1BC01888.png"/>


<img src="http://eagle.fish.washington.edu/cnidarian/skitch/OluridaSurvey2014__JSR_-_Zenodo_1BC01903.png" alt="OluridaSurvey2014__JSR_-_Zenodo_1BC01903.png"/>
<https://zenodo.org/record/30373>

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/jheare_OluridaSurvey2014_1BC01964.png" alt="jheare_OluridaSurvey2014_1BC01964.png"/> <https://github.com/jheare/OluridaSurvey2014>

This link with Zenodo is nice. Every time you create another release, Zenodo automatically updates. 


---

#Case 7

>Claire E. Olson, Steven B. Roberts. Indication of family-specific DNA methylation patterns in developing oysters bioRxiv doi: <http://dx.doi.org/10.1101/012831>

Another preprint, this time on bioRxiv. This is probably our most *reproducible* work. It is done in a Jupyter notebook (fomerly IPython). In the paper the Github is directly cited.


<img src="http://eagle.fish.washington.edu/cnidarian/skitch/biorxiv_org_content_biorxiv_early_2015_03_13_012831_full_pdf_1BC01AE5.png" alt="biorxiv_org_content_biorxiv_early_2015_03_13_012831_full_pdf_1BC01AE5.png"/>

<img src="http://eagle.fish.washington.edu/cnidarian/skitch/che625_olson-ms-nb_1BC01A88.png" alt="che625_olson-ms-nb_1BC01A88.png"/> <https://github.com/che625/olson-ms-nb>




---

#Case 8

>Steven Roberts. (2015). paper-Oyster-EE2: v1.5. Zenodo. 10.5281/zenodo.19046 Influence of 17α-ethinylestradiol on DNA Methylation in Oysters


---

#Case 9
