# Biocomputing Project - Unix and Bioinformatics Data Handling

This project demonstrates basic Unix commands and bioinformatics data manipulation, including file downloads, directory management, sequence analysis, and data extraction.

## Project Structure
```
.
├── Tomilola/                # Main directory
│   ├── Biocomputing/        # Subdirectory for biocomputing files
│   │   ├── wildtype.gbk     # GenBank file (duplicate download removed)
│   │   ├── mutant           # Output file containing "tatatata" matches
│   │   └── compare/         # Directory for comparison data
│   │       ├── unix_intro_data/ # Extracted training data
│   │       └── Mito.dat     # Copied mitochondrial data file
│   └── wildtype.fna         # FASTA file moved here from Biocomputing
└── fasta.txt                # Line counts of FASTQ files
```

## Key Operations

1. **Directory Setup**:
   ```bash
   mkdir Tomilola Biocomputing
   ```

2. **Data Download**:
   - Downloaded `wildtype.fna` (FASTA) and `wildtype.gbk` (GenBank) from GitHub
   - Removed duplicate `wildtype.gbk.1`

3. **Sequence Analysis**:
   - Searched for "tatatata" motif in `wildtype.fna`
   - Saved results to `mutant` file

4. **Training Data Processing**:
   - Downloaded and extracted Unix intro data
   - Explored `seqmonk_genomes/Saccharomyces cerevisiae/EF4/`
   - Copied `Mito.dat` to main directory

5. **FASTQ Analysis**:
   - Counted lines in `lane8_DD_P4_TTAGGC_L008_R1.fastq.gz`
   - Saved all FASTQ line counts to `fasta.txt`

6. **Utilities**:
   - Installed `figlet` for ASCII art display
   - Used `nano` for file editing
   - Employed `wc`, `grep`, `tar`, `gunzip` for data handling

## Requirements
- Unix-like system (Linux/MacOS/WSL)
- Basic Unix utilities (installed by default)
- `figlet` (optional, for banner display)
- Internet access for downloads

## Usage
1. Clone or download the script
2. Make executable: `chmod +x script.sh`
3. Run: `./script.sh`
