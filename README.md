# Nanopore Mitochondrial Genome Analysis Pipeline

Command-line (Bash) and R workflows for processing Oxford Nanopore long-read sequencing data from raw basecalled reads through mapping, consensus generation, SNP calling, multi-tier quality filtering, and downstream haplotyping analyses in vertebrate eDNA samples.

## Overview

This pipeline implements a complete end-to-end workflow including:

- Read mapping to mitochondrial reference genomes (minimap2)
- Consensus sequence generation (Medaka)
- Variant calling and normalization (bcftools)
- Multi-tier SNP filtering (strict, moderate, relaxed)
- Quality control and coverage assessment
- Haplogroup inference and eDNA–tissue concordance analyses
- Comparative evaluation of SNP panel robustness across filtering stringencies

## Workflow components

- `MEE_sequence_analysis_bash.txt`  
  Command-line workflow for processing Nanopore reads from basecalled FASTQ/BAM files through variant calling and SNP filtering.

- `MEE_sequence_analysis.Rmd`  
  R-based downstream analysis including SNP evaluation, haplotype clustering, concordance testing, and figure generation.

- `MEE_sequence_analysis_cleaned_annotated.Rmd`  
  Annotated and cleaned version of the analysis workflow for reproducibility and interpretation.

## Data availability

Input data and supporting metadata are available via Figshare (as referenced in the associated manuscript), including:

- `nanopore_reads_October_2025.zip`
- `nanopore_barcode_metadata.csv`
- `paired_samples_subset.csv`

## Context

This repository contains the analysis workflow developed for mitochondrial haplotyping from eDNA using long-read sequencing approaches.

## Status

Manuscript currently under review at *Methods in Ecology and Evolution*.

## Author

Lauren Rodriguez  
PhD Candidate, University of Innsbruck
