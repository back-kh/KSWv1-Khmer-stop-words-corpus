# KSW: Khmer Stop Word based Dictionary for Keyword Extraction

## Overview

KSW introduces a specialized approach to keyword extraction in Khmer text by leveraging a tailored stop word dictionary. Given the limited NLP resources for the Khmer language, our methodology effectively addresses the challenges associated with keyword extraction, significantly improving accuracy and relevance. 

## Motivation

Keyword extraction is vital for enhancing information retrieval, document classification, and text summarization. Traditional methods struggle with Khmer due to the scarcity of linguistic tools. By creating a custom stop word dictionary, KSW aims to fill this gap and promote effective text processing for Khmer.

## Methodology

### 1. Dataset Collection

We curated a diverse dataset of around 2,500 Khmer documents from sources such as news articles, blogs, and social media. This collection reflects contemporary Khmer usage and was meticulously filtered to maintain quality.

### 2. Stop Word Dictionary Construction

The stop word dictionary was developed through four key processes:

- **Translation:** We translated a list of common English stop words into Khmer, establishing a foundational list.
- **Synonym Addition:** To ensure comprehensive coverage, synonyms of the translated words were included.
- **Context-Specific Words:** Additional words were manually identified from our dataset that often appeared but held little informational value.
- **Redundancy Removal:** A thorough review eliminated duplicate entries, resulting in a refined list of approximately 1,000 Khmer stop words.

### 3. Keyword Extraction Process

Our extraction process involves:

- **Preprocessing:** Cleaning text data and normalizing word forms.
- **Stop Word Removal:** Filtering out non-informative words using our stop word dictionary.
- **Candidate Keyword Extraction:** Identifying significant words based on frequency thresholds.
- **Keyword Ranking:** Employing TF-IDF to rank keywords based on relevance and frequency.

## Results

KSW demonstrated superior performance compared to traditional methods like TF-IDF and RAKE, achieving precision and recall metrics that indicate its effectiveness. Detailed experimental results are available in the paper.

### Evaluation Metrics

- **Precision:** Accuracy of extracted keywords.
- **Recall:** Completeness of keyword identification.
- **F1-Score:** Balance between precision and recall.

## Applications

KSW can be utilized in various NLP tasks, including:

- **Improving Search Engines:** Enhancing retrieval accuracy by filtering out common words.
- **Text Analysis:** Providing clearer insights in sentiment analysis and summarization tasks.

## Future Work

We aim to expand the stop word dictionary and explore advanced techniques such as machine learning and deep learning to further enhance keyword extraction for Khmer.

## Acknowledgments

Special thanks to ARES Belgium and the Chinese Academy of Sciences for their support.

## Citation
@article{thuon2024ksw,
  title={KSW: Khmer Stop Word based Dictionary for Keyword Extraction},
  author={Thuon, Nimol and Zhang, Wangrui and Thuon, Sada},
  journal={arXiv preprint arXiv:2405.17390},
  year={2024}
}
Join us in advancing Khmer language processing and contributing to the development of NLP tools for under-resourced languages!
