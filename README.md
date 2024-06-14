# Question Answering System with Web Scraping and Document Indexing

This project implements a question answering system that retrieves information from scraped web pages and indexed documents. 
It utilizes:
- web scraping to gather content from specific tabs on a website, 
- preprocesses the text data, 
- creates a PDF report, and 
- sets up an interactive querying interface using GenAI for natural language processing.

## Table of Contents

1. [Dependencies](#dependencies)
2. [Setup Instructions](#setup-instructions)
3. [Usage](#usage)
4. [Components](#components)
5. [License](#license)

## Dependencies

Ensure you have the following dependencies installed:
- `requests`
- `beautifulsoup4`
- `transformers`
- `sentence-transformers`
- `faiss-cpu`
- `pandas`
- `nltk`
- `chromadb`
- `reportlab`
- `langchain==0.0.187`
- `unstructured`
- `docx2txt`
- `genai`

You can install them using pip:

```bash
pip install -r requirements.txt
```

## Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/Diksha-Bisht/Question-Answer.git
cd Question-Answer
```

2. Install the dependencies as mentioned above.

3. Obtain an API key for GenAI from GenAI website and store it securely.

4. Ensure you have access to a directory containing PDF documents for indexing.

## Usage

### Running the Script
1. Directly run the cells in any of the `Jupyter` environments, OR
2. Run the script

To run the script, execute the following command:

```bash
python Q&A.py
```

> To do so you need to conver the file from `.ipynb` format to `.py` format.

### Input Requirements
- The script will prompt you to enter a question after initialisation.
- Ensure the question is relevant to the content scraped and indexed.


## Components

1. Web Scraping

>> Uses requests and BeautifulSoup to extract content from specific tabs of a website.

>>Combines scraped text data into a unified corpus for further processing.

2. Text Preprocessing

>> Normalizes text by converting to lowercase and removing unnecessary characters like newlines.

3. PDF Generation

>> Utilizes `reportlab` to create a PDF report from the preprocessed text data.

>> Saves the generated PDF in a specified directory `/content/sample_data` in this case).

4. Document Indexing and Querying

>> Sets up a document indexing pipeline using `ChromaDB` and `VectorStoreIndex`.

>> Uses `HuggingFace` for document embeddings and `GenAI` for querying.

>> Creates an interactive loop to input questions and retrieve answers based on indexed documents.



### Note:
The code needs correction for better performance, any possible corrections are always welcomed.

#### Thankyou

#### Collaborators:
1. Diksha Bisht: [bishtdiksha096@gmail.com](mailto:bishtdiksha096@gmail.com)
2. Deepak Garg: [gargdeepak114@gmail.com](mailto:gargdeepak114@gmail.com)



#### Please read Explaination.txt for the explaination of code
