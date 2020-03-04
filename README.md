# Oviz-Bio-demo

Documents of [Oviz-Bio](https://bio.oviz.org/), a Platform for Bioinformatics Visualization

# Intergrated

## LandScape
The 'LandScape' visualization is frequently utilized to provide a systematic illustration of integrative data from multiple layers of batch samples, which are always compared to each other on certain attributes, such as genes and biological pathways mutated in cancers. To visualize data, a CSV file in the required format is needed.
### demo_data
Several demo CSV files are provided.
- `landscape_demo.csv` is the official demo CSV file.
- `PMIDxxx.Figx.landscape.csv` files to present LandScape instances in published papers (see [Reference](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/LandScape/markdown/LandScape-References.markdown)).
### markdown
Markdown files of LandScape analysis page on Oviz-Bio Platform.
- Manual
- References
- About

<!-- ## Circos -->

# Small Mutation

## Mut: On Genes
The 'Mutations on Genes' displays SNVs and InDels with their coordinates and function annotations along the selected transcript of a given gene in three levels (genome, cDNA, and peptide).
### demo_data
- Check the `Mutation CSV input` official demo input [here](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/Mut_OnGenes/demo_data/Mut_OnGenes_demo.mutations.csv).
- Check the `Depth BGZ input` official demo input [here](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/Mut_OnGenes/demo_data/Mut_OnGenes_demo.depth.tsv.bgz).
### markdown
Markdown files of 'Mut: On Genes' page on Oviz-Bio Platform.
- Manual
- References
- About

## SNV: Context
The 'Context' visualization, otherwise known as the 'Lego plot' of mutational frequencies, describes the distribution of mutations across batch samples on a given region. To visualize data, To visualize data, a BGZ file in the required format is needed.
### demo_data
Several demo TSV files are provided.
- [SNV_Context_demo_MutList.tsv.bgz](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/SNV_Context/demo_data/SNV_Context_demo_MutList.tsv.bgz) is the official demo BGZ file for the visualization.
- [SNV_Context_demo_Region.bed](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/SNV_Context/demo_data/SNV_Context_demo_Region.bed) is the official demo TSV file for the optional custom region data. 
### markdown
Markdown files of Context analysis page on Oviz-Bio Platform.
- Manual
- References
- About

## SNV: Signature
The 'Signature' visualization is wildly used in mutational signature analysis. It shows the signature profile with the conventional 96 mutation type classification. We also compare each signature with all recorded signature references in the [COSMIC database](https://cancer.sanger.ac.uk/cosmic/signatures/SBS/) by the cosine similarity test. The top three similar signature references are listed with their percentage of similarity. To visualize data, a CSV file in the required format is needed.
### demo_data
- Check the official demo input [here](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/SNV_Signature/demo_data/SNV_Signature_demo.csv).
### markdown
Markdown files of Signature analysis page on Oviz-Bio Platform.
- Manual
- References
- About

## Mut: Signature Dist
The 'Signature Dist' visualization shows the fraction of signatures within individual samples. It can also be used to show the fraction of signatures within several cancer types. To visualize data, a CSV file in the required format is needed.
### demo_data
- Check the official demo input [here](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/Mut_Signature_dist/demo_data/Mut_Signature_dist_demo.csv).
### markdown
Markdown files of Signature Dist analysis page on Oviz-Bio Platform.
- Manual
- References
- About

# Copy Number Variation

## CNV: Single Sample
The 'Single Sample' visualization is an interactive version of the output plot from 'Patchwork', a bioinformatics tool for analyzing allele-specific copy numbers and loss-of-heterozygosity in cancer genomes. This visualization summarizes all 24 chromosomal plots generated by 'Patchwork' and provides user with the choice to highlight information of one particular chromosome. To visualize data, a CSV file in the required format is needed.
### demo_data
- Check the official demo input [here](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/CNV_Single_Sample/demo_data/CNV_Single_Sample_demo.csv).
- User can directly use the output from the 'Patchwork' tool as our input file.
### markdown
Markdown files of Single Sample analysis page on Oviz-Bio Platform.
- Manual
- References
- About

## CNV: Group Samples
The 'Group Sample' visualization is an interactive and extended version of the output plot from 'GISTIC', a bioinformatics tool for identifying regions of the genome that are significantly amplified or deleted across a set of samples. To visualize data, three TSV files in the required format are needed.
### demo_data
Several demo TSV files are provided.
- **scores**: [Group_Sample_scores.tsv](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/CNV_Group_Samples/demo_data/CNV_Group_Samples_demo_scores.tsv). User can directly use the score output from the 'GISTIC' tool as our input file.
- **amp_genes.conf_90**: [Group_Sample_amp_genes.conf_90.tsv](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/CNV_Group_Samples/demo_data/CNV_Group_Samples_demo_amp_genes.conf_90.tsv). User can directly use the amp_genes.conf_90 output from the 'GISTIC' tool as our input file.
- **del_genes.conf_90**: [Group_Sample_del_genes.conf_90.tsv](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/CNV_Group_Samples/demo_data/CNV_Group_Samples_demo_del_genes.conf_90.tsv). User can directly use the del_genes.conf_90 output from the 'GISTIC' tool as our input file.
### markdown
Markdown files of Group Samples analysis page on Oviz-Bio Platform.
- Manual
- References
- About

# Structure Variation

## SV:Heatmap
Linkage heatmap is an useful method to visualize read linkage patterns on SV event, especially in studies with long-range sequencing data, such as 10x linked-reads. We apply the "SV: Heatmap" visualization to display the heatmap matrix based on sequencing reads linkage between two local windowlized regions of SV case. The color depth of each cross-linked window pair is proportional to the number of linkages. Along the chromosome coordinate axis of the heatmap matrix, annotation information is added, such as Ensembl genes. To visualize data, upload a **TXT** file in the *required* format, and then use sidebar options to adjust heatmap color scheme and choose other SVs to display if uploaded data contains multiple cases.

### demo_data
Two demo **TXT** files are provided.
- [10x_resolution80.txt](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/SV_Heatmap/demo_data/10x_resolution80.txt) stores the shared 10x barcodes linkage matrix.
- [pair_end_resolution25_ALK-KIF5B.txt](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/SV_Heatmap/demo_data/pair_end_resolution25_ALK-KIF5B.txt) stores the shared paired-end reads linkage matrix.
### markdown
Markdown files of SV:Heatmap analysis page on Oviz-Bio Platform.
- Manual
- References
- About

## SV:Reads Support
The "SV:Reads Support" visualization is frequently utilized to provide the detail illustration of supporting split reads for given SV events. To visualize data, a **TXT** file in the required format is needed.
### demo_data
[indels.junc.reads.txt](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/SV_Read_Support/demo_data/indels.junc.reads.txt) stores information of supporting split reads for given SV events.
### markdown
Markdown files of SV:Reads Support analysis page on Oviz-Bio Platform.
- Manual
- References
- About

# Gene Fusion

## Fusion Genes
the `Fusion Genes` visualization displays the whole structure of chimeric transcript structure.
### demo_data
- Check the official demo input [here](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/Fusion_Genes/demo_data/Fusion_Genes_demo.tsv).
### markdown
Markdown files of 'Fusion Genes' page on Oviz-Bio Platform.
- Manual
- References
- About

# Onco Virus

## Virus: Integ HotSpot
the `Virus: Integ HotSpot` visualization displays the oncovirus integrated hotspot of group samples in a genome browser way.
### demo_data
- Check the official demo input [here](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/Virus_IntegHotSpot/demo_data/Virus_IntegHotSpot_demo.csv).
- [HBV_PMID22634754.csv](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/Virus_IntegHotSpot/demo_data/HBV_PMID22634754.csv) and [HPV_PMID25581428.csv](https://github.com/Nobel-Justin/Oviz-Bio-demo/blob/master/Virus_IntegHotSpot/demo_data/HPV_PMID25581428.csv) record integration cases of oncovirus HBV and HPV, respectively.
### markdown
Markdown files of `Virus: Integ HotSpot` page on Oviz-Bio Platform.
- Manual
- References
- About
