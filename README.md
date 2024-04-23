[![author](https://img.shields.io/badge/author-Luiz_Carlos-blue.svg)](https://www.linkedin.com/in/luiz-carlos-vieira-4582797b/) [![](https://img.shields.io/badge/python-3.8+-yellow.svg)](https://www.python.org/downloads/release/python) [![Other Projects](https://img.shields.io/badge/Others-Projects-red.svg?style=flat)](https://github.com/ziul-bio?tab=repositories)


# DMS alpha-synuclein

Welcome to the DMS_a-syn repository! This project focuses on the descriptive data analysis for modeling alpha-synuclein Deep Mutation Scan (DMS) data. It was developed as part of a bioinformatics class project at the University of Texas at Austin. My team was composed of Nathan Strominger and me.

## Getting Started

These instructions will guide you through setting up your local environment and running the analysis.

### Prerequisites

Before you begin, ensure you have Python installed on your machine. This project was developed using Python 3.8. We recommend using a virtual environment to manage the dependencies.

### Installation

1. **Clone the repository:**

```bash
# clone the repository
git clone https://github.com/yourusername/DMS_a-syn.git
cd DMS_a-syn

# creates a vitual enviroment
python -m venv env
source env/bin/activate

# install the required packages
pip install -r requirements.txt
```


### Usage

To run the analysis and extract embeddings for your protein data, follow these steps:

All the steps on how to preprocessing the data and the modeling is described on 'data_processing.ipynb'

Extract embeddings: Replace model_name with the name of the model you are using, and fasta_file with the path to your FASTA file containing protein sequences.

```bash
python scripts/extract.py esm2_t30_150M_UR50D data/a_syn_DMS_sequences.fasta embeddings/output_folder_name 30 --include mean
```

