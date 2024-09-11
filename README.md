# Word Similarity Extraction and Visualization from PDFs

This repository contains a Python script that processes and analyzes text extracted from three distinct PDFs: a food and travel blog, an airline booking receipt, and a food delivery receipt. The project focuses on identifying words similar to specified keywords and visualizing them effectively.

## Project Overview

### Objectives

1. **PDF Extraction**: 
   - Extract and clean text from the provided PDFs using libraries such as [PyPDF2](https://pypi.org/project/PyPDF2/) or [pdfplumber](https://pypi.org/project/pdfplumber/).

2. **Finding Similar Words in the Blog PDF**:
   - Analyze the text from "Mapping-Cost-of-Balanced-Diet-December-2014.pdf" using the **Gensim** library and the **GloVe** model ([glove.6B.50d.txt](https://machinelearningmastery.com/develop-word-embeddings-python-gensim/)).
   - Identify words similar to the keywords "FOOD" and "RESERVATION".
   - Store these similar words in two separate Bag of Words (BoW) models.

3. **Word Cloud Visualization**:
   - Create a word cloud from the words in the BoW models for the blog PDF, highlighting the most frequent terms.

4. **Analyzing Additional PDFs with GPT API**:
   - Use the **GPT API** to find words similar to "FOOD" and "RESERVATION" in "Air_Canada_Booking_Confirmation.pdf" and "Receipt_22Jun2022.pdf".
   - Display the list of similar words extracted from these additional PDFs.

### Installation

1. Clone this repository:
  
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Obtain API keys if needed for Gensim and GPT, and configure them according to the instructions provided in the notebook.

## Usage

1. **Run the Jupyter Notebook**:
    - Open the notebook and follow the instructions to extract text from the PDFs.
    - Analyze text using Gensim and the GPT API as described in the notebook.
    - Generate and visualize the word clouds.

2. **View Results**:
    - The notebook will display the results of the word similarity analysis and the word cloud visualizations.

## Documentation

The notebook includes detailed documentation and explanations for each step, including how Gensim was used for word similarity analysis and how the GPT API was applied to analyze additional PDFs.

## License

This project is licensed under the MIT License.
