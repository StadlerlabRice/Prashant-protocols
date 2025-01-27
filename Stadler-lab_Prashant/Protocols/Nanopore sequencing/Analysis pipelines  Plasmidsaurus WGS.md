**How is bacterial genome assembly generated?**
 
1. Remove the bottom 5% worst fastq reads via [Filtlong](https://github.com/rrwick/Filtlong) v0.2.1 (default parameters)  
2. Downsample the reads to 250 Mb via Filtlong to create a rough sketch of the assembly with [Miniasm](https://academic.oup.com/bioinformatics/article/32/14/2103/1742895) v0.3  
3. Using information acquired from the Miniasm assembly, re-downsample the reads to ~100x coverage (do nothing if there isn't at least 100x coverage) with heavy weight applied to removing low quality reads (helps small plasmids stick around)  
4. Run a [Flye](https://www.nature.com/articles/s41587-019-0072-8) v2.9.1 assembly with parameters selected for high quality ONT reads  
5. Polish Flye assembly via [Medaka](https://github.com/nanoporetech/medaka) v1.8.0 using the reads generated in step 3  
6. Run several analyses:

- annotation
    
    - [Bakta](https://www.microbiologyresearch.org/content/journal/mgen/10.1099/mgen.0.000685) v1.6.1
- contig analysis
    
    - [Bandage](https://academic.oup.com/bioinformatics/article/31/20/3350/196114) v0.8.1
- genome completeness and contamination
    
    - [CheckM](https://genome.cshlp.org/content/25/7/1043) v1.2.2
- species / plasmid identification
    
    - [Mash](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1841-x) v2.3 against RefSeq genomes+plasmids
    - [Sourmash](https://joss.theoj.org/papers/10.21105/joss.00027) v4.6.1 against GenBank
    - [CheckM](https://genome.cshlp.org/content/25/7/1043) v1.2.2
 > From <[https://www.plasmidsaurus.com/faq/#bact-assembly](https://www.plasmidsaurus.com/faq/#bact-assembly)>  

- Keeping this here for reference (in case they remove from site)