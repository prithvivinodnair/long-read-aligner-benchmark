# Environment Setup (Google Colab)

## 1. Clone the repository
```bash
!git clone https://github.com/<your-username>/long-read-aligner-benchmark.git
%cd long-read-aligner-benchmark
## Downloading the Reference Genome

GitHub does not allow uploading files >25MB.  
To obtain the reference genome used in this project:

1. Download human chromosome 22 from NCBI:
   https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_000001405.40/

2. Extract the FASTA file and place it in:
   data/reference/chr22.fa
