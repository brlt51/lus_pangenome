This readme file was generated on 2025-06-10 by Esme Padgett

GENERAL INFORMATION
Title of Dataset: Lus_pangenome_draft

Author/Principal Investigator Information
Name: Esme Padgett
Institution: Durham University
Address: Durham DH1 3LE
Email: esme.padgett@durham.ac.uk

Author/Associate or Co-investigator Information
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
  
SHARING INFORMATION
If using the data/code contained within this repository, or its associated pangenome/genome assembly data deposited in [], please cite:
  (https://github.com/espadgett/lus_pangenome)
  [replace with paper citation when available]

Where possible, please also credit the following for their generation of sequencing data used in this project:
  You FM, Xiao J, Li P, Yao Z, Jia G, He L, et al. Chromosome‐scale pseudomolecules refined by optical, physical and genetic maps in flax. Plant J. 2018;95(2):371–84.
  Dvorianinova EM, Bolsheva NL, Pushkova EN, Rozhmina TA, Zhuchenko AA, Novakovskiy RO, et al. Isolating Linum usitatissimum L. nuclear DNA enabled assembling high-quality genome. Int J Mol Sci. 2022;23(21):13244.
  Zhang J, Qi Y, Wang L, Wang L, Yan X, Dang Z, et al. Genomic comparison and population diversity analysis provide insights into the domestication and improvement of flax. Iscience. 2020;23(4).
  
DATA & FILE OVERVIEW
Directory file list:
code_scripts
  script_a1 - 
  script_a2 - 
  script_a3 - 
  script_a4 - 
  script_a5 - 
  script_a6 - 
genome_asm
  busco_report
    atlant_busco.out - 
    bienne_busco.out - 
    heiya_busco.out - 
    longya_busco.out - 
  quast_report
    atlant_report.txt - 
    bienne_report.txt - 
    heiya_report.txt - 
    longya_report.txt - 
  ragtag_asm_report*
    atlant_ragtag_info.zip -
    bienne_ragtag_info.zip -
    heiya_ragtag_info.zip -
    longya_ragtag_info.zip -
pangenome_asm
  functional_annotation
    SV_functional_annotation2.xlsx -
    filtered_ids.txt - 
    goterms_list.csv - 
    pacid_data.csv - 
    pacidname_aligned.sam.zip - 
    vcf_filtered_annotation.txt - 
  svcalls
    genome_svcalls
      atlant_svim_filtered.vcf - 
      bienne_svim_filtered.vcf - 
      heiya_svim_filtered.vcf - 
      longya_svim_filtered.vcf - 
    candidate_results.csv - 
    final_svdatasetmod2.vcf.zip - 

Relationship between files, if important: 

Data not included in current data package:
1. Due to file size constraints:
       the GFA pangenome graph of L.usitatissimum is not deposited in github.com/espadgett/Lus_pangenome. Instead, it is deposited at [].
       *the final RagTag-scaffolded genome asm (FASTA) files are not deposited in github.com/espadgett/Lus_pangenome. They are instead available from [].
       PGGB-output VCF files, recording the pangenome-level SV calls. Summary files can be delivered upon request to esme.padgett@durham.ac.uk. Pangenome SV calls are still represented within *final_svdatasetmod2.vcf.zip*.
2. Additional HiC data, used in final genome and pangenome creation, is deposited in [], as work by Dr. Adrian Brennan. Live L.bienne var 1_6 shoots were collected at (36.80044, -5.39258) in 2016, L.bienne var Isr shoots were collected at (33.24028, 35.75056) prior to 2019.

There is only one version of this dataset (updated 2025-06-10)

METHODOLOGICAL INFORMATION
Methods are described in [paper citation]

And in greater detail, if it would be helpful, I have described my methods in my MBiol thesis:
[link to durham thesis]

If you post to the issues page on the GitHub itself, I might not reply in a reasonable time.
So, please feel free shoot me an email at esme.padgett@durham.ac.uk. This is my first GitHub repo so I might have made mistakes :)
