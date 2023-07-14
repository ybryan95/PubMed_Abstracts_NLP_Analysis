![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Python-docx](https://img.shields.io/badge/python--docx-3E8FC1?style=plastic&logo=python&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-007ACC?style=social&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat-square&logo=seaborn&logoColor=white)
![SciSpacy](https://img.shields.io/badge/SciSpacy-FFCA28?style=for-the-badge&logo=SciSpacy&logoColor=white)
![Biopython](https://img.shields.io/badge/Biopython-FFA500?style=plastic&logo=biopython&logoColor=white)


# :dna: NLP Analysis of Gene's Associations on Disease Ontology and Gene Ontology :dna:

This repository contains Python code that performs Natural Language Processing (NLP) to analyze genes' associations based on Disease Ontology and Gene Ontology. It does this using abstracts from PubMed, obtained via an automated literature search. 

## :pushpin: Table of Contents

- [Background](#background)
- [Prerequisites](#prerequisites)
- [Methodology](#methodology)
- [Output](#output)
- [Usage](#usage)
- [Contributing](#contributing)

## :bulb: Background

This project continues the Python scripts found in the following repositories:

1. [PubMed_scraper](https://github.com/ybryan95/PubMed_scraper): A script that scrapes PubMed for articles related to a given topic, extracting the titles, abstracts, and PMIDs of the articles using the PubMed API.
2. [PubMed_scraper_GPT](https://github.com/ybryan95/PubMed_scraper_GPT): A script that utilizes the GPT-3 language model to filter articles found via an automated literature search on PubMed.

We encourage you to visit these repositories to understand how the input file 'output_text.docx' is generated.

## :hammer_and_wrench: Prerequisites

Before you begin, ensure you have met the following requirements:

* You have installed the required Python libraries: `python-docx`, `pandas`, `requests`, `matplotlib`, `seaborn`, `numpy`, `json`, and `time`.
* You have a Windows/Linux/Mac machine running Python 3.7+.
* You have a BioOntology API key.

## :compass: Methodology

This script works by parsing information from the 'output_text.docx' document (a product of the PubMed_scraper and PubMed_scraper_GPT repositories). The document contains tables of gene names and related information. 

This information is processed and utilized to perform requests to the BioOntology API for Disease Ontology and Gene Ontology data related to each gene. The script then categorizes and analyses this data, outputting the results as heatmaps and frequency bar graphs for both Disease Ontology and Gene Ontology. 

## :bar_chart: Output

The script outputs:

1. Frequency plots of disease counts and disease frequencies.
2. A heatmap showing gene-disease associations.
3. A clustered heatmap (hierarchical clustering) of these associations.
4. Frequency plots and heatmaps for Gene Ontology data.

## :computer: Usage

Provide the 'output_text.docx' file from the PubMed_scraper and PubMed_scraper_GPT scripts as input, as well as your BioOntology API key.

> :warning: This code is provided as is. The user is responsible for ensuring compliance with the terms of use of the BioOntology API and any other data sources.

## :handshake: Contributing

Contributions, issues, and feature requests are welcome! For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.

