# Primary skills 

* Population genetics: dN/dS, nucleotide diversity, selective sweep statistics, phylogenetic comparative methods

* Genomics: variant calling, bulk RNA-seq analysis, k-mer analyses

* Computational biology: snakemake workflows, high-performance and cloud computing, R, python, latex, github, bash

# Evolution of environment-specific gene expression

Paper: https://doi.org/10.1093/genetics/iyad074

This is my first chapter published in *Genetics*.

In this paper, I investigated whether the environment-specificity of a gene's expression affects the strength of purifying selection acting on it. The key idea behind this expectation is that selection acts on phenotypes. Thus, selection can only act to conserve a given DNA element when that element is producing a phenotype. If only some individuals in a population are experiencing heat stress, for example, then only that subset of individuals will experience selection to maintain their heat stress responses. The other individuals not experiencing heat stress could accumulate substitutions in their heat tolerance genes without any consequence. This expectation is well-solidified in theoretical papers, but has not been tested experimentally. I leveraged about 20 terabases of RNA-seq data in *Arabidopsis thaliana* from over 200 different environmental conditions to test this hypothesis. 

# K-mer-based approaches to population genetics, estimating genetic diversity

Preprint: https://doi.org/10.1101/2024.05.17.594778

This is the second chapter of my dissertation and it is currently undergoing peer review.

In this paper, I use k-mers to measure genetic diversity indices across 112 different plant species.

# Machine learning modles to estimate timing of allele frequency trajectories

Github repo: https://github.com/milesroberts-123/selection-demography-cnn/tree/dev

This is the third chapter of my dissertation and it is still in progress.

I am interested in building machine learning models that can, for a given genomic region known to have experienced a recent selective sweep, accurately predict the time to fixation of the sweep.
