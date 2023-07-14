# NLP Analysis of Gene's Associations on Disease Ontology and Gene Ontology

## Table of Contents
1. [Background](#background)
2. [Methodology](#methodology)
3. [Output](#output)
4. [Requirements](#requirements)
5. [Usage](#usage)

<a name="background"></a>
## Background

This repository contains Python code that performs Natural Language Processing (NLP) to analyse genes' associations based on Disease Ontology and Gene Ontology. It does this using abstracts from PubMed, obtained via an automated literature search. This code is a sequel to the Python scripts found in the following repositories:

1. [PubMed_scraper](https://github.com/ybryan95/PubMed_scraper): A script that scrapes PubMed for articles related to a given topic, extracting the titles, abstracts, and PMIDs of the articles using the PubMed API.
2. [PubMed_scraper_GPT](https://github.com/ybryan95/PubMed_scraper_GPT): A script that utilizes the GPT-3 language model to filter articles found via an automated literature search on PubMed. It then parses the results of the queries to extract the titles, abstracts, and PMIDs of the articles.

Please visit these repositories if you are interested in understanding how the input file 'output_text.docx' is generated. 

<a name="methodology"></a>
## Methodology

This script works by parsing information from the 'output_text.docx' document (a product of the PubMed_scraper and PubMed_scraper_GPT repositories). The document contains tables of gene names and related information. This information is processed and utilized to perform requests to the BioOntology API for Disease Ontology and Gene Ontology data related to each gene. The script then categorizes and analyses this data, outputting the results as heatmaps and frequency bar graphs for both Disease Ontology and Gene Ontology. 

<a name="output"></a>
## Output

The output of this script includes:

1. Frequency plots of disease counts and disease frequencies for diseases that occur more or less than five times.
2. A heatmap showing the associations between different genes and diseases.
3. A clustered heatmap of these gene-disease associations.
4. Similarly, frequency plots and heatmaps are generated for Gene Ontology data as well.

<a name="requirements"></a>
## Requirements

This script requires several Python libraries including:

- Python-docx: For reading and writing Microsoft Office Word documents.
- Pandas: For data manipulation and analysis.
- Requests: For making HTTP requests.
- Matplotlib and Seaborn: For data visualization.
- Numpy: For numerical operations.
- json: For handling JSON data.
- time: For managing the pace of API requests.

Additionally, the script utilizes the BioOntology API and requires an API key for this service. 

<a name="usage"></a>
## Usage

To use this script, you simply need to provide the 'output_text.docx' file from the PubMed_scraper and PubMed_scraper_GPT scripts as input. You will also need to provide your BioOntology API key.

> **_NOTE:_** This code is provided as is, and the user is responsible for ensuring compliance with the terms of use of the BioOntology API and any other data sources.


