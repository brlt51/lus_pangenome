This readme file was generated on 2025-06-10 by Esme Padgett

GENERAL INFORMATION  
Title of Dataset: Lus_pangenome_draft

Author  
Name: Esme Padgett  
Institution: Durham University  
Address: Durham DH1 3LE  
Email: esme.padgett@durham.ac.uk  

Author  
Name: Adrian Brennan  
ORCID: https://orcid.org/0000-0002-8171-769X  
Institution: Durham University  
Address: Durham DH1 3LE  
Email: a.c.brennan@durham.ac.uk  

Date of genome asm data collection: 2024-11-21 from NCBI PRNJ databases (https://www.ncbi.nlm.nih.gov/datasets/genome/)  

Data derived from other sources:  
    You FM, Xiao J, Li P, Yao Z, Jia G, He L, et al. Chromosome‐scale pseudomolecules refined by optical, physical and genetic maps in flax. Plant J. 2018;95(2):371–84.  
    Dvorianinova EM, Bolsheva NL, Pushkova EN, Rozhmina TA, Zhuchenko AA, Novakovskiy RO, et al. Isolating Linum usitatissimum L. nuclear DNA enabled assembling high-quality genome. Int J Mol Sci. 2022;23(21):13244.  
    Zhang J, Qi Y, Wang L, Wang L, Yan X, Dang Z, et al. Genomic comparison and population diversity analysis provide insights into the domestication and improvement of flax. Iscience. 2020;23(4).  
  
USAGE INFORMATION  
Use at your own peril. :)  

If you post to the issues page on the GitHub itself, I might not reply in a reasonable time.
So, please feel free shoot me an email at esme.padgett@durham.ac.uk.  

SHARING INFORMATION
If using the data/code contained within this repository, or its associated pangenome/genome assembly data deposited in [], please cite:  
    (https://github.com/espadgett/lus_pangenome)  
    [paper citation will be inserted if/when available]  

Where possible, please also credit the following for their generation of sequencing data used in this project:  
    You FM, Xiao J, Li P, Yao Z, Jia G, He L, et al. Chromosome‐scale pseudomolecules refined by optical, physical and genetic maps in flax. Plant J. 2018;95(2):371–84.  
    Dvorianinova EM, Bolsheva NL, Pushkova EN, Rozhmina TA, Zhuchenko AA, Novakovskiy RO, et al. Isolating Linum usitatissimum L. nuclear DNA enabled assembling high-quality genome. Int J Mol Sci. 2022;23(21):13244.  
    Zhang J, Qi Y, Wang L, Wang L, Yan X, Dang Z, et al. Genomic comparison and population diversity analysis provide insights into the domestication and improvement of flax. Iscience. 2020;23(4).  
  
DATA & FILE OVERVIEW  
Directory file list:  
*FOLDER code_scripts*  
    **script_a1** - A sample Linux (Bash) script used to rename PGGB and SVIM-asm VCF outputs in the PanSN format.  
    **script_a2** - An R script used to validate the SV calls of a PGGB VCF using the calls of SVIM-asm VCFs.  
    **script_a3** - An R script to estimate the pangenome length contributions from Insertions and Inversions, building upon the reference L. usitatissimum var CDC Bethune. Pangenome size estimates are based on all pairwise genome comparisons and combinations (e.g. single, double, triple genome comparisons).  
   **script_a4** - An R script to generate the Eigenvalues, scree plot, and PCA for the SV calls from a VCF file.  
    **script_a5** - An R script to assign GO term with functions.  
    **script_a6** - An R script to assign GO term functions to SVs. GO terms are associated with a pacid; pacids—from the annotated transcript—are assigned to the appropriate pangenome SV. This allows for SVs to be functionally annotated. Later in the script (# Creating bubble plots), SV sets can also be made from within the pangenome, to determine functions assigned within sample groups.  
*FOLDER genome_asm*  
    *FOLDER busco_report*  
      ***_busco.out** - BUSCO output reports for the final RagTag-scaffolded assemblies  
    *FOLDER quast_report*  
      ***_report.txt** - QUAST output reports for the final RagTag-scaffolded assemblies  
    *FOLDER ragtag_asm_report*  
      ***_ragtag_info.zip** - RagTag assembly statistics (ragtag.scaffold.agp, ragtag.scaffold.asm.paf, ragtag.scaffold.asm.paf.log, ragtag.scaffold.confidence.txt, ragtag.scaffold.err, ragtag.scaffold.stats). Does NOT include ragtag.scaffold.fasta (due to file size constraints)  
*FOLDER pangenome_asm*  
    *FOLDER functional_annotation*  
      **SV_functional_annotation2.xlsx** - final collection of functionally annotated SVs from the L.usitatissimum pangenome. (Referenced as File A1 in manuscript).  
      **filtered_ids.txt** - pacid codes overlapping with VCF (SV regions), extracted from 2012 transcript of L.ustitatissimum (from Wang, Zhiwen, et al. "The genome of flax (Linum usitatissimum) assembled de novo from short shotgun sequence reads." The Plant Journal 72.3 (2012): 461-473.)
      **goterms_list.csv** - Gene Ontology (GO) terms associated with pacids.  
      **pacid_data.csv** - SV location info, also associated to pacid info.  
      **pacidname_aligned.sam.zip** - pacids aligned to pangenome location coordinates (initial step in determining which functional annotations from 2012 transcript of L.ustitatissimum were present in the pangenome).  
      **vcf_filtered_annotation.txt** - functional annotations from 2012 transcript of L.ustitatissimum, containing only annotations present at SV locations within the pangenome.  
    *FOLDER svcalls*  
      *FOLDER genome_svcalls*  
        ***_svim_filtered.vcf** - genome-level SV calls.  
      **candidate_results.csv** - SVs candidates for domestication and agricultural functions (causal mutant candidates).  
      **final_svdatasetmod2.vcf.zip** - pangenome-level SV calls validated by genome-level SV calls.  

File notes: Amongst the 'functional_annotation' folder files, there's a lot of overlap. The Excel file is your best bet.  

Data not included in current data package:  
1. Due to file size constraints:  
       the GFA pangenome graph of L.usitatissimum is not deposited in github.com/espadgett/Lus_pangenome. Instead, it is deposited at [].  
       *the final RagTag-scaffolded genome asm (FASTA) files are not deposited in github.com/espadgett/Lus_pangenome. They are instead available from [].  
       PGGB-output VCF files, recording the pangenome-level SV calls. Summary files can be delivered upon request to esme.padgett@durham.ac.uk. Pangenome SV calls are still represented within *final_svdatasetmod2.vcf.zip*.  
2. Additional HiC data, used in final genome and pangenome creation, is deposited in [], as work by Dr. Adrian Brennan. Live L.bienne var 1_6 shoots were collected at (36.80044, -5.39258) in 2016, L.bienne var Isr shoots were collected at (33.24028, 35.75056) prior to 2019.  

There is only one version of this dataset. (updated 2025-06-10)  

METHODOLOGICAL INFORMATION  
Methods are described in [paper citation will be inserted if/when available]  

And in greater detail, if it would be helpful, I have described my methods in my Master's thesis, when this project took place:  
[link to durham thesis]


