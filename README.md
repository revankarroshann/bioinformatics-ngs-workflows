# Bioinformatics NGS Workflows

A beginner-to-intermediate bioinformatics workflow repository focused on Next-Generation Sequencing (NGS) data analysis, RNA-seq processing, workflow automation, and Linux-based bioinformatics pipelines.

This repository demonstrates hands-on implementation of commonly used bioinformatics tools and workflows used in genomic and transcriptomic analysis.

---

# Tools & Technologies

- Linux / Bash
- Python
- BWA
- SAMtools
- FastQC
- STAR
- featureCounts
- DESeq2
- Snakemake

---

# Repository Structure

```bash
bioinformatics-ngs-workflows/
│
├── data/           # Sample FASTQ, CSV, GTF files
├── notes/          # Learning notes and workflow explanations
├── results/        # BAM, VCF, QC and alignment outputs
├── scripts/        # Bioinformatics pipeline scripts
├── star_output/    # RNA-seq STAR alignment outputs
├── workflows/      # Snakemake workflow automation
├── ref.fa          # Reference genome
└── README.md
```

---

# Implemented Workflows

## 1. Variant Calling Workflow

Pipeline includes:
- Reference genome indexing
- Read alignment using BWA
- SAM/BAM conversion
- BAM sorting and indexing
- Variant calling
- Variant filtering

Key outputs:
- BAM alignment files
- VCF variant files
- Alignment statistics

---

## 2. RNA-seq Workflow

Pipeline includes:
- STAR genome indexing
- RNA-seq read alignment
- BAM processing
- featureCounts gene quantification
- Differential expression concepts using DESeq2

Key outputs:
- Sorted BAM files
- STAR alignment reports
- Gene count outputs

---

## 3. Workflow Automation with Snakemake

Implemented a simplified Snakemake workflow demonstrating:
- Workflow dependencies
- Automated execution order
- RNA-seq workflow orchestration
- Reproducible pipeline structure

---

# Example Scripts

## BWA Alignment Pipeline

```bash
bash scripts/bwa_pipeline_v3.sh
```

## FASTQ Analysis

```bash
bash scripts/fastq_analysis.sh
```

## Gene Analysis

```bash
bash scripts/gene_analysis.sh
```

---

# Example Outputs

Repository includes:
- Filtered VCF files
- Sorted BAM files
- FastQC reports
- STAR alignment logs
- Workflow execution reports

---

# Learning Objectives

This repository was built to strengthen practical understanding of:
- NGS workflows
- RNA-seq analysis
- Bioinformatics automation
- Linux-based pipeline execution
- Genomic data processing

---

# Future Improvements

Planned future additions:
- Full RNA-seq differential expression workflow
- Multi-sample automation
- Advanced visualization
- Containerized workflows
- Workflow reproducibility improvements
