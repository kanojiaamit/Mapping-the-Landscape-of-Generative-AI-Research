# Mapping the Landscape of Generative AI Research through Web of Science

## Overview

In the rapidly evolving field of generative artificial intelligence (AI), it is critical for academics, practitioners, and policymakers to identify key research themes and understand their interconnections. This project leverages the comprehensive Web of Science (WoS) database to systematically search for publications related to generative AI. Through analytical approaches focused on keyword co-occurrence networks derived from author keywords, we aim to map the intellectual structure of the field and identify core themes and emerging trends in generative AI research.

## Objectives

- **Comprehensive Literature Retrieval:** Systematically retrieve publications related to generative AI from the Web of Science database using a well-defined set of search terms (e.g., "generative adversarial networks", "generative AI").
- **Keyword Co-Occurrence Network Analysis:** Construct a network from author keywords in the retrieved publications to visually represent connections between research themes.
- **Identification of Key Research Themes:** Analyze the keyword co-occurrence network using weighted network analysis to highlight focus areas, central keywords, and trends in generative AI research.

## Data Sources

- **Web of Science Publications:** Two datasets (`Project_3_data_1.xls` and `Project_3_data_2.xls`) containing bibliographic records and metadata for generative AI-related publications.

## Methodology

### 1. Data Retrieval

- Publications were systematically retrieved from the Web of Science database using relevant generative AI search terms.
- Two datasets were merged, resulting in a unified dataset of 1,674 publications.

### 2. Data Processing & Cleaning

- Author keywords were extracted from the publication metadata.
- Standard natural language processing steps were implemented using NLTK: tokenization, stopword removal, and lemmatization.

### 3. Keyword Co-Occurrence Network Construction

- Bigrams (pairs of keywords) were generated to capture co-occurrence relationships.
- A weighted network was built, where nodes represent keywords and edges represent the frequency of their co-occurrence.

### 4. Network Analysis & Visualization

- The network was analyzed to identify the most frequent and central co-occurrences.
- Visualization tools (e.g., `networkx`, `matplotlib`) were used to explore the structure of generative AI research themes.

### 5. Insights & Observations

- **Top Co-Occurrences:** Highlight dominant themes such as generative models, artificial intelligence, learning, networks, and model-based research.
- **Least Frequent Co-Occurrences:** Reveal specialized or niche intersections, particularly within human-computer interaction and interdisciplinary areas.
- **Overall:** The analysis provides a comprehensive map of major focus areas and potential future trends in generative AI research.

## Usage

1. **Setup:**
   - The analysis is implemented in a Jupyter notebook (`Mapping_GenAI_Landscape.ipynb`).
   - Required libraries: `pandas`, `numpy`, `matplotlib`, `nltk`, `networkx`.
   - The notebook is designed for Google Colab; ensure you have access to the datasets in your Google Drive.

2. **Run the Notebook:**
   - Mount Google Drive and set the working directory as shown in the notebook.
   - Load and concatenate the datasets.
   - Execute all cells for data processing, network construction, analysis, and visualization.

## Key Files

- `Mapping_GenAI_Landscape.ipynb` : Main analysis notebook.
- `Project_3_data_1.xls`, `Project_3_data_2.xls` : Datasets containing publication metadata.

## Example Observations

- The most frequent keyword pairs reveal strong interconnections between "generative", "ai", "learning", "network", and "model".
- Rare co-occurrences suggest emerging or niche areas, especially in the context of human-computer interaction (HCI) and interdisciplinary research.
- Both the most and least frequent co-occurrences provide valuable insights into the intellectual landscape of generative AI.

## License

This project is for academic and research purposes only. Please cite appropriately if you use or build upon this work.

## Acknowledgments

- Web of Science for providing access to the publication data.
- NLTK and Python open-source community for NLP and network analysis tools.
