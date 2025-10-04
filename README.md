# Coding-Exercise LangExtract – NLP Text Language Extraction Project
This notebook implements automated extraction of structured language features (entities) from unstructured documents using the langextract library. The main workflow is designed to read document inputs, process them using entity extraction models, and export results for analysis and visualization. This is suitable for use-cases like contract analysis, financial document parsing, and knowledge discovery from text-heavy datasets.

Project Overview
The notebook installs and sets up the latest version of langextract, along with core dependencies for NLP, data handling, and visualization (e.g., pandas, numpy, easyocr, docling-core).

The workflow guides you through entity extraction for financial and government documents, with examples focused on identifying organizations, dates, monetary amounts, persons, locations, roles, account numbers, contract references, percents, and other key fields.

Main Pipeline Steps
Loads or uploads documents (supports PDF input for batch processing).

Initializes extraction with sample prompts, specifying which entities to extract from input text.

Runs extraction models to process each document, saving annotated extraction results as JSONL (extractionresults.jsonl) for review.

Generates a visualization (visualization.html) for quick analysis of extractions.

Demonstrates extraction from sample financial transaction text as well as government policy documents, providing both code and output examples.

How to Use
Change the input file or folder to your target documents (text, PDF, etc.).

Select or modify the prompt to specify which entities you want to extract.

Run the pipeline to produce structured extraction outputs.

Analyze results in extractionresults.jsonl (for downstream tasks) or use visualization.html for a summary.

Example Entities
Entity Class	Example Extracted Value
ORGANIZATION	SBI Credit Card
DATE	February 5, 2025
MONEY	12,450
PERSON	Ramesh Verma
LOCATION	Bengaluru
ROLE	Cardholder
ACCOUNTNUMBER	4111-5678-9012-3456
PERCENT	5
CONTRACTREFERENCE	Transaction ID TXN-778899
