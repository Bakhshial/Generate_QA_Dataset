# Generate QA Dataset For AI Chatbot Fine-Tuning
This repository contains the code and resources for fine-tuning a large language model (LLM) to create a cybersecurity-focused AI chatbot. The chatbot is designed to assist users with cybersecurity-related queries by generating accurate and context-aware responses. The fine-tuning process involves generating question-answer pairs from various cybersecurity sources such as websites and PDFs.

### Project Overview
The goal of this project is to build an AI chatbot that leverages a fine-tuned LLM to provide reliable and informative answers to cybersecurity-related questions. This repository includes scripts for:

    Extracting and cleaning text data from PDFs and web pages.
    Generating question-answer pairs using a T5-based model.
    Handling text encoding issues and ensuring clean data for fine-tuning.
    Saving the generated question-answer pairs in both CSV and JSON formats for further use.
### Features
    Text Extraction: Extracts and preprocesses text from PDFs and websites.
    Question-Answer Generation: Uses a pre-trained T5 model to generate QA pairs from the extracted text.
    Data Cleaning: Removes unwanted characters and formatting errors from the text to ensure clean and usable data.
    Data Storage: Saves the generated QA pairs in CSV and JSON formats, ready for fine-tuning the model.
### Installation
To run the code in this repository, you'll need the following Python packages:

    spacy
    transformers
    PyMuPDF (installed as fitz)
    requests
    beautifulsoup4
    re (part of Python standard library)
    json (part of Python standard library)
    csv (part of Python standard library)
    You can install the required packages using pip:


    pip install spacy transformers pymupdf requests beautifulsoup4
Ensure that you have the appropriate versions of Python and PyTorch installed to support the transformers library.

Usage
Text Extraction:

Use the script to extract text from cybersecurity-related PDFs or websites.
Question-Answer Generation:

The script processes the extracted text to generate QA pairs using the T5 model.
Data Cleaning:

The text is cleaned to remove special characters, encoding errors, and irrelevant content.
Data Storage:

The generated QA pairs are saved in qa_dataset.csv and qa_dataset.json for further use.
Example
To generate QA pairs from a website, use the following code snippet:

python

    website_url = 'https://www.example.com'
    website_text = scrape_website(website_url)
    qa_pairs = generate_qa_pairs(website_text)
The resulting QA pairs will be saved in the specified CSV and JSON files.

Contributing
Contributions are welcome! If you'd like to contribute to this project, please fork the repository and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

Contact
If you have any questions or suggestions, feel free to open an issue or contact the repository owner.
