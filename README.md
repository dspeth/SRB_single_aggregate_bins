## SRB_single_aggregate_bins
Jupyter notebooks and table files used for the binning of metagenomes obtained from MDA amplified single ANME-SRB aggregates

### General
The files in this repository represent 6 metagenomes retrieved from individual aggregates composed of methane oxidizing ANME archaea and sulfate reducing bacteria. 
Single agregate sorting and sequencing was done at the Joint Genome Institute (JGI), and data was downloaded from their Integrated Microbial Genomes (IMG) resource.
The single aggregates were MDA amplified prior to sequencing, and thus traditional binning tools can not be used to separate the organisms. 
Instead, the kmer composition of the contigs and taxonomic annotation of the genes on the contigs is used to assign bins. 

Binning was done using jupyter notebooks, included in the repository. Contigs were subsequently retrieved using the tab_based_seq_lookup.pl script included in the repository.
The notebooks detail the preprocessing that was done on JGI supplied files to obtain the "*_kmer_freq" and "*_phylogeny_w_header" files used in the binning.

### files
*.fna - Contig fasta file assembled by JGI  
*.ipynb - noteook with the code used to bin the dataset  
*_kmer_freq - kmer frequencies of the contigs, with k=4  
*_phylogeny_w_header - taxonomy of the genes on the contigs  
