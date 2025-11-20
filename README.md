# Long-Read Aligner Benchmark

This project benchmarks three long-read alignment tools — **Minimap2**, **NGMLR**, and **Winnowmap** — on simulated Oxford Nanopore reads. The main goals are to (1) compare alignment accuracy, runtime, and memory usage, and (2) assess whether alignment errors occur more frequently in **coding** or **noncoding** regions of the genome.

## Project Goals

- Generate simulated Nanopore-like reads using **NanoSim**.
- Align reads to a reference genome (e.g., human chr20) using Minimap2, NGMLR, and Winnowmap.
- Compute accuracy, mismatch/indel rates, runtime, and memory usage for each tool.
- Compare error patterns in coding vs noncoding regions using genome annotations (GFF).
- Summarize results in tables and plots for the final report.

## Repository Structure

- `environment/` – setup files (e.g., `requirements.txt`, instructions for Colab).
- `data/`
  - `reference/` – reference FASTA (e.g., chr20) and index files.
  - `annotations/` – GFF/GTF gene annotations.
  - `simulated_reads/` – NanoSim-generated FASTQ files.
- `notebooks/` – Jupyter/Colab notebooks for analysis.
- `scripts/` – shell scripts and Python helpers for running aligners and evaluation.
- `results/`
  - `logs/` – runtime and tool logs.
  - `figures/` – plots for accuracy, performance, and error patterns.

## Getting Started (Google Colab)

1. Open a new notebook in Google Colab.
2. Clone this repository:

   ```bash
   !git clone https://github.com/<your-username>/long-read-aligner-benchmark.git
   %cd long-read-aligner-benchmark
