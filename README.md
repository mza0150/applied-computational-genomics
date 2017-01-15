# Applied Computational Genomics Course at UU: Spring 2017
- Faculty: Aaron Quinlan (aquinlan at genetics.utah.edu)
- Teaching assistants: Julie Feusier and Jingtao Guo
- Meets Tu and Th from 9:10-10:30 in HSEB 2948
- January 10 - April 25
- 2 credit hours

# Overview
This course will provide a comprehensive introduction to fundamental concepts and experimental approaches in the analysis and interpretation of experimental genomics data. It will be structured as a series of lectures covering key concepts and analytical strategies. A diverse range of biological questions enabled by modern DNA sequencing technologies will be explored including sequence alignment, the identification of genetic variation, structural variation, and ChIP-seq and RNA-seq analysis. Students will learn and apply the fundamental data formats and analysis strategies that underlie computational genomics research. **The primary goal of the course is for students to be grounded in theory and leave the course empowered to conduct independent genomic analyses.**

# Prerequisites
- Online introduction to Linux. Students must complete the following two online tutorials before class begins. If they don't things will be very complicated very quickly.
  - [Code academy's Intro to Unix](https://www.codecademy.com/en/courses/learn-the-command-line/lessons/environment/exercises/bash-profile)
  - [Command line bootcamp](http://rik.smith-unna.com/command_line_bootcamp/?id=9xnbkx6eaof)
- An Apple or Linux computer. Or a Windows machine with [Putty](http://www.putty.org/) installed.
- Every student must have a gmail account to work with Google Docs.

# Course lecture slides
[Class 1: Course overview and Intro to UNIX](https://docs.google.com/presentation/d/1B8kvetTDwUe-d7hZuV2NufVOMPM7MCxh_MyP-n9yDZo/edit?usp=sharing)
[Class 2: Intro to UNIX, Part 2](https://docs.google.com/presentation/d/1YSXYqCSHUZGRVr00oTttv_v1u83ccPLpF5_TMtW0iRI/edit?usp=sharing)
[Class 3: The human genome](https://docs.google.com/presentation/d/1304Ueup_n8_vqKjQZh-AV3dDAOs2gCqNgrm8o25nBHo/edit?usp=sharing)

# Syllabus
- **Class 1 (Tu Jan 10; Quinlan): Course overview and Intro to UNIX**
    - [Class 1 Slides](https://docs.google.com/presentation/d/1B8kvetTDwUe-d7hZuV2NufVOMPM7MCxh_MyP-n9yDZo/edit?usp=sharing)
    - **Required** Reading Prior to Lecture: 
        - Part 1 of [Unix and Perl Primer for Biologists](http://korflab.ucdavis.edu/Unix_and_Perl/current.pdf)
    - Topics covered
        - Brief history of computational biology
        - Course computing environment
        - Intro. to UNIX: Part 1
            - Logging in
            - The "shell"
            - "Home"
            - Navigation
            - File system
            - Files
            - Basic commands
                - ls
                - pwd
                - cd
                - mkdir
                - head
                - cat
- **Class 2 (Th Jan 12; Quinlan): Intro to UNIX Part 2**
    - [Class 2 Slides](https://docs.google.com/presentation/d/1YSXYqCSHUZGRVr00oTttv_v1u83ccPLpF5_TMtW0iRI/edit?usp=sharing)
    - **Required** Reading Prior to Lecture: 
        - Part 2 (Advanced UNIX) of [Unix and Perl Primer for Biologists](http://korflab.ucdavis.edu/Unix_and_Perl/current.pdf)
    - Topics covered
        - Intro. to UNIX: Part 2
          - grep
          - cut
          - redirects
    - **Homework 1 assigned. (due by start of class, Jan 17)**
 
- **Class 3 (Tu Jan 17; Quinlan): The human genome**
    - [Class 3 Slides](https://docs.google.com/presentation/d/1304Ueup_n8_vqKjQZh-AV3dDAOs2gCqNgrm8o25nBHo/edit?usp=sharing)
    - **Required** Reading Prior to Lecture: 
        - [Initial sequencing and analysis of the human genome](http://www.nature.com/nature/journal/v409/n6822/full/409860a0.html)
    - Topics covered
      - Karyotype
      - Chromosome structure
      - Centromeres
      - Banding
      - Chromatin
      - How was the genome sequenced?
        - sequencing technology
        - assembly strategy
      - Chromosomes
        - size
        - gene content
        - centromeres
      - Haplotypes
      - Genes and transcripts
        - how many?
        - isoforms
      - Repeat content
        - mobile elements
        - simple repeats
      - GC content, banding
      - CpG islands  
- **Class 4 (Th Jan 19; Quinlan): Using UNIX to find patterns in a genome**
    - **Required** Reading Prior to Lecture:    
        - None.     
    - Topics covered
      - Thought experiment: kmers and kmer uniqueness.
      - Restriction enzymes
      - Origins of replication
      - The UNIX PATH
      - Environment variables
      - Basic regular expressions with greo
      - sort
      - uniq
    - **Homework 2 (finding biological patterns in FASTA files with UNIX) assigned (due Jan 24)**
- **Class 5 (Tu Jan 24; Quinlan): Mutation, recombination and genetic variation**
    - **Required** Reading Prior to Lecture: 
        - [A global reference for human genetic variation](http://www.nature.com/nature/journal/v526/n7571/full/nature15393.html)
    - Topics covered
      - Mutation and mechanisms
      - Polymorphism
      - SNPs
      - Recombination
        - Haplotypes
        - Linkage disequilibrium
      - Landscape of human genetic variation
          - Alleles and genotypes
          - Allele frequency spectrum
          - Hardy weinberg equilibrium
          - Population stratification and Fixation index
      - INDELs
      - SV and CNV
      - Human mutation rates
- **Class 6 (Th Jan 26; Quinlan): Modern DNA sequencing technologies**
    - **Required** Reading Prior to Lecture: 
        - [Coming of age: ten years of next-generation sequencing technologies](http://www.nature.com/nrg/journal/v17/n6/full/nrg.2016.49.html)
    - Topics covered
        - Sanger dideoxy sequencing
        - Illumina sequencing
            - Overview of technology
            - Paired-end vs. single-end
        - Pacbio
        - Oxford nanopore
        - Base calling
        - FASTQ format
    - **Homework 3 (working with the FASTQ format) assigned (due Jan 31)**
- **Class 7 (Tu Jan 31; Quinlan): DNA sequence alignment**
    - **Required** Reading Prior to Lecture: 
        - [Alignment of Next-Generation Sequencing Reads](http://www.annualreviews.org/doi/abs/10.1146/annurev-genom-090413-025358?journalCode=genom)
    - Topics covered
      - Sequence alignment
          - Theory
          - Mapping versus alignment
          - Local versus global alignment
              - Smith waterman
              - Needleman-wunsch
          - Basic challenges with modern DNA sequences
          - Tools
      - The SAM/BAM format
      - samtools and IGV
    - **Homework 4 (creating and working with SAM/BAM files with samtools and IGV) assigned (due Feb 2)**
- **Class 8 (Th Feb 2; Quinlan and/or Marth): Detecting genetic variation, part 1**
    - **Required** Reading Prior to Lecture: 
        - [A framework for variation discovery and genotyping using next-generation DNA sequencing data](http://www.nature.com/ng/journal/v43/n5/full/ng.806.html)
    - **Optional** Reading Prior to Lecture: 
        - [A general approach to single-nucleotide polymorphism discovery.](http://www.nature.com/ng/journal/v23/n4/full/ng1299_452.html)
    - Topics covered
      - Polymorphism rate, nucleotide diversity, heterozygosity
          - variation between species
          - variation regionally within a species.
      - SNP and INDEL calling
          - Theory
              - Basic concept
              - Sequencing error
              - Bayes theorem and priors
      - Assigning a genotype
      - Common problems and artifacts
          - paralogy
          - low depth
          - high error rate
          - ambiguous alignment
      - Single sample variant detection
- **Class 9 (Tu Feb 7; Quinlan): Detecting genetic variation, part 2**
    - **Required** Reading Prior to Lecture: 
        - [The VCF format and VCFtools](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3137218/)
    - Topics covered
        - VCF format
          - Attributes
          - Genotypes
        - Population calling
        - Basic annotations
    - Exploring the format
        - examples
        - IGV
    - Manipulating VCF with bcftools
    - **Homework 5 (variant calling and working with VCF files with bcftools and UNIX) assigned (due Feb 9)**
- **Class 10 (Th Feb 9; Quinlan): Annotating of genetic variation**
    - **Required** Reading Prior to Lecture: 
        - [Choice of transcripts and software has a large effect on variant annotation](https://genomemedicine.biomedcentral.com/articles/10.1186/gm543)
    - Topics covered
        - Concepts
          - e.g, synonymous, non-synonymous
          - frameshift
          - stopgain
          - constraint
          - impact of transcript model
    - Tools
        - Polyphen
        - SIFT
        - vcfanno
        - CADD
        - VEP
        - SnpEff
    - **Homework 6 (annotating and profiling VCF files) assigned (due Feb 14)**
- **Class 11 (Tu Feb 14; Quinlan): Exome sequencing in studies of human disease**
    - **Required** Reading Prior to Lecture: 
        - [Exome sequencing as a tool for Mendelian disease gene discovery](http://www.nature.com/nrg/journal/v12/n11/full/nrg3031.html)
    - Topics covered
        - Exome capture
        - Variant detection in families
          - Mendelian inheritance
          - Mendelian violations (de novo mutations, LoH, uniparental disomy)
        - The Exome Aggregation Consortium
        - Mendelian disease analysis
            - Variant annotation
            - Using population allele frequency
    - **Homework 6 (variant prioritization with snpeff, gqt, and bcftools) assigned (due Feb 16)**
- **Class 12 (Th Feb 16; Quinlan): Somatic mutation in cancer and "healthy" tissue**
    - **Required** Reading Prior to Lecture: 
        - [Sensitive detection of somatic point mutations in impure and heterogeneous cancer samples](http://www.nature.com/nbt/journal/v31/n3/full/nbt.2514.html)
    - Topics covered
        - Sources of mutation
        - Mutational landscape
        - Tumor heterogeneity
        - Somatic mutation detetion
            - why is it so hard?
        - Using mutation to track cancer evolution
        - Mosaicism and disease
- **Class 13 (Tu Feb 21; Quinlan): Variation in genome structure**
    - **Required** Reading Prior to Lecture: 
        - [Genome structural variation discovery and genotyping](http://www.nature.com/nrg/journal/v12/n5/full/nrg2958.html)
    - Topics covered
        - The genome is repetitive
        - Segmental duplication
        - SV versus CNV
        - SV Mechanisms
            - NAHR / ectopic recombination
            - NHEJ
            - Replication mechansism
        - SV detection
        - Examples
    - **Homework 7 (visualizing SV and CNV) assigned (due Feb 23)**
- **Class 14 (Th Feb 23; Quinlan): Genome annotation**
    - **Required** Reading Prior to Lecture: 
        - None
    - Topics covered
      - How and why do we annotate a genome?
      - Conservation
      - CpG islands
      - Repeatmasker
      - Chromatin modifications
      - DNA methylations
      - Linkage blocks
  - **Homework 8 (exploring genome annotation files with UNIX) assigned (due Feb 28)**
- **Class 15 (Tu Feb 28; Quinlan): Genome data formats and genome arithmetic**
    - **Required** Reading Prior to Lecture: 
        - None
    - Topics covered
      - The genome as a coordinate system
      - BED format
      - GFF format
      - VCF format
      - Recap BAM format
      - UCSC and Biomart to retrieve genome annotations
      - UCSC and IGV to visualize 
- **Class 16 (Th Mar 2; Quinlan): Applied genome arithmetic with bedtools; part 1**
    - **Required** Reading Prior to Lecture: 
        - [BEDTools: the Swiss‐army tool for genome feature analysis](http://onlinelibrary.wiley.com/doi/10.1002/0471250953.bi1112s47/abstract?userIsAuthenticated=false&deniedAccessCustomisedMessage=)
    - Topics covered
      - The genome as a coordinate system revisited
      - Basic concepts of genome arithmetic
      - Introduction to bedtools
    - **Homework 9 (basic genome arithmetic with bedtools) assigned (due Mar 7)**
- **Class 17 (Tu Mar 7; Quinlan): Applied genome arithmetic with bedtools; part 2**
- **Class 18 (Th Mar 9; Quinlan): Digging deeper into UNIX, part 1**
    - awk
    - sed
    - tr
    - PATH
    - .bashrc
- **Class 19 (Tu Mar 21; Quinlan): ChIP-seq analysis**
    - experimental design
    - protocols
    - examples
- **Class 20 (Th Mar 23; Quinlan): RNA-seq analysis**
    - analyses
    - toolsets
- **Class 21 (Tu Mar 28; Quinlan): Basic probability**
    - Probability with coins and dice
    - Probability with DNA
    - Conditional probabilities
    - Use R for examples
- **Class 22 (Th Mar 30; Quinlan): Probability distributions**
    - Binomial
    - Gaussian
    - Poisson
    - Applications
- **Class 23 (Tu Apr 4; Quinlan): How do I know if my observation is significant?**
    - Models
    - Expectation
    - Tests for significance
- **Class 24 (Th Apr 6; Quinlan): Data visualization, part 1**
    - Why
    - Pattern recognition
    - Detect problems
    - Ansombe’s quartet
    - **Introduce class projects**
- **Class 25 (Tu Apr 11; Quinlan): Data visualization, part 2**
    - http://www.nature.com/collections/qghhqm/pointsofsignificance
    - Scatter plots
    - Histograms
    - Box whiskers
- **Class 26 (Th Apr 13; Quinlan): Digging deeper into UNIX, part 2**
    - loops
    - shuffling
    - randomization
    - advanced commands
    - basic scripts and pipelines
- **Class 27 (Tu Apr 18; Quinlan): Advanced topics**
- **Class 28 (Th Apr 20; Quinlan): Group Presentations, part 1**
- **Class 29 (Tu Apr 25; Quinlan): Group Presentations, part 2**
