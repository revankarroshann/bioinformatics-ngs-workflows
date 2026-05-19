# linux-ngs-foundation
This repository documents my hands-on training in Linux, Python, and bioinformatics workflows as preparation for NGS Analyst roles.

Environment Setup
* Installed WSL (Ubuntu)
* Installed Miniconda and created bioinformatics environment
* Installed libraries: Biopython, Pandas, NumPy, Matplotlib
* Verified tools: FastQC, BWA, SAMtools

Linux Command Line Skills
File & Directory Operations
* Navigation: `pwd`, `ls`, `cd`
* File handling: `touch`, `cp`, `mv`, `rm`
* Directory creation: `mkdir`

Pattern Matching
* Wildcards: `*.txt`, `*.fastq`

Practice Work
* Created and managed files using terminal commands
* Practiced file movement, copying, and deletion
* Applied wildcard-based filtering for file selection

Key Learnings
* Efficient file handling using terminal instead of GUI
* Importance of Linux in handling large bioinformatics datasets
* Foundation for building reproducible pipelines

Progress Log
* Day 1: Environment setup (WSL, Conda, libraries)
* Day 2: Linux basics (navigation, file handling, wildcards)

Next Steps
* Text processing: `grep`, `cut`, `sort`, `uniq`
* Bash scripting
* NGS file formats (FASTQ, SAM/BAM, VCF)
* Python-based sequence processing

Text Processing Day 3
- grep → filtering data based on patterns
- wc → counting lines
- sort → ordering data
- uniq → removing duplicates / counting frequency
- cut → extracting columns from structured data
- pipes (|) → chaining commands

 Day 4 (Pipelines)

- Created pipeline scripts to automate data processing
- Combined grep, sort, wc into workflows
- Practiced multi-step filtering using pipelines
- Learned how to run scripts using bash

Day 5 (Structured Data Processing)
- Worked with CSV-like biological data
- Learned to extract columns using cut
- Used grep for text filtering
- Used awk for numeric conditions
- Combined tools to solve structured data problems

Day 6 (FASTQ Processing)
- Worked with FASTQ-like structured data
- Understood 4-line read format
- Extracted sequence lines using awk (NR % 4)
- Filtered sequences based on patterns
- Linked sequence data with read IDs

Day 7 (FASTQ Workflow)
- Built mini pipeline for FASTQ data processing
- Extracted sequences using awk
- Applied filtering conditions on sequence data
- Linked sequence data with read IDs

Day 8 (Dynamic FASTQ Pipeline)
- Built reusable FASTQ processing pipeline
- Added dynamic pattern input using command-line arguments
- Extracted sequences and filtered based on user-defined patterns
- Linked sequence data with corresponding read IDs

 Day 9 (FastQC)
- Installed FastQC
- Generated quality report for FASTQ file
- Checked sequence quality, length, and GC content

Day 10 (SAMtools)
- Created SAM file with aligned reads
- Converted SAM to BAM format
- Used samtools to view and count reads

Day 11 (SAMtools - Sorting & Indexing)
- Sorted BAM file using samtools sort
- Indexed BAM file for fast access
- Queried reads from chromosome using samtools view

 Day 12 (Alignment Statistics)
- Used samtools flagstat to analyze alignment
- Evaluated total, mapped, and unmapped reads
- Calculated mapping percentage

 Day 13 (Python - FASTQ Processing)
- Wrote Python script to read FASTQ file
- Counted total number of sequences
- Applied modulo logic (i % 4) to extract sequence lines

Day 14 (Python - GC Content Filtering)
- Calculated GC percentage of sequences from FASTQ
- Filtered sequences with GC > 50%
- Applied Python for biological data processing

Day 15 (BWA Alignment Pipeline)
- Aligned FASTQ reads to reference genome using BWA
- Generated SAM file from alignment
- Converted SAM to BAM
- Sorted and indexed BAM file
- Evaluated alignment using samtools flagstat

Day 16 (Pipeline Automation)
- Created bash script to automate NGS workflow
- Integrated BWA alignment and SAMtools processing
- Generated BAM, sorted BAM, index, and stats automatically

Day 17 (Reusable Pipeline)
- Modified pipeline to accept FASTQ input as argument
- Used basename to generate dynamic output file names
- Prevented overwriting of files
- Made pipeline reusable for different datasets

Day 18 (Batch Processing)
- Implemented loop to process multiple FASTQ files
- Automated alignment and SAMtools steps for each file
- Enabled batch processing for large datasets

Day 19 (Project Structure)
- Organized repository into data, scripts, and results folders
- Updated pipeline to use structured paths
- Improved project readability and maintainability

Day 20 (Flexible Pipeline)
- Built a fully flexible pipeline using input arguments
- Accepts input folder, reference genome, and output folder
- Supports batch processing of FASTQ files
- Structured workflow for real-world usage

Day 21 (Variant Calling Setup)
- Installed bcftools
- Prepared sorted and indexed BAM files
- Understood preparation steps required before variant calling

Day 22 (First Variant Calling)
- Generated first VCF file using bcftools
- Learned mpileup and variant calling workflow
- Understood REF, ALT, and genomic variant positions

Day 23 (Understanding VCF)
- Learned basic VCF structure
- Understood CHROM, POS, REF, ALT, and QUAL columns
- Practiced interpreting simple variants

Day 24 (Variant Filtering)
- Learned variant filtering using bcftools
- Understood QUAL (confidence score) and DP (read depth)
- Generated filtered VCF file using QUAL-based filtering
- Practiced removing low-confidence variants

Day 25 (Variant Annotation Basics)
- Learned the purpose of variant annotation
- Understood LOW, MODERATE, and HIGH impact variants
- Differentiated between variant calling and annotation

Day 26 (RNA-seq Introduction)
- Learned the purpose of RNA-seq and gene expression analysis
- Understood the difference between WGS and RNA-seq
- Installed STAR aligner
- Learned why STAR is splice-aware

Day 27 (STAR Genome Indexing)
- Learned STAR genome indexing for RNA-seq alignment
- Understood why indexing is required before alignment
- Learned that tiny genomes may require smaller indexing settings
- Successfully generated STAR index files

Day 28 (STAR RNA-seq Alignment)
- Performed RNA-seq alignment using STAR
- Generated RNA-seq alignment outputs and statistics
- Learned the role of Aligned.out.sam and Log.final.out
- Understood STAR as a splice-aware RNA-seq aligner

Day 29 (RNA-seq BAM Processing)
- Converted STAR SAM output into BAM format
- Sorted and indexed RNA-seq BAM files
- Generated alignment statistics using samtools flagstat
- Reused BAM workflow concepts in RNA-seq analysis

Day 30 (featureCounts and Gene Expression)
- Installed and used featureCounts for RNA-seq analysis
- Learned how gene expression counts are generated
- Understood the role of GTF annotation files
- Generated a basic gene count matrix

Day 31 (Understanding Count Matrices)
- Learned the structure of RNA-seq count matrices
- Understood rows as genes and columns as samples
- Interpreted gene expression counts from featureCounts output
- Connected read counts with gene expression levels