Data were sourced from:

Schaum, N., Lehallier, B., Hahn, O. et al. Ageing hallmarks exhibit organ-specific temporal signatures. Nature 583, 596–602 (2020). https://doi.org/10.1038/s41586-020-2499-y

Raw data (not used) are available on GEO (GSE132040). Processed data found at: https://figshare.com/projects/The_murine_transcriptome_reveals_global_aging_nodes_with_organ-specific_phase_and_amplitude/65126

To create the data for this package, the raw count data from figshare (https://figshare.com/articles/dataset/Raw_count_table/8286230?file=15517064) for each selected organ was processed in DESeq2 with the formula:
    design = ~ age + sex
These results were then compared to the differential gene expression file, MACA_Bulk_deseq2_results.bin, (https://figshare.com/articles/dataset/Differential_Gene_Expression/12227531?file=22484429) to confirm our results were identical in both the number of genes identified to be DEGs and to what degree (e.g. log2fold change, p-adj is identical)

The full process can be found at:

inst/extdata/Schaum_SY.R

Note that we did not recreate any of the figures or tables from the article as we were able to create an identical match to the uploaded, processed data on figshare. 

